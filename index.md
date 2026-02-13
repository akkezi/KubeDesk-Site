---
layout: default
title: Home
---

<section class="hero">
    <div class="container">
        <h1>The Desktop Client for Kubernetes Cluster Management</h1>
        <p class="subtitle">Gain complete visibility into your clusters. Browse, inspect, and analyze all Kubernetes objects in real-time. Built with Electron, React, and Go.</p>
        
            <!-- macOS Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-mac">
                    <svg class="os-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="currentColor" d="M318.7 268.7c-.2-36.7 16.4-64.4 50-84.8-18.8-26.9-47.2-41.7-84.7-44.6-35.5-2.8-74.3 20.7-88.5 20.7-15 0-49.4-19.7-76.4-19.7C63.3 141.2 4 184.8 4 273.5q0 39.3 14.4 81.2c12.8 36.7 59 126.7 107.2 125.2 25.2-.6 43-17.9 75.8-17.9 31.8 0 48.3 17.9 76.4 17.9 48.6-.7 90.4-82.5 102.6-119.3-65.2-30.7-61.7-90-61.7-91.9zm-56.6-164.2c27.3-32.4 24.8-61.9 24-72.5-24.1 1.4-52 16.4-67.9 34.9-17.5 19.8-27.8 44.3-25.6 71.9 26.1 2 52.3-11.4 69.5-34.3z"/></svg>
                    Download for macOS
                </button>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-arm64.dmg">Apple Silicon (M1/M2/M3)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-x64.dmg">Intel Chip</a>
                </div>
            </div>

            <!-- Windows Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-win">
                    <svg class="os-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--!Font Awesome Free 6.5.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2024 Fonticons, Inc.--><path fill="currentColor" d="M0 93.7l183.6-25.3v177.4H0V93.7zm0 324.6l183.6 25.3V268.4H0v149.9zm203.8 28L448 480V268.4H203.8v177.9zm0-380.6v180.1H448V32L203.8 65.7z"/></svg>
                    Download for Windows
                </button>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Setup.exe">Installer (.exe)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Portable.exe">Portable (.exe)</a>
                </div>
            </div>

            <!-- Linux Dropdown -->
            <div class="dropdown">
                <button class="btn-pill btn-linux">
                    <svg class="os-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
                        <path fill="#F0C419" d="M388.2 386.4c-8.4-15.6-26.6-21.4-44.4-17 0 0-8.6 3.2-16.2 16.4 1 20 6.6 47.8-13.8 54.4-18.4 6-40.8-16.6-54.8-15.6-13.4.8-49 43.6 22 56 46.2 8 83-20.2 83-20.2 36.8-9 24.2-74 24.2-74zM107.6 386.4c8.4-15.6 26.6-21.4 44.4-17 0 0 8.6 3.2 16.2 16.4-1 20-6.6 47.8 13.8 54.4 18.4 6 40.8-16.6 54.8-15.6 13.4.8 49 43.6-22 56-46.2 8-83-20.2-83-20.2-36.8-9-24.2-74-24.2-74z"/>
                        <path fill="#000" d="M256 36.4C140.2 36.4 74 186.2 74 248.6c0 62.4-7.4 68.2-7.4 97.4 0 55.4 34 50.2 34 50.2 0-38.6 19.6-57.8 19.6-57.8 7.4-46.4 47.4-30 64-24.8 16.6 5.2 41.2 5.2 60.8 1.4-12.8-59.8-70.8-71.2-87.4-65.8-9-34.8 18-93.2 96-93.2 79.4 0 102.6 57.6 97.8 93.2-16.6-5.4-74.6 6.2-87.4 65.8 19.6 3.8 44.2 3.8 60.8-1.4 16.6-5.2 56.6-21.6 64 24.8 0 0 19.6 19.2 19.6 57.8 0 0 34 5.2 34-50.2 0-29.2-7.4-35-7.4-97.4C438 186.2 371.8 36.4 256 36.4z"/>
                        <path fill="#FFF" d="M331 298c-1.2-9-33.8-15.6-75-15.6-41.2 0-73.8 6.6-75 15.6-1.8 14.2 19.2 65.8 75 65.8 55.8 0 76.8-51.6 75-65.8z"/>
                        <path fill="#F0C419" d="M304 258.4c0 3.2-14.8 18.2-48.4 18.2-33.2 0-48.4-15.2-48.4-18.2 0-3.6 19.2-10 48.4-10 29.8 0 48.4 6.4 48.4 10z"/>
                        <ellipse cx="218.4" cy="189.4" rx="10.8" ry="17.6" fill="#FFF"/>
                        <ellipse cx="293.4" cy="189.4" rx="10.8" ry="17.6" fill="#FFF"/>
                        <circle cx="219.4" cy="191.8" r="4.2" fill="#000"/>
                        <circle cx="292.4" cy="191.8" r="4.2" fill="#000"/>
                    </svg>
                    Download for Linux
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
