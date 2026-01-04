# 🌊 Danube Messaging

**Danube is an open-source, distributed messaging broker system, built in Rust**

Danube aims to be a lightweight yet powerful, secure and scalable messaging platform, suitable for event-driven applications
Sub-second dispatch + cloud economics. One broker, two modes: best-effort pub/sub or at-least-once streaming with WAL + object storage.

[![Documentation](https://img.shields.io/badge/📖_Read_the_Docs-blue?style=for-the-badge)](https://danube-docs.dev-state.com/)
[![Quick Start](https://img.shields.io/badge/🚀_Docker_Quick_Start-green?style=for-the-badge)](https://danube-docs.dev-state.com/getting_started/Danube_docker_compose/)

---

## ⚡ Why Danube?

### 🌩️ **Distributed Stateless Brokers**
All metadata in ETCD, all data in WAL + object storage (S3/GCS/Azure). Zero state on brokers means effortless horizontal scaling, add or remove brokers in seconds without data migration. Infinite retention without local disk constraints.

### 🔥 **Two Speed Gears**
- **Non-Reliable**: Zero persistence, lowest latency for real-time metrics and live telemetry
- **Reliable**: At-least-once delivery with WAL + cloud persistence for critical workloads

### 🔐 **Schema Registry Built-In**
Centralized schema management with versioning and compatibility checking. Support for JSON Schema, Avro, and Protobuf. Prevent invalid messages before they reach consumers.

### 🔌 **Plug-and-Play Connectors**
[**Danube Connect**](https://github.com/danube-messaging/danube-connect) framework for integration with external systems—MQTT, databases, Kafka, ClickHouse, vector DBs, and more. Pure Rust, isolated from broker.

---

## 🏗️ The Danube Ecosystem

### Core Platform
- **[danube](https://github.com/danube-messaging/danube)** - The messaging broker (Rust)  
  _Stateless, cloud-native, with WAL + object storage persistence_

### Client Libraries
- **[danube-client](https://github.com/danube-messaging/danube/tree/main/danube-client)** - Rust client library  
  _Async, type-safe, with full Schema Registry support_
  
- **[danube-go](https://github.com/danube-messaging/danube-go)** - Go client library  
  _Simple, idiomatic Go API for producers and consumers_

### Admin & Monitoring
- **[danube-admin-ui](https://github.com/danube-messaging/danube-admin-ui)** - Web UI for cluster management  
  _React-based dashboard for brokers, topics, and subscriptions_

### Integration Framework
- **[danube-connect](https://github.com/danube-messaging/danube-connect)** - Connector ecosystem  
  _Plug-and-play integrations with external systems_
---

## 📚 Learn More

- **[Documentation](https://danube-docs.dev-state.com/)** - Architecture, concepts, and guides
- **[Getting Started](https://danube-docs.dev-state.com/getting_started/Danube_docker_compose/)** - Deploy your first cluster
- **[Client Libraries](https://danube-docs.dev-state.com/client_libraries/producer-basics/)** - Rust and Go SDKs
- **[Schema Registry](https://danube-docs.dev-state.com/architecture/schema_registry_architecture/)** - Type-safe messaging

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
