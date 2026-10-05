# 📦 Rooibox.net — Carrier-Grade Security Suite for ISPs

Welcome to the official GitHub Organization for **Rooibox**, an open-source ecosystem designed to provide Unified XDR/SIEM, Active DNS Threat Protection, and Autonomous AI Pentesting tailored specifically for Internet Service Providers (ISPs) and Telecom operators.

---

## ⚡ Key Pillars of the Rooibox Ecosystem

- 🛡️ **Network SIEM & XDR (`rooibox/ruleset` & `rooibox/stack`):** High-performance ingestion pipeline (Vector + Wazuh + OpenSearch) built for agentless Syslog processing from Cisco, Juniper, Huawei, MikroTik, and BNGs.
- 🔒 **Carrier-Grade DNS Security (`rooibox/dns-engine` & `rooibox/threat-feeds`):** Open-source alternative to Whalebone. RPZ-based blocking on Knot Resolver to neutralize C2, botnets, and phishing attempts at the DNS level.
- 🎯 **Agentic AI Pentesting (`rooibox/attack`):** Autonomous multi-agent AI framework for continuous attack surface management and breach simulation.
- 💻 **Linux Infrastructure Protection:** Agent-based vulnerability detection, FIM, and SCA scanning for Linux servers (BNG, Billing, DNS, Virtualization).

---

## 📂 Ecosystem Repositories

| Repository | Description |
| :--- | :--- |
| **[ruleset](./ruleset)** | Custom Wazuh decoders & rulesets for telecom vendors (Cisco, Juniper, Huawei, MikroTik, BNG) |
| **[stack](./stack)** | Infrastructure-as-Code (Docker Compose & Helm Charts) with pre-configured Vector pipelines |
| **[dns-engine](./dns-engine)** | Knot Resolver configs, Lua sinkhole logic & custom Blockpage engine |
| **[threat-feeds](./threat-feeds)** | Hourly Threat Intelligence aggregator and RPZ feed builder |
| **[cli](./cli)** | The `rooibox-cli` tool for effortless GitOps updates and rule testing |
| **[docs](./docs)** | Vendor logging setup guides, architecture blueprints, and sizing calculators |

---

## 🚀 Quick Start & Deployment

Deploy the complete Rooibox Stack in a single command using our Docker Compose profile:

```bash
git clone [https://github.com/rooibox/stack.git](https://github.com/rooibox/stack.git)
cd stack/docker-compose
docker compose up -d
