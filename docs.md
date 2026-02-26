---
layout: default
title: Documentation
---

<div class="markdown-content">

# Documentation

Welcome to the KubeDesk documentation. KubeDesk is a native desktop application for Kubernetes cluster management, built with Electron, React, and Go.

## Getting Started

### 1. Download KubeDesk

Download the latest release for your operating system from the [Releases page](https://github.com/akkezi/KubeDesk/releases):

- **macOS (Apple Silicon)** — `KubeDesk-mac-arm64.dmg`
- **macOS (Intel)** — `KubeDesk-mac-x64.dmg`
- **Windows** — `KubeDesk-win-x64.exe`
- **Linux (AppImage)** — `KubeDesk-linux-x86_64.AppImage`
- **Linux (Debian/Ubuntu)** — `KubeDesk-linux-amd64.deb`

### 2. Install KubeDesk

- **macOS**: Open the `.dmg` file and drag KubeDesk to your Applications folder.
- **Windows**: Run the `.exe` installer and follow the setup wizard.
- **Linux (AppImage)**: Make the file executable (`chmod +x`) and run it directly.
- **Linux (deb)**: Install with `sudo dpkg -i KubeDesk-linux-amd64.deb`.

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

| Component | Minimum Version |
|---|---|
| Kubernetes | 1.20+ |
| kubeconfig | Any valid kubeconfig file |
| macOS | 11 (Big Sur) or later |
| Windows | Windows 10 or later |
| Linux | Ubuntu 20.04+ / Fedora 34+ or equivalent |

## Configuration

KubeDesk reads from your existing kubeconfig file and respects all configured contexts, namespaces, and cluster credentials. No additional configuration is required.

## Source Code

KubeDesk is fully open source. Explore the source code, report issues, or contribute on GitHub:

- **Repository**: [github.com/akkezi/KubeDesk](https://github.com/akkezi/KubeDesk)
- **Issues**: [github.com/akkezi/KubeDesk/issues](https://github.com/akkezi/KubeDesk/issues)
- **Releases**: [github.com/akkezi/KubeDesk/releases](https://github.com/akkezi/KubeDesk/releases)

## License

KubeDesk is released under the [MIT License]({{ site.baseurl }}/terms).

</div>
