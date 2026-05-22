# Danube Messaging

**An open-source pub/sub and streaming platform built in Rust. Zero external dependencies.**

Danube is a self-contained messaging platform with embedded Raft consensus for metadata replication. Secure by default with TLS/mTLS, JWT authentication, and fine-grained RBAC. Run it as **standalone** for development, **cluster** for production, or **edge** for MQTT-to-cloud IoT ingestion. One binary, three modes.

[![Documentation](https://img.shields.io/badge/📖_Read_the_Docs-blue?style=for-the-badge)](https://danube-docs.dev-state.com/)
[![Quick Start](https://img.shields.io/badge/🚀_Try_it_Now-green?style=for-the-badge)](https://danube-docs.dev-state.com/getting_started/Broker_modes/)

---

## ⚡ Three Ways to Run

🖥️ **Standalone** : single broker, zero config. Download the [binary](https://github.com/danube-messaging/danube/releases) and run `danube-broker --mode standalone --data-dir ./data`

🌐 **Cluster** : multi-broker with Raft consensus, automated topic rebalancing, and horizontal scaling. Deploy with [Docker Compose](https://danube-docs.dev-state.com/getting_started/Danube_docker_compose/) or [Kubernetes](https://danube-docs.dev-state.com/getting_started/Danube_kubernetes/)

🏭 **Edge** : MQTT gateway that ingests IoT device data, validates payloads against schemas, buffers in a local WAL, and replicates to the cluster. Designed for factory floors and remote sites where devices speak MQTT and need resilient delivery to a central platform

---

## ✨ Highlights

* **Two-speed dispatch** : non-reliable (sub-millisecond, zero persistence) or reliable (at-least-once with WAL + cloud storage)
* **Schema registry** : JSON Schema, Avro with versioning and compatibility enforcement
* **AI-native admin** : manage your cluster via natural language through [MCP](https://danube-docs.dev-state.com/danube_admin/ai_admin_assistant/) (Claude, Cursor, etc)
* **Cluster resilience** : automatic leader election, failover, and topic reconciliation on restart. Scale horizontally by adding brokers with zero downtime
* **Self-optimizing clusters** : intelligent load management that monitors broker health and automatically rebalances topics to prevent hotspots. New topics land on the least-loaded broker
* **Connector SDK** : plug-and-play integrations with databases, Kafka, ClickHouse, and more via [Danube Connect](https://github.com/danube-messaging/danube-connectors)

---

## 🏗️ Ecosystem

- **[danube](https://github.com/danube-messaging/danube)** : messaging broker (standalone, cluster, and edge modes)
- **[danube-connect-core](https://github.com/danube-messaging/danube-connect-core)** : core SDK for building connectors
- **[danube-connectors](https://github.com/danube-messaging/danube-connectors)** : available connectors

## 📦 Client Libraries

- **[Rust](https://github.com/danube-messaging/danube/tree/main/danube-client)** · **[Go](https://github.com/danube-messaging/danube-go)** · **[Java](https://github.com/danube-messaging/danube-java)** · **[Python](https://github.com/danube-messaging/danube-py)**

Contributions for other languages are welcome!

## 📚 Learn More

**[Documentation](https://danube-docs.dev-state.com/)** · **[Getting Started](https://danube-docs.dev-state.com/getting_started/Broker_modes/)** · **[Architecture](https://danube-docs.dev-state.com/architecture/architecture/)** · **[Schema Registry](https://danube-docs.dev-state.com/concepts/schema_registry_guide/)**

---

## 🤝 Get Involved

⭐ **Star the repo** · 🐛 **[Report issues](https://github.com/danube-messaging/danube/issues)** · 💡 **Contribute** (PRs welcome across all repos)
