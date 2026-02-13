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
                    <svg class="os-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><path fill="currentColor" d="M318.7 268.7c-.2-36.7 16.4-64.4 50-84.8-18.8-26.9-47.2-41.7-84.7-44.6-35.5-2.8-74.3 20.7-88.5 20.7-15 0-49.4-19.7-76.4-19.7C63.3 141.2 4 184.8 4 273.5q0 39.3 14.4 81.2c12.8 36.7 59 126.7 107.2 125.2 25.2-.6 43-17.9 75.8-17.9 31.8 0 48.3 17.9 76.4 17.9 48.6-.7 90.4-82.5 102.6-119.3-65.2-30.7-61.7-90-61.7-91.9zm-56.6-164.2c27.3-32.4 24.8-61.9 24-72.5-24.1 1.4-52 16.4-67.9 34.9-17.5 19.8-27.8 44.3-25.6 71.9 26.1 2 52.3-11.4 69.5-34.3z"/></svg>
                    <span>Download for macOS</span>
                    <svg class="arrow-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M288 32c0-17.7-14.3-32-32-32s-32 14.3-32 32V274.7l-73.4-73.4c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3l128 128c12.5 12.5 32.8 12.5 45.3 0l128-128c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0L288 274.7V32zM64 352c-35.3 0-64 28.7-64 64v32c0 35.3 28.7 64 64 64H448c35.3 0 64-28.7 64-64V416c0-35.3-28.7-64-64-64H346.5l-45.3 45.3c-25 25-65.5 25-90.5 0L165.5 352H64zM432 456c-13.3 0-24-10.7-24-24s10.7-24 24-24s24 10.7 24 24s-10.7 24-24 24z"/></svg>
                </button>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-arm64.dmg">Apple Silicon (M1/M2/M3)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-x64.dmg">Intel Chip</a>
                </div>
            </div>

            <!-- Windows Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-win">
                    <svg class="os-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><path fill="currentColor" d="M0 93.7l183.6-25.3v177.4H0V93.7zm0 324.6l183.6 25.3V268.4H0v149.9zm203.8 28L448 480V268.4H203.8v177.9zm0-380.6v180.1H448V32L203.8 65.7z"/></svg>
                    <span>Download for Windows</span>
                    <svg class="arrow-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M288 32c0-17.7-14.3-32-32-32s-32 14.3-32 32V274.7l-73.4-73.4c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3l128 128c12.5 12.5 32.8 12.5 45.3 0l128-128c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0L288 274.7V32zM64 352c-35.3 0-64 28.7-64 64v32c0 35.3 28.7 64 64 64H448c35.3 0 64-28.7 64-64V416c0-35.3-28.7-64-64-64H346.5l-45.3 45.3c-25 25-65.5 25-90.5 0L165.5 352H64zM432 456c-13.3 0-24-10.7-24-24s10.7-24 24-24s24 10.7 24 24s-10.7 24-24 24z"/></svg>
                </button>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Setup.exe">Installer (.exe)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Portable.exe">Portable (.exe)</a>
                </div>
            </div>

            <!-- Linux Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-linux">
                    <svg class="os-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="currentColor" d="M379 274.5c0 78.5-62 142.5-135 142.5-12.7 0-24.8-2-36.3-5.5l14 49c7.3 25.5-13 46.5-39.7 46.5H166c-26.7 0-47-21-39.7-46.5l14-49c-11.5 3.5-23.7 5.5-36.3 5.5-73 0-135-64-135-142.5V235c0-41.5 17-81 61.5-115C42.5 106 58 87.5 73.5 61c20.5-35 55.5-56 94.5-56s74 21 94.5 56c15.5 26.5 31 45 43 59 44.5 34 61.5 73.5 61.5 115v39.5zm-33.5-36c0-23.5-20.5-42.5-44.5-42.5h-15c-6.5 0-10 6-7 12 5.5 11 11.5 24.5 11.5 39.5 0 26-21.5 45.5-48.5 45.5-9.5 0-18.5-2.5-26.5-7-7-4-16-1-18.5 7-1 3.5-2.5 7-2.5 11 0 25.5 29 44.5 83 45.5 36.5 .5 68-18 68-111zM116 238.5c0 15 6 28.5 11.5 39.5 3 6-.5 12-7 12h-15c-24 0-44.5 19-44.5 42.5 0 93 31.5 111.5 68 111 54-1 83-20 83-45.5 0-4-1-7.5-2.5-11-2.5-7.5-11.5-10.5-18.5-7-8 4.5-17 7-26.5 7-27 0-48.5-19.5-48.5-45.5 0-15 6-28.5 11.5-39.5 3-6-.5-12-7-12h-37.5z"/></svg>
                    <span>Download for Linux</span>
                    <svg class="arrow-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path fill="currentColor" d="M288 32c0-17.7-14.3-32-32-32s-32 14.3-32 32V274.7l-73.4-73.4c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3l128 128c12.5 12.5 32.8 12.5 45.3 0l128-128c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0L288 274.7V32zM64 352c-35.3 0-64 28.7-64 64v32c0 35.3 28.7 64 64 64H448c35.3 0 64-28.7 64-64V416c0-35.3-28.7-64-64-64H346.5l-45.3 45.3c-25 25-65.5 25-90.5 0L165.5 352H64zM432 456c-13.3 0-24-10.7-24-24s10.7-24 24-24s24 10.7 24 24s-10.7 24-24 24z"/></svg>
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
