<div align="center">

# Imran Siddique

**The safety, trust, and reliability platform for production AI agents**

*We are building the Kubernetes for AI agent governance*

[![Website](https://img.shields.io/badge/imransiddique.com-blue?style=flat-square&logo=google-chrome&logoColor=white)](https://imransiddique.com)
[![PyPI](https://img.shields.io/badge/pip_install-agent--governance-blue?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/agent-governance/)
[![GitHub](https://img.shields.io/badge/GitHub-imran--siddique-181717?style=flat-square&logo=github)](https://github.com/imran-siddique)
[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4%EF%B8%8F-ff69b4?style=flat-square)](https://github.com/sponsors/imran-siddique)

</div>

---

## The Problem

The AI agent market is projected to reach **$47B by 2030**. Enterprises are deploying autonomous agents that execute tools, access sensitive data, and make decisions -- with **no built-in governance, audit trails, or policy enforcement**.

A2A gives agents a common language. MCP gives agents tools. **Neither enforces trust.**

## The Solution: Agent Governance Ecosystem

An open-source stack for governing autonomous AI agents in production -- the **SSL/TLS equivalent for AI agent-to-agent communication**.

```
pip install agent-governance[full]
```

```
+------------------------------------------------------------------+
|                    AGENT GOVERNANCE STACK                         |
+------------------------------------------------------------------+
|  AGENT HYPERVISOR  |  Runtime supervisor, Execution Rings (0-3)  |
|    (Runtime)       |  Joint Liability, Saga Orchestration         |
+--------------------+---------------------------------------------+
|  AGENT SRE         |  SLOs, chaos testing, canary deploys        |
|    (Reliability)   |  Incident response, runbook automation      |
+--------------------+---------------------------------------------+
|  AGENTMESH         |  Zero-trust identity, mTLS, protocol bridge |
|    (Trust)         |  A2A + MCP + IATP, behavioral scoring       |
+--------------------+---------------------------------------------+
|  AGENT OS          |  Policy enforcement kernel, <0.1ms p99      |
|    (Kernel)        |  Capability-based access, Merkle audit logs |
+------------------------------------------------------------------+
```

### Repositories

| Component | Description | Tests | Install |
|-----------|-------------|-------|---------|
| [**Agent OS**](https://github.com/imran-siddique/agent-os) | Governance kernel -- policy enforcement in <0.1ms p99 | 1,500+ | `pip install agent-os-kernel` |
| [**AgentMesh**](https://github.com/imran-siddique/agent-mesh) | SSL for AI Agents -- zero-trust agent communication | 1,400+ | `pip install agentmesh-platform` |
| [**Agent Hypervisor**](https://github.com/imran-siddique/agent-hypervisor) | Runtime supervisor with Execution Rings and Saga Orchestration | 326+ | `pip install agent-hypervisor` |
| [**Agent SRE**](https://github.com/imran-siddique/agent-sre) | SRE for AI agents -- SLOs, chaos testing, observability | 1,070+ | `pip install agent-sre` |
| [**agent-governance**](https://github.com/imran-siddique/agent-governance) | Meta-package -- full stack in one install | -- | `pip install agent-governance[full]` |

**Total: 4,300+ tests | 5 repos | 17 modules | 6 framework integrations**

### Production Integrations

<p align="center">
  <a href="https://github.com/langgenius/dify-plugins/pull/2060"><img src="https://img.shields.io/badge/Dify-65K_%E2%AD%90_Merged-success?style=for-the-badge" alt="Dify"></a>
  <a href="https://github.com/run-llama/llama_index/pull/20644"><img src="https://img.shields.io/badge/LlamaIndex-47K_%E2%AD%90_Merged-success?style=for-the-badge" alt="LlamaIndex"></a>
  <a href="https://github.com/nicepkg/awesome-github-copilot/pull/26"><img src="https://img.shields.io/badge/GitHub_Copilot-21.6K_%E2%AD%90_Merged-success?style=for-the-badge" alt="Copilot"></a>
  <a href="https://github.com/microsoft/agent-lightning/pull/478"><img src="https://img.shields.io/badge/Agent_Lightning-15K_%E2%AD%90_Merged-success?style=for-the-badge" alt="Agent-Lightning"></a>
</p>

Active proposals at **20+ major AI frameworks**: OpenAI, Anthropic, Google A2A, Oracle, AutoGen, CrewAI, Haystack, PydanticAI, Semantic Kernel, and more.

---

### What Makes This Different?

Most frameworks focus on **building agents**. We focus on **governing them**:

| Capability | How It Works |
|------------|-------------|
| **Execution Rings** | CPU ring-inspired privilege isolation (Ring 0-3) for AI agents |
| **Joint Liability** | Shapley-value fault attribution across agent groups |
| **Saga Orchestration** | Multi-agent transactions with automatic compensation |
| **Cryptographic Trust** | DID-based identity, Merkle audit trails, behavioral scoring |
| **SLO-Driven Reliability** | Error budgets, chaos testing, canary deploys |
| **<0.1ms Governance** | Deterministic policy enforcement with zero agent code changes |

---

<div align="center">

**Star the repos to help others discover AI agent governance**

[![Agent OS](https://img.shields.io/github/stars/imran-siddique/agent-os?style=social&label=Agent%20OS)](https://github.com/imran-siddique/agent-os)
[![AgentMesh](https://img.shields.io/github/stars/imran-siddique/agent-mesh?style=social&label=AgentMesh)](https://github.com/imran-siddique/agent-mesh)
[![Agent Hypervisor](https://img.shields.io/github/stars/imran-siddique/agent-hypervisor?style=social&label=Hypervisor)](https://github.com/imran-siddique/agent-hypervisor)
[![Agent SRE](https://img.shields.io/github/stars/imran-siddique/agent-sre?style=social&label=Agent%20SRE)](https://github.com/imran-siddique/agent-sre)

**[imransiddique.com](https://imransiddique.com)** | **[Documentation](https://imransiddique.com/agent-os-docs/)**

</div>
