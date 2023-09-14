# Helm Learning Repository

![image](https://github.com/willdadrummer/learn-helm/assets/52965466/584148cc-dc01-4e29-99b5-ce62e0439e09)

Welcome to the Helm Learning Repository! This repository is designed to help you learn how to use Helm, a package manager for Kubernetes applications. Whether you're a beginner or an experienced Kubernetes user, this guide will walk you through the basics of Helm and help you become proficient in managing your Kubernetes applications.

## Table of Contents

1. [What is Helm?](#what-is-helm)
2. [Getting Started](#getting-started)
   - [Installing Helm](#installing-helm)
3. [Basic Helm Commands](#basic-helm-commands)
   - [Chart Installation](#chart-installation)
   - [Chart Upgrades](#chart-upgrades)
   - [Chart Removal](#chart-removal)
4. [Creating Your Own Helm Charts](#creating-your-own-helm-charts)
5. [Advanced Helm Usage](#advanced-helm-usage)
   - [Helm Repositories](#helm-repositories)
   - [Helm Templates](#helm-templates)
6. [Contributing](#contributing)
7. [License](#license)

## What is Helm?

Helm is a package manager for Kubernetes that makes it easy to define, install, and upgrade even the most complex Kubernetes applications. It uses charts, which are packages of pre-configured Kubernetes resources, to simplify the deployment process.

## Getting Started

### Installing Helm

Before you can start using Helm, you need to install it on your local machine.

Binary downloads of the Helm client can be found on [the Releases page](https://github.com/helm/helm/releases/latest).

Unpack the `helm` binary and add it to your PATH and you are good to go!

If you want to use a package manager:

- [Homebrew](https://brew.sh/) users can use `brew install helm`.
- [Chocolatey](https://chocolatey.org/) users can use `choco install kubernetes-helm`.
- [Scoop](https://scoop.sh/) users can use `scoop install helm`.
- [GoFish](https://gofi.sh/) users can use `gofish install helm`.
- [Snapcraft](https://snapcraft.io/) users can use `snap install helm --classic`

To rapidly get Helm up and running, start with the [Quick Start Guide](https://helm.sh/docs/intro/quickstart/).

See the [installation guide](https://helm.sh/docs/intro/install/) for more options,
including installing pre-releases.

## Basic Helm Commands

### Chart Installation

To install a Helm chart onto your Kubernetes cluster, use the `helm install` command. Here's an example of installing a WordPress chart:

```helm install my-wordpress stable/wordpress```

### Chart Upgrades

Helm allows you to easily upgrade your deployed charts as new versions become available. Here's how to upgrade a chart:

```helm upgrade my-wordpress stable/wordpress```

### Chart Removal

When you're done with a Helm chart, you can remove it from your cluster using the `helm uninstall` command.

```helm uninstall my-wordpress```

## Creating Your Own Helm Charts

Creating custom Helm charts is a powerful way to package and deploy your Kubernetes applications. Stay tuned for detailed tutorials on creating your own charts!

## Advanced Helm Usage

### Helm Repositories

Helm allows you to manage repositories of pre-packaged charts. You can add, update, and search for charts from these repositories. Here's how to work with Helm repositories:

```helm repo add stable https://charts.helm.sh/stable```

### Updating Helm Repositories 

```helm repo update```

### Searching for Charts

```helm search repo stable/wordpress```


### Helm Templates

Helm templates are a powerful feature that allows you to customize your charts before deployment. Learn how to use Helm templates effectively:

```helm template my-wordpress stable/wordpress```

## Contributing

If you'd like to contribute to this Helm Learning Repository, feel free to fork the repository, make changes, and submit a pull request. We welcome your contributions and ideas!

## License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

Happy Helm-ing! 🚢🎩
