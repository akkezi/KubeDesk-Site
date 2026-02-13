---
layout: default
title: Home
---

<section class="hero">
    <div class="container">
        <img src="{{ site.baseurl }}/assets/images/logo.png" alt="KubeDesk Logo" class="hero-logo" width="100" style="width: 100px; height: auto;">
        <h1>The Desktop Client for Kubernetes Cluster Management</h1>
        <p class="subtitle">Gain complete visibility into your clusters. Browse, inspect, and analyze all Kubernetes objects in real-time. Built with Electron, React, and Go.</p>
        
            <!-- macOS Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-mac">
                    <img src="{{ site.baseurl }}/assets/images/apple.svg" class="os-icon" alt="macOS">
                    <span>Download for macOS</span>
                </button>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-arm64.dmg">Apple Silicon (M1/M2/M3)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-x64.dmg">Intel Chip</a>
                </div>
            </div>

            <!-- Windows Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-win">
                    <img src="{{ site.baseurl }}/assets/images/windows.svg" class="os-icon" alt="Windows">
                    <span>Download for Windows</span>
                </button>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Setup.exe">Installer (.exe)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Portable.exe">Portable (.exe)</a>
                </div>
            </div>

            <!-- Linux Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-linux">
                    <img src="{{ site.baseurl }}/assets/images/linux.svg" class="os-icon" alt="Linux">
                    <span>Download for Linux</span>
                </button>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk.AppImage">Portable AppImage</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/kubedesk_amd64.deb">Debian / Ubuntu (.deb)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/kubedesk.x86_64.rpm">RedHat / Fedora (.rpm)</a>
                </div>
            </div>
        
        <div class="hero-image">
            <img src="{{ site.baseurl }}/assets/images/screenshots/001.png" alt="KubeDesk Dashboard" class="app-screenshot">
        </div>
    </div>
</section>

<section class="features">
    <div class="container">
        <h2>Unmatched Observability & Visualization</h2>
        <div class="feature-grid">
            <div class="feature-card">
                <h3>🔄 Multi-Cluster Management</h3>
                <p>Switch between multiple Kubernetes clusters seamlessly from a single interface. Monitor all your environments without context switching.</p>
            </div>
            <div class="feature-card">
                <h3>👀 Ultimate Resource Viewer</h3>
                <p>Browse all your K8s resources with a beautiful and intuitive UI. Designed for administrators to audit and inspect cluster status.</p>
            </div>
            <div class="feature-card">
                <h3>📜 Real-time Logs</h3>
                <p>Stream pod logs instantly in read-only mode. Filter, search, and analyze logs to diagnose issues faster.</p>
            </div>
            <div class="feature-card">
                <h3>📄 Manifest Viewer</h3>
                <p>Inspect the full YAML configuration of any object. syntax highlighting helps you understand exactly how your resources are defined.</p>
            </div>
            <div class="feature-card">
                <h3>⚓ Helm Deployment & Catalog</h3>
                <p>Deploy Helm charts directly to your cluster. Browse and install from a rich catalog of available Helm repositories.</p>
            </div>
             <div class="feature-card">
                <h3>🧩 Custom Resource Inspection</h3>
                <p>Native support for viewing Custom Resource Definitions (CRDs) and their instances. See the full picture of your extensions.</p>
            </div>
        </div>
    </div>
</section>

<section class="gallery">
    <div class="container">
        <div class="gallery-scroll">
            <img src="{{ site.baseurl }}/assets/images/screenshots/002.png" alt="Cluster View">
            <img src="{{ site.baseurl }}/assets/images/screenshots/003.png" alt="Pod Details">
            <img src="{{ site.baseurl }}/assets/images/screenshots/004.png" alt="Terminal">
            <img src="{{ site.baseurl }}/assets/images/screenshots/005.png" alt="Settings">
             <img src="{{ site.baseurl }}/assets/images/screenshots/009.png" alt="Logs">
        </div>
    </div>
</section>

