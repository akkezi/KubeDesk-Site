# Technical Specification — KubeDesk Site Improvements

## Difficulty Assessment
**Medium** — Multiple coordinated changes across several files: new pages, nav/footer refactoring, mobile responsiveness, no build system means direct file edits only.

---

## Technical Context

| Item | Value |
|---|---|
| Static site generator | Jekyll (GitHub Pages compatible) |
| Theme | `jekyll-theme-slate` (overridden by custom layout) |
| Plugins | `jekyll-seo-tag` |
| CSS | Custom `assets/css/style.css` (~24 KB), dark theme, purple accent (`#7c3aed`) |
| JS | All inline in `_layouts/default.html` (lightbox, tab simulator, drag-and-drop) |
| Fonts | Google Fonts — Inter |
| Build | None (Jekyll served directly by GitHub Pages) |
| Base URL | `/kubedesk-site` |

---

## Current Issues Identified

1. **Duplicate footer** in `_layouts/default.html` (lines 35–44 and 46–55) — two `<footer class="site-footer">` elements.
2. **Footer Privacy/Terms links** point to `#` — broken placeholders.
3. **Nav "Docs" link** points to `/docs` but no docs page exists.
4. **Installation section** in `index.md` (lines 306–326) contains only "Coming soon" placeholder content — to be removed.
5. **No mobile nav toggle** — `site-nav` wraps but can overflow on narrow viewports.
6. **No Releases link** in nav.

---

## Implementation Approach

### Files to Modify
- `index.md` — remove `<section class="installation">` block
- `_layouts/default.html` — fix duplicate footer, update nav links (add Docs + Releases), update footer links to real pages, add mobile hamburger menu JS/CSS
- `assets/css/style.css` — add mobile nav styles, remove/keep `.installation` styles, add markdown content page styles for docs/privacy/terms

### Files to Create
- `privacy.md` — Privacy Policy (MIT license 2 context, no personal data collection)
- `terms.md` — Terms of Service (MIT license 2)
- `docs.md` — Documentation landing page

---

## Source Code Structure Changes

```
KubeDesk-Site/
├── _layouts/
│   └── default.html          ← MODIFY: fix footer, update nav, add mobile menu
├── assets/
│   └── css/
│       └── style.css         ← MODIFY: mobile nav, markdown page styles
├── index.md                  ← MODIFY: remove installation section
├── privacy.md                ← CREATE: Privacy Policy (MIT 2)
├── terms.md                  ← CREATE: Terms of Service (MIT 2)
└── docs.md                   ← CREATE: Documentation landing page
```

---

## Detailed Changes

### 1. `index.md` — Remove Installation Section
Remove lines 306–326 (`<section class="installation">...</section>`) entirely.  
Keep CSS class `.installation` in stylesheet in case it's referenced elsewhere (it is referenced in `.features h2, .installation h2, .tech-stack h2` selector — update that selector to remove the reference).

### 2. `_layouts/default.html` — Nav & Footer

**Navigation** — replace current 2-link nav with 4-link nav:
```html
<nav class="site-nav">
    <a href="{{ site.baseurl }}/docs">Documentation</a>
    <a href="https://github.com/akkezi/KubeDesk/releases" target="_blank">Releases</a>
    <a href="https://github.com/akkezi/KubeDesk" target="_blank">GitHub</a>
    <button class="nav-toggle" aria-label="Toggle navigation">&#9776;</button>
</nav>
```

**Footer** — merge two footers into one:
```html
<footer class="site-footer">
    <div class="container">
        <p>&copy; {{ site.time | date: "%Y" }} KubeDesk. All rights reserved.</p>
        <div class="footer-links">
            <a href="{{ site.baseurl }}/privacy">Privacy</a>
            <a href="{{ site.baseurl }}/terms">Terms</a>
            <a href="{{ site.baseurl }}/docs">Documentation</a>
            <a href="https://github.com/akkezi/KubeDesk/releases" target="_blank">Releases</a>
            <a href="https://github.com/akkezi/KubeDesk" target="_blank">GitHub</a>
            <a href="https://github.com/akkezi/KubeDesk/issues" target="_blank">Report an Issue</a>
        </div>
    </div>
</footer>
```

**Mobile nav toggle JS** — add inline script to handle `.nav-toggle` click toggling `.nav-open` on `.site-nav`.

### 3. `assets/css/style.css`

**Mobile nav styles:**
```css
.nav-toggle {
    display: none; /* hidden on desktop */
    background: none;
    border: none;
    color: var(--text-color);
    font-size: 1.5rem;
    cursor: pointer;
    padding: 4px 8px;
}

@media (max-width: 768px) {
    .nav-toggle { display: block; }
    .site-nav {
        position: fixed;
        top: 0; right: -100%;
        width: 240px; height: 100vh;
        background: rgba(1, 4, 9, 0.97);
        flex-direction: column;
        padding: 80px 30px 30px;
        gap: 24px;
        transition: right 0.3s ease;
        border-left: 1px solid var(--border-color);
        z-index: 999;
    }
    .site-nav.nav-open { right: 0; }
}
```

**Markdown content page styles** (for docs/privacy/terms):
```css
.markdown-content {
    max-width: 800px;
    margin: 0 auto;
    padding: 60px 20px;
    line-height: 1.8;
}
.markdown-content h1, .markdown-content h2, .markdown-content h3 { margin: 2rem 0 1rem; }
.markdown-content p { margin-bottom: 1rem; color: var(--text-color); }
.markdown-content ul, .markdown-content ol { padding-left: 1.5rem; margin-bottom: 1rem; }
.markdown-content a { color: var(--primary-color); }
```

**Remove `.installation` from compound selector** (line ~926):
Change `.features h2, .installation h2, .tech-stack h2` → `.features h2, .tech-stack h2`.

### 4. `privacy.md` — Privacy Policy

Front matter: `layout: default`, `title: Privacy Policy`  
Wrap content in `<div class="markdown-content">...</div>`.  
Content: MIT License 2 context — no personal data collected, no cookies beyond GitHub Pages analytics, open source under MIT. Last updated date.

### 5. `terms.md` — Terms of Service

Front matter: `layout: default`, `title: Terms of Service`  
Content: Free software terms under MIT License 2, no warranties, no liability, open source. Last updated date.

### 6. `docs.md` — Documentation Landing Page

Front matter: `layout: default`, `title: Documentation`  
Content: Getting started section, links to GitHub README, download links, feature overview, link to releases page. Wrapped in `<div class="markdown-content">`.

---

## Responsiveness Verification Points

| Screen | Element | Expected |
|---|---|---|
| < 768px | Nav | Hamburger button visible, links in slide-in drawer |
| < 768px | Hero h1 | Font size 2rem (already in CSS) |
| < 768px | Download buttons | Stacked column (already in CSS) |
| < 768px | Feature grid | Single column (already in CSS) |
| < 768px | Footer | Column layout (already in CSS) |
| < 768px | App simulator | Horizontal scrollable tabs (already in CSS) |
| < 480px | New pages (docs/privacy/terms) | Padding/font readable |

---

## Verification Approach

Jekyll has no local lint/test commands required for GitHub Pages.  
Manual verification:
1. Open `index.md` — confirm installation section is removed
2. Open `_layouts/default.html` — confirm single footer, correct nav links
3. Check `privacy.md`, `terms.md`, `docs.md` render via Jekyll layout
4. Resize browser to 375px — confirm hamburger nav appears and works
5. Confirm footer Privacy/Terms links navigate correctly
6. No broken `#` anchors remain in nav/footer
