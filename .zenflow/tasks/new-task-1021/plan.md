# Spec and build

## Configuration
- **Artifacts Path**: `.zenflow/tasks/new-task-1021`

---

## Agent Instructions

Ask the user questions when anything is unclear or needs their input. This includes:
- Ambiguous or incomplete requirements
- Technical decisions that affect architecture or user experience
- Trade-offs that require business context

Do not make assumptions on important decisions — get clarification first.

If you are blocked and need user clarification, mark the current step with `[!]` in plan.md before stopping.

---

## Workflow Steps

### [x] Step: Technical Specification
<!-- chat-id: cdd43a22-70e0-40b2-8876-a392d1e8b693 -->

Spec saved to `.zenflow/tasks/new-task-1021/spec.md`.

Difficulty: **medium**. Stack is Jekyll (GitHub Pages), no build system, pure static files.

---

### [x] Step: Remove installation section from index.md
<!-- chat-id: 90b81dd7-ff1d-499c-a970-9f809c2cf975 -->
- Delete the `<section class="installation">...</section>` block (end of `index.md`)
- Update `assets/css/style.css`: remove `.installation` from the compound `h2` selector

### [x] Step: Fix duplicate footer and update nav in default.html
<!-- chat-id: 66e7d09a-6920-4d9e-87bd-42f573a46181 -->
- Merge the two `<footer class="site-footer">` blocks into one
- Update footer links: Privacy → `/privacy`, Terms → `/terms`, add Documentation + Releases + Report an Issue
- Update nav: add Documentation (`/docs`) and Releases (GitHub releases URL) links
- Add mobile hamburger toggle button to nav
- Add inline JS for mobile nav toggle (`.nav-toggle` click → toggle `.nav-open` on `.site-nav`)

### [ ] Step: Add responsive mobile nav and markdown page styles to style.css
- Add `.nav-toggle` styles (hidden on desktop, visible on mobile)
- Add `.site-nav` mobile slide-in drawer styles + `.nav-open` state
- Add `.markdown-content` styles for docs/privacy/terms pages

### [ ] Step: Create privacy.md, terms.md, and docs.md pages
- `privacy.md`: Privacy Policy under MIT License 2 context, `layout: default`
- `terms.md`: Terms of Service under MIT License 2, `layout: default`
- `docs.md`: Documentation landing page with getting started, links to GitHub README/releases, `layout: default`
- All wrapped in `<div class="markdown-content">` for consistent styling
