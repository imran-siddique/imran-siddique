<div align="center">

# Imran Siddique

**Chief Platform Officer at [Opaque Systems](https://opaque.co) | Creator of [Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit)**

[![Website](https://img.shields.io/badge/imransiddique.com-blue?style=flat-square&logo=google-chrome&logoColor=white)](https://imransiddique.com)
[![PyPI](https://img.shields.io/badge/pip_install-ai--agent--governance-blue?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/ai-agent-governance/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-imransiddique1986-0077B5?style=flat-square&logo=linkedin)](https://linkedin.com/in/imransiddique1986)
[![Sponsor](https://img.shields.io/badge/Sponsor-ff69b4?style=flat-square)](https://github.com/sponsors/imran-siddique)

</div>

---

18 years at Microsoft building core infrastructure: SQL Azure, Azure DevOps Code Search, Azure for Industries, Microsoft Learn, and founding the Agent Governance Toolkit. In June 2026, I joined [Opaque Systems](https://opaque.co) as Chief Platform Officer. AGT is being donated to the [Agentic AI Foundation](https://agenticai.foundation) as the policy-layer standard for enterprise autonomous systems.

My approach: **Scale by Subtraction**. The most resilient systems are built by removing unnecessary complexity, not adding layers on top of it.

## The problem

Enterprises are giving AI agents real reach: email, CRMs, databases, financial systems. Most of the industry has tried to solve this at the content layer -- guardrails that screen what goes in and what comes out.

Guardrails help, but they leak. No filter reliably predicts a non-deterministic system. A single piece of untrusted content -- an email, a document, a support ticket -- can contain hidden instructions that redirect an agent into quietly exfiltrating internal data.

You don't run a regulated business on probably.

## What I'm building at Opaque

Three-layer trust architecture for the agentic AI era:

| Layer | What it does |
|-------|-------------|
| **Behavioral policy** | What an agent is allowed to do -- the policy engine I built in AGT |
| **Confidential computing** | Hardware-attested execution where data cannot leak even if the software is compromised |
| **Cryptographic proof** | Every agent action governed by policy, enforced in silicon, and auditor-ready |

Not guardrails that probably hold. Proof that they did.

## Agent Governance Toolkit

The open-source governance layer for production AI agents. Now at the Agentic AI Foundation.

```
pip install ai-agent-governance[full]
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
|  AGENTMESH         |  Zero-trust identity, DID/SPIFFE, mTLS      |
|    (Trust)         |  A2A + MCP governance, behavioral scoring   |
+--------------------+---------------------------------------------+
|  AGENT OS          |  Policy enforcement kernel, <0.1ms p99      |
|    (Kernel)        |  Capability-based access, Merkle audit logs |
+------------------------------------------------------------------+
```

**10 formal specifications | 992 conformance tests | 25 ADRs | Python SDK + .NET SDK + Rust core | 2,800+ stars | 300K+ monthly downloads**

[![AGT](https://img.shields.io/github/stars/microsoft/agent-governance-toolkit?style=social&label=Agent%20Governance%20Toolkit)](https://github.com/microsoft/agent-governance-toolkit)

### What makes this different

| Capability | How it works |
|------------|--------------|
| **Execution Rings** | CPU ring-inspired privilege isolation (Ring 0-3) for agent actions |
| **VADP** | Cryptographic delegation chains where each step narrows scope, never widens |
| **AgentMesh Identity** | DID/SPIFFE-based durable cryptographic identity, not ephemeral session tokens |
| **Decision BOM** | Reverse-traceable decision provenance via Merkle chains |
| **GovernanceEventSink** | Pluggable observability backend, no vendor coupling |
| **Trust Score Decay** | Configurable half-life: a trust score at deployment time is meaningless 6 months later |

---

## Upstream contributions

| Project | Contribution |
|---------|-------------|
| Google ADK | `AgentGovernancePlugin`: governance lifecycle hooks for the ADK agent runtime |
| Oracle Agent Spec | `ToolPolicy`, `ExecutionGuard`, `PolicyViolation` tracing additions |
| AAIF / LF AI & Data | Agent identity standards and governance interoperability |
| CoSAI WS4 | Agent governance working group |
| OWASP ASI | Agentic security integration (Top 10 for Agentic Applications) |
| OpenSSF | Scorecard improvements, supply chain security patterns |

---

## Integrations

<p align="center">
  <a href="https://github.com/langgenius/dify-plugins/pull/2060"><img src="https://img.shields.io/badge/Dify-65K_%E2%AD%90_Merged-success?style=for-the-badge" alt="Dify"></a>
  <a href="https://github.com/run-llama/llama_index/pull/20644"><img src="https://img.shields.io/badge/LlamaIndex-47K_%E2%AD%90_Merged-success?style=for-the-badge" alt="LlamaIndex"></a>
  <a href="https://github.com/github/awesome-copilot/pull/755"><img src="https://img.shields.io/badge/GitHub_Copilot-Merged-success?style=for-the-badge" alt="Copilot"></a>
  <a href="https://github.com/microsoft/agent-lightning/pull/478"><img src="https://img.shields.io/badge/Agent_Lightning-15K_%E2%AD%90_Merged-success?style=for-the-badge" alt="Agent-Lightning"></a>
</p>

## Featured in

<p align="center">
  <a href="https://github.com/Shubhamsaboo/awesome-llm-apps"><img src="https://img.shields.io/badge/awesome--llm--apps-92K_%E2%AD%90-orange?style=flat-square" alt="awesome-llm-apps"></a>
  <a href="https://github.com/Jenqyang/Awesome-AI-Agents/pull/45"><img src="https://img.shields.io/badge/Awesome--AI--Agents-listed-orange?style=flat-square" alt="Awesome-AI-Agents"></a>
  <a href="https://github.com/github/awesome-copilot/pull/755"><img src="https://img.shields.io/badge/awesome--copilot-listed-orange?style=flat-square" alt="awesome-copilot"></a>
  <a href="https://github.com/magsther/awesome-opentelemetry/pull/24"><img src="https://img.shields.io/badge/awesome--opentelemetry-listed-orange?style=flat-square" alt="awesome-opentelemetry"></a>
  <a href="https://github.com/TensorBlock/awesome-mcp-servers/pull/66"><img src="https://img.shields.io/badge/awesome--mcp--servers-listed-orange?style=flat-square" alt="awesome-mcp-servers"></a>
  <a href="https://github.com/rohitg00/awesome-devops-mcp-servers/pull/27"><img src="https://img.shields.io/badge/awesome--devops--mcp-listed-orange?style=flat-square" alt="awesome-devops-mcp"></a>
  <a href="https://github.com/heilcheng/awesome-agent-skills/pull/34"><img src="https://img.shields.io/badge/awesome--agent--skills-listed-orange?style=flat-square" alt="awesome-agent-skills"></a>
  <a href="https://github.com/MicrosoftDocs/community-content/pull/287"><img src="https://img.shields.io/badge/Microsoft_Community-Expert-purple?style=flat-square" alt="Microsoft Community Expert"></a>
</p>

---

<div align="center">

**[imransiddique.com](https://imransiddique.com)**

</div>