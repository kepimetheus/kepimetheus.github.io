# Kepimetheus 🚀

> Because 2 AM you shouldn't need to remember PromQL syntax

Kepimetheus is an AI-powered natural language interface for Prometheus queries, powered by AWS Bedrock. It transforms plain English into PromQL, making monitoring more accessible for everyone.

<div align="center">
  <img src="logo.png" alt="Kepimetheus Logo" width="200">
</div>

## 🌟 Features

- **Natural Language to PromQL**: Write queries in plain English
- **AWS Bedrock Integration**: Enterprise-grade LLM capabilities
- **Grafana Plugin**: Native integration with your dashboards
- **Helm Installation**: Deploy in seconds
- **Production Ready**: Built for real-world monitoring needs

## 🚀 Quick Start

### Prerequisites

- Kubernetes cluster
- Helm v3+
- Prometheus installed
- AWS credentials configured

### Installation

```bash
# Add Kepimetheus Helm repository
helm repo add kepimetheus https://kepimetheus.github.io/charts

# Install Kepimetheus
helm install kepimetheus kepimetheus/kepimetheus
```

## 📖 Usage

```bash
# Example: Query CPU usage in plain English
kepimetheus query "Show me CPU usage for production namespace pods"

# Output: Generates and executes PromQL query
rate(container_cpu_usage_seconds_total{namespace="production"}[5m])
```

## 🛠️ Configuration


## 🔒 Security

- AWS IAM authentication supported
- RBAC enabled by default
- Secure by design

## 🤝 Contributing

We love contributions! Please read our [Contributing Guide](CONTRIBUTING.md) first.

```bash
# Development setup
git clone https://github.com/kepimetheus/kepimetheus.git
cd kepimetheus
make dev
```

## 📝 License

[Apache 2.0](LICENSE)

## 🎮 About

Created by Rodrigo Melgar, an OpenSource who believes Kubernetes is just Tetris for containers. When not making monitoring more accessible, he's probably explaining to his kids why blowing on NES cartridges was the original debugging technique.

## ⭐ Why "Kepimetheus"?

Because like every good Kubernetes project, we needed a 'k' prefix. Also, epimetheus.github.io was taken. Sometimes the best solutions come from DNS availability!

## 📞 Support

- 📚 [Documentation](https://kepimetheus.github.io/docs)
- 🐛 [Issue Tracker](https://github.com/kepimetheus/kepimetheus/issues)
- 💬 [Community Discord](#)

---

<div align="center">
Made with ☕ by developers who got tired of writing PromQL at 2 AM.
</div>
