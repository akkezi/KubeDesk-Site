---
layout: default
title: Documentation
---

<div class="markdown-content" markdown="1">

# Documentation

Welcome to the KubeDesk documentation. 

KubeDesk is a Desktop Client for Kubernetes Cluster Management, built with Electron, React, and Go.

## Getting Started

### 1. Download KubeDesk

Download the latest release for your operating system from the [Site](https://akkezi.github.io/kubedesk-site/):

- **Windows (Installer)** — `KubeDesk-x.y.z_Windows_Setup.exe`
- **Windows (Portable)** — `KubeDesk-x.y.z_Windows_Portable.exe`
- **Linux (Portable AppImage)** — `KubeDesk-x.y.z_Linux_Portable.AppImage`
- **Linux (Debian/Ubuntu)** — `kubedesk-x.y.z_amd64.deb`
- **Linux (Redhat/Fedora/AlmaLinux/RockyLinux)** — `kubedesk-x.y.z.x86_64.rpm`
- **macOS (Intel Chip)** — `KubeDesk-x.y.z_macOS_intel.dmg`
- **macOS (Apple Silicon - Soon)** — `KubeDesk-x.y.z_macOS_silicon.dmg`

### 2. Install KubeDesk

- **Windows**: Run the `.exe` installer and follow the setup wizard.
- **Linux (AppImage)**: Make the file executable (`chmod +x`) and run it directly (Require `libfuse2` installed on Linux).
- **Linux (deb)**: Install with `sudo dpkg -i kubedesk-x.y.z_amd64.deb`.
- **Linux (rpm)**: Install with `sudo rpm -Uvh kubedesk-x.y.z.x86_64.rpm`.
- **macOS**: Open the `.dmg` file and drag KubeDesk to your Applications folder.

### 3. Connect to Your Cluster

KubeDesk automatically detects kubeconfig files from the default location (`~/.kube/config`). On first launch:

1. Open KubeDesk
2. Your configured clusters will appear in the cluster selector
3. Select a cluster to connect and start browsing your Kubernetes resources

## Features

- **Cluster Explorer** — Browse all Kubernetes objects: Pods, Deployments, Services, ConfigMaps, Secrets, and more
- **Real-time Updates** — Live view of resource status and events
- **Multi-cluster Support** — Switch between clusters instantly
- **Resource Inspector** — Inspect full YAML definitions and resource metadata
- **Dark Theme** — Easy on the eyes for long cluster debugging sessions

## Requirements

|   Component   |   Minimum Version   |
|---|---|
|   Kubernetes   |   1.20+   |
|   kubeconfig   |   Any valid kubeconfig file   |
|   Windows   |   Windows 10 or later   |
|   Linux (deb)   |   Debian (Buster) 10+ / Ubuntu 20.04+ / Fedora 34+ or equivalent   |
|   Linux (rpm)   |   Redhat 7+ / AlmaLinux 7+ / RockyLinux 7+ + or equivalent   |
|   macOS   |   11 (Big Sur) or later   |

## Configuration

KubeDesk reads from your existing kubeconfig file and respects all configured contexts, namespaces, and cluster credentials. 
No additional configuration is required.

## GitHub

- **Repository**: [github.com/akkezi/KubeDesk](https://github.com/akkezi/KubeDesk)
- **Issues**: [github.com/akkezi/KubeDesk/issues](https://github.com/akkezi/KubeDesk/issues)
- **Releases**: [github.com/akkezi/KubeDesk/releases](https://github.com/akkezi/KubeDesk/releases)

## License

KubeDesk is licensed under the [Mozilla Public License 2.0 (MPL-2.0)](https://www.mozilla.org/en-US/MPL/2.0/). See the [Terms of Service]({{ site.baseurl }}/terms) for details.

</div>