<section class="object-visibility">
    <div class="container">
        <h2>Comprehensive Object Visibility</h2>
        <p class="subtitle">Access detailed information for every Kubernetes object without touching the CLI.</p>
        <div class="object-grid">
            <div class="object-category">
                <h3>Dashboard & Events</h3>
                <ul>
                    <li>Dashboard Overview</li>
                    <li>Cluster Events</li>
                </ul>
            </div>
            <div class="object-category">
                <h3>Infrastructure</h3>
                <ul>
                    <li>Nodes</li>
                    <li>Namespaces</li>
                    <li>Resource Quotas</li>
                    <li>Limit Ranges</li>
                    <li>Leases</li>
                </ul>
            </div>
            <div class="object-category">
                <h3>Workloads</h3>
                <ul>
                    <li>Pods & Templates</li>
                    <li>Deployments</li>
                    <li>StatefulSets</li>
                    <li>DaemonSets</li>
                    <li>ReplicaSets</li>
                    <li>Jobs & CronJobs</li>
                    <li>Replication Controllers</li>
                </ul>
            </div>
             <div class="object-category">
                <h3>Configuration</h3>
                <ul>
                    <li>ConfigMaps</li>
                    <li>Secrets</li>
                    <li>Runtime Classes</li>
                    <li>HPA</li>
                    <li>Pod Disruption Budgets</li>
                    <li>Priority Classes</li>
                </ul>
            </div>
            <div class="object-category">
                <h3>Networking</h3>
                <ul>
                    <li>Services</li>
                    <li>Endpoints & Slices</li>
                    <li>Ingress & Classes</li>
                    <li>Network Policies</li>
                </ul>
            </div>
            <div class="object-category">
                <h3>Storage</h3>
                <ul>
                    <li>Storage Classes</li>
                    <li>Persistent Volumes (PV)</li>
                    <li>Volume Claims (PVC)</li>
                    <li>Volume Attachments</li>
                    <li>CSI Drivers & Nodes</li>
                </ul>
            </div>
            <div class="object-category">
                <h3>Access Control</h3>
                <ul>
                    <li>Service Accounts</li>
                    <li>Roles & Bindings</li>
                    <li>Cluster Roles & Bindings</li>
                    <li>CSR</li>
                </ul>
            </div>
            <div class="object-category">
                <h3>Admission & Dynamic</h3>
                <ul>
                    <li>Mutating/Validating Webhooks</li>
                    <li>Validating Policies</li>
                    <li>Device Classes</li>
                    <li>Resource Claims</li>
                </ul>
            </div>
             <div class="object-category">
                <h3>Applications & CRDs</h3>
                <ul>
                    <li>Helm Charts & Releases</li>
                    <li>Repositories</li>
                    <li>Custom Resource Definitions</li>
                    <li>GitOps (Planned)</li>
                </ul>
            </div>
        </div>
    </div>
</section>

<section class="tech-stack">
    <div class="container">
        <h2>Built on Modern Tech</h2>
        <p class="stack-subtitle">Engineered for performance and reliability.</p>
        <div class="stack-grid">
            <div class="stack-item"><span>⚛️</span> React</div>
            <div class="stack-item"><span>📘</span> TypeScript</div>
            <div class="stack-item"><span>🐹</span> Go (Backend)</div>
            <div class="stack-item"><span>⚡</span> Electron</div>
            <div class="stack-item"><span>🚀</span> Turborepo</div>
        </div>
    </div>
</section>

<section class="installation">
    <div class="container">
        <h2>Installation</h2>
        <p class="install-subtitle">Get started in seconds. Download the latest release related to your OS.</p>
        <div class="install-tabs">
            <div class="code-block">
                <div class="code-header">Windows (Coming to Winget soon)</div>
                <pre><code># Download the installer from Releases
KubeDesk Setup 0.3.4.exe</code></pre>
            </div>
            <div class="code-block">
                <div class="code-header">Portable</div>
                <pre><code># Run without installation
KubeDesk 0.3.4.exe</code></pre>
            </div>
        </div>
        <div class="cta-bottom">
            <a href="https://github.com/akkezi/KubeDesk/releases" class="btn btn-secondary">View all releases on GitHub</a>
        </div>
    </div>
</section>
