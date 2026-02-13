---
layout: default
title: Home
---

<section class="hero">
    <div class="container">
        <img src="{{ site.baseurl }}/assets/images/logo.png" alt="KubeDesk Logo" class="hero-logo" width="100" style="width: 100px; height: auto;">
        <h1>The Desktop Client for Kubernetes Cluster Management</h1>
        <p class="subtitle">Gain complete visibility into your clusters. Browse, inspect, and analyze all Kubernetes objects in real-time. Built with Electron, React, and Go.</p>
        
        <div class="download-buttons">
            <!-- macOS Dropdown -->
            <div class="dropdown">
                <a href="#" class="btn-pill btn-mac">
                    <img src="{{ site.baseurl }}/assets/images/apple.svg" class="os-icon" alt="macOS">
                    <span>Download for macOS</span>
                </a>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-arm64.dmg">Apple Silicon (M1/M2/M3)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-mac-x64.dmg">Intel Chip</a>
                </div>
            </div>

            <!-- Windows Dropdown -->
            <div class="dropdown">
                <a href="#" class="btn-pill btn-win">
                    <img src="{{ site.baseurl }}/assets/images/windows.svg" class="os-icon" alt="Windows">
                    <span>Download for Windows</span>
                </a>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Setup.exe">Installer (.exe)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk-Portable.exe">Portable (.exe)</a>
                </div>
            </div>

            <!-- Linux Dropdown -->
            <div class="dropdown">
                <a href="#" class="btn-pill btn-linux">
                    <img src="{{ site.baseurl }}/assets/images/linux.svg" class="os-icon" alt="Linux">
                    <span>Download for Linux</span>
                </a>
                <div class="dropdown-menu">
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/KubeDesk.AppImage">Portable AppImage</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/kubedesk_amd64.deb">Debian / Ubuntu (.deb)</a>
                    <a href="https://github.com/akkezi/KubeDesk/releases/latest/download/kubedesk.x86_64.rpm">RedHat / Fedora (.rpm)</a>
                </div>
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
						<img src="{{ site.baseurl }}/assets/images/screenshots/001.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/002.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/003.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/004.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/005.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/006.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/007.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/008.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/009.png" alt="Screenshot" onclick="openLightbox(this)">
            <img src="{{ site.baseurl }}/assets/images/screenshots/010.png" alt="Screenshot" onclick="openLightbox(this)">
        </div>
    </div>
</section>

