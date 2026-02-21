# 🌊 Danube Messaging

**Danube is an open-source, distributed messaging broker system, built in Rust**

Danube aims to be a lightweight yet powerful, secure and scalable messaging platform, suitable for event-driven applications
Sub-second dispatch + cloud economics. One broker, two modes: best-effort pub/sub or at-least-once streaming with WAL + object storage.

[![Documentation](https://img.shields.io/badge/📖_Read_the_Docs-blue?style=for-the-badge)](https://danube-docs.dev-state.com/)
[![Quick Start](https://img.shields.io/badge/🚀_Docker_Quick_Start-green?style=for-the-badge)](https://danube-docs.dev-state.com/getting_started/Danube_docker_compose/)

---

## ⚡ Why Danube?
 
### 🌩️ **Cloud-Native Stateless Architecture**
Zero broker state—metadata in ETCD, data in WAL + S3/GCS/Azure. Scale horizontally in seconds without data migration. Add or remove brokers instantly. Infinite retention without local disk limits. True cloud economics.
 
### 🎯 **Self-Optimizing Clusters**
Intelligent load management continuously monitors broker health and automatically rebalances topics to prevent hotspots. New topics land on the least-loaded broker. Workload changes? The cluster adapts without manual intervention.

### 🤖 **AI-Native Administration**
Manage your cluster through natural language with Claude, Cursor, or Windsurf. 32 intelligent tools accessible via Model Context Protocol (MCP), create topics, analyze lag, troubleshoot issues, query metrics, all by conversation. CLI, Web UI, or AI: your choice.

### 🔥 **Two-Speed Dispatch**
- **Non-Reliable**: Zero persistence, sub-millisecond latency for real-time metrics and live telemetry
- **Reliable**: At-least-once delivery with WAL + cloud durability for critical workloads
 
### 📋 **Built-In Schema Registry**
Centralized schema versioning with compatibility enforcement across JSON Schema, Avro, and Protobuf. Prevent schema drift and invalid messages before they reach consumers. Single source of truth for your data contracts.
 
### 🔌 **Pure Rust Connector SDK**
Plug-and-play integrations with MQTT, databases, Kafka, ClickHouse, vector databases, and more. Framework isolated from broker core—build connectors without touching cluster internals.

---

## 🏗️ The Danube Ecosystem

- **[danube](https://github.com/danube-messaging/danube)** - The messaging broker, a lightweight, cloud‑native messaging platform built in Rust.
- **[danube-connect-core](https://github.com/danube-messaging/danube-connect-core)** - Core SDK for building high-performance connectors
- **[danube-connectors](https://github.com/danube-messaging/danube-connectors)** - Available connectors for Danube Messaging
- **[danube-cli](https://github.com/danube-messaging/danube/tree/main/danube-cli)** - Command-line companion for interacting with Danube messaging system
- **[danube-admin](https://github.com/danube-messaging/danube/tree/main/danube-admin-cli)** - Unified admin tool (CLI + AI/MCP + Web UI)

## 📦 Client Libraries
- 🦀 **[danube-client](https://github.com/danube-messaging/danube/tree/main/danube-client)** - Danube Rust client library (SDK)
- 🐹 **[danube-go](https://github.com/danube-messaging/danube-go)** - Danube Go client library (SDK)
- ♨️ **[danube-java](https://github.com/danube-messaging/danube-java)** - Danube Java client library (SDK)
- 🐍 **[danube-py](https://github.com/danube-messaging/danube-py)** - Danube Python client library (SDK)   

## 📚 Learn More

- **[Documentation](https://danube-docs.dev-state.com/)** - Architecture, concepts, and guides
- **[Getting Started](https://danube-docs.dev-state.com/getting_started/Danube_docker_compose/)** - Deploy your first cluster
- **[Client Libraries](https://danube-docs.dev-state.com/client_libraries/setup/)** - Rust and Go SDKs
- **[Schema Registry](https://danube-docs.dev-state.com/concepts/schema_registry_guide/)** - Type-safe messaging

---

## 🤝 Get Involved

- **⭐ Star the repo** - Show your support!
- **🐛 Report issues** - Help us improve
- **💡 Contribute** - PRs welcome across all repos
- **📣 Join discussions** - Share ideas and feedback

---

<div align="center">

**Built with 🦀 Rust • Designed for ☁️ Cloud • Made for 🚀 Scale**

[GitHub](https://github.com/danube-messaging) • [Docs](https://danube-docs.dev-state.com/)

</div>