<section class="app-simulator-section">
    <div class="container">
        <h2>Comprehensive Object Visibility</h2>
        <p class="subtitle">Explore the full capabilities of KubeDesk. Click on a category to view supported objects.</p>
        
    <div class="app-simulator">
            <!-- Sidebar -->
            <div class="app-sidebar">
                <div class="sidebar-item active" onclick="switchTab(this, 'dashboard')">
                    <span class="icon">📊</span> Dashboard & Events
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'infrastructure')">
                    <span class="icon">🏗️</span> Infrastructure
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'workloads')">
                    <span class="icon">📦</span> Workloads
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'configuration')">
                    <span class="icon">⚙️</span> Configuration
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'networking')">
                    <span class="icon">🌐</span> Networking
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'storage')">
                    <span class="icon">💾</span> Storage
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'access')">
                    <span class="icon">🔑</span> Access Control
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'admission')">
                    <span class="icon">🛡️</span> Admission Control
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'dynamic')">
                    <span class="icon">⚡</span> Dynamic Resource
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'applications')">
                    <span class="icon">🚀</span> Applications
                </div>
                <div class="sidebar-item" onclick="switchTab(this, 'crd')">
                    <span class="icon">🧩</span> Custom Resources
                </div>
            </div>

            <!-- Content Area -->
            <div class="app-content">
                <!-- Dashboard -->
                <div id="dashboard" class="tab-content active">
                    <h3>📊 Dashboard & Events</h3>
                    <div class="content-grid">
                        <div class="content-card">Dashboard Overview</div>
                        <div class="content-card">Cluster Events</div>
                    </div>
                </div>

                <!-- Infrastructure -->
                <div id="infrastructure" class="tab-content">
                    <h3>🏗️ Infrastructure</h3>
                    <div class="content-grid">
                        <div class="content-card">Nodes</div>
                        <div class="content-card">Namespaces</div>
                        <div class="content-card">Resource Quotas</div>
                        <div class="content-card">Limit Ranges</div>
                        <div class="content-card">Leases</div>
                    </div>
                </div>

                <!-- Workloads -->
                <div id="workloads" class="tab-content">
                    <h3>📦 Workloads</h3>
                    <div class="content-grid">
                        <div class="content-card">Pods</div>
                        <div class="content-card">Pod Template</div>
                        <div class="content-card">Deployments</div>
                        <div class="content-card">StatefulSets</div>
                        <div class="content-card">DaemonSets</div>
                        <div class="content-card">ReplicaSets</div>
                        <div class="content-card">Replication Controllers</div>
                        <div class="content-card">Jobs</div>
                        <div class="content-card">CronJobs</div>
                    </div>
                </div>

                <!-- Configuration -->
                <div id="configuration" class="tab-content">
                    <h3>⚙️ Configuration</h3>
                    <div class="content-grid">
                        <div class="content-card">Config Maps</div>
                        <div class="content-card">Secrets</div>
                        <div class="content-card">Runtime Classes</div>
                        <div class="content-card">Horizontal Pod Autoscalers</div>
                        <div class="content-card">Pod Disruption Budgets</div>
                        <div class="content-card">Priority Classes</div>
                    </div>
                </div>

                <!-- Networking -->
                <div id="networking" class="tab-content">
                    <h3>🌐 Networking</h3>
                    <div class="content-grid">
                        <div class="content-card">Services</div>
                        <div class="content-card">Endpoints</div>
                        <div class="content-card">Endpoint Slices</div>
                        <div class="content-card">Ingress</div>
                        <div class="content-card">Ingress Classes</div>
                        <div class="content-card">Network Policies</div>
                    </div>
                </div>

                <!-- Storage -->
                <div id="storage" class="tab-content">
                    <h3>💾 Storage</h3>
                    <div class="content-grid">
                        <div class="content-card">Storage Classes</div>
                        <div class="content-card">Persistent Volumes</div>
                        <div class="content-card">Persistent Volume Claims</div>
                        <div class="content-card">Volume Attachments</div>
                        <div class="content-card">Volume Attributes Classes</div>
                        <div class="content-card">CSI Drivers</div>
                        <div class="content-card">CSI Nodes</div>
                        <div class="content-card">CSI Storage Capacities</div>
                    </div>
                </div>

                <!-- Access Control -->
                <div id="access" class="tab-content">
                    <h3>🔑 Access Control</h3>
                    <div class="content-grid">
                        <div class="content-card">Service Accounts</div>
                        <div class="content-card">Roles</div>
                        <div class="content-card">Role Bindings</div>
                        <div class="content-card">Cluster Roles</div>
                        <div class="content-card">Cluster Role Bindings</div>
                        <div class="content-card">Certificate Signing Request</div>
                    </div>
                </div>

                <!-- Admission Control -->
                <div id="admission" class="tab-content">
                    <h3>🛡️ Admission Control</h3>
                    <div class="content-grid">
                        <div class="content-card">Mutating Webhook Configurations</div>
                        <div class="content-card">Validating Webhook Configurations</div>
                        <div class="content-card">Validating Admission Policies</div>
                        <div class="content-card">Validating Admission Policy Bindings</div>
                    </div>
                </div>

                <!-- Dynamic Resource Allocation -->
                <div id="dynamic" class="tab-content">
                    <h3>⚡ Dynamic Resource Allocation</h3>
                    <div class="content-grid">
                        <div class="content-card">Device Classes</div>
                        <div class="content-card">Resource Claims</div>
                        <div class="content-card">Resource Claim Templates</div>
                        <div class="content-card">Resource Slices</div>
                    </div>
                </div>

                <!-- Applications -->
                <div id="applications" class="tab-content">
                    <h3>🚀 Applications</h3>
                    <div class="content-grid">
                        <div class="content-card">Helm Charts</div>
                        <div class="content-card">Helm Repositories</div>
                        <div class="content-card">Helm Releases</div>
                        <div class="content-card">Kustomize (Planned)</div>
                        <div class="content-card">Operator Lifecycle Manager (Planned)</div>
                        <div class="content-card">GitOps (Planned)</div>
                        <div class="content-card">Argo CD (Planned)</div>
                        <div class="content-card">Flux CD (Planned)</div>
                    </div>
                </div>

                <!-- Custom Resources -->
                <div id="crd" class="tab-content">
                    <h3>🧩 Custom Resources</h3>
                    <div class="content-grid">
                        <div class="content-card">Definitions</div>
                        <div class="content-card">CRDs</div>
                    </div>
                </div>
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
                <div class="code-header">Installer versions</div>
                <pre><code># Coming soon
														 Coming soon
										 </code>
								</pre>
            </div>
            <div class="code-block">
                <div class="code-header">Portable versions</div>
                <pre><code># Coming soon
														 Coming soon
										  </code>
								</pre>
            </div>
        </div>
        <div class="cta-bottom">
            <a href="https://github.com/akkezi/KubeDesk/releases" class="btn btn-secondary">View all releases on GitHub</a>
        </div>
    </div>
</section>
