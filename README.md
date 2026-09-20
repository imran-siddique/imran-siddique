<div align="center">

# Imran Siddique

**Chief Platform Officer at [OPAQUE](https://opaque.co) | Creator of the [Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit)**

[![Website](https://img.shields.io/badge/imransiddique.com-blue?style=flat-square&logo=google-chrome&logoColor=white)](https://imransiddique.com)
[![AgenTrust](https://img.shields.io/badge/agentrust--io.com-0ea5e9?style=flat-square)](https://agentrust-io.com)
[![PyPI](https://img.shields.io/pypi/v/agent-governance-toolkit?style=flat-square&label=agent-governance-toolkit&logo=pypi&logoColor=white)](https://pypi.org/project/agent-governance-toolkit/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-imransiddique1986-0077B5?style=flat-square&logo=linkedin)](https://linkedin.com/in/imransiddique1986)
[![Sponsor](https://img.shields.io/badge/Sponsor-ff69b4?style=flat-square)](https://github.com/sponsors/imran-siddique)

</div>

---

18 years at Microsoft on core infrastructure: SQL Azure, Azure DevOps Code Search, Azure for
Industries, Microsoft Learn, and the Agent Governance Toolkit. Since June 2026 I have been Chief
Platform Officer at [OPAQUE](https://opaque.co), where I build AgenTrust: the open specifications
and runtimes that let an enterprise prove what an AI agent actually did.

My approach is **Scale by Subtraction**. The systems that survive are the ones where complexity was
removed rather than layered on top.

## The problem

Enterprises are giving agents real reach: email, CRMs, databases, financial systems. Most of the
industry has tried to solve this at the content layer, with guardrails that screen what goes in and
what comes out.

Guardrails help, and they leak. No filter reliably predicts a non-deterministic system. A single
piece of untrusted content, an email or a document or a support ticket, can carry hidden
instructions that redirect an agent into quietly exfiltrating internal data.

You do not run a regulated business on probably.

## What I build at OPAQUE

| Layer | What it does |
|-------|-------------|
| **Behavioral policy** | What an agent is allowed to do. The policy engine I built in AGT, now Cedar policy evaluated on every tool call |
| **Confidential computing** | Hardware-attested execution on SEV-SNP and TDX, where data does not leak even if the software above it is compromised |
| **Cryptographic proof** | A signed record of what ran, under which policy, touching which data, that a third party can check offline |

## AgenTrust: the open stack

Specifications and runtimes at [agentrust-io.com](https://agentrust-io.com). A live TDX quote
verifies in your browser at [agentrust-io.com/verify](https://agentrust-io.com/verify), and the
runnable set is at [agentrust-io.com/demos](https://agentrust-io.com/demos).

| Project | What it does | Where it is |
|---------|--------------|-------------|
| [**TRACE**](https://github.com/agentrust-io/trace-spec) | Portable signed runtime evidence: what ran, where, under which policy, touching which data, calling which tools, checkable offline by a third party | Spec v0.2. Hosted at the Linux Foundation as its own series, developed with AMD, Intel, Microsoft, OPAQUE and TII. Proposed to the Agentic AI Foundation sandbox as [aaif/project-proposals#42](https://github.com/aaif/project-proposals/issues/42) |
| [**Confidential MCP**](https://github.com/agentrust-io/cmcp) | A TEE-attested gateway that enforces Cedar policy on every MCP tool call and emits the TRACE record for it | v0.5.0, MIT |
| [**Agent Manifest**](https://github.com/agentrust-io/agent-manifest) | Hardware-anchors the 10 artifacts that define an agent at deployment: system prompt, policy bundle, tool schemas, model identity, RAG corpus, memory state, decision-log baseline, delegation chain, supply-chain provenance, approvals | Spec v0.2, Python SDK. In review as CoSAI WS4 issue #149 |
| [**Confidential A2A**](https://github.com/agentrust-io/ca2a) | Attested, attenuated agent-to-agent delegation and sealed peer channels as a profile on A2A, with an offline verifier and fail-closed SEV-SNP/TDX/TPM appraisal | v0.2.0 |
| [**Weight Custody Manifest**](https://github.com/agentrust-io/weight-custody-manifest) | Custody for model weights deployed into customer-controlled and sovereign infrastructure, with a published threat model and stated limits | v0.28.2, Apache-2.0, pre-1.0 |
| [**TRACE test suite**](https://github.com/agentrust-io/trace-tests) | Conformance tests, so TRACE support is something you run rather than something you assert | Public |

## Agent Governance Toolkit

The open-source governance layer for production AI agents, stewarded by Microsoft under MIT.

```
pip install "agent-governance-toolkit[full]"
```

```
+------------------------------------------------------------------+
|                    AGENT GOVERNANCE STACK                         |
+------------------------------------------------------------------+
|  AGENT HYPERVISOR  |  Runtime supervisor, Execution Rings (0-3)   |
|    (Runtime)       |  Joint Liability, Saga Orchestration         |
+--------------------+---------------------------------------------+
|  AGENT SRE         |  SLOs, chaos testing, canary deploys         |
|    (Reliability)   |  Incident response, runbook automation       |
+--------------------+---------------------------------------------+
|  AGENTMESH         |  Zero-trust identity, DID/SPIFFE, mTLS       |
|    (Trust)         |  A2A + MCP governance, behavioral scoring    |
+--------------------+---------------------------------------------+
|  AGENT OS          |  Policy enforcement kernel                   |
|    (Kernel)        |  Capability-based access, Merkle audit logs  |
+------------------------------------------------------------------+
```

10 formal specifications, 36 architecture decision records, SDKs for Python, .NET, TypeScript, Go
and Rust, and governance plugins for Claude Code, Copilot CLI and opencode.

[![Stars](https://img.shields.io/github/stars/microsoft/agent-governance-toolkit?style=flat-square&label=stars)](https://github.com/microsoft/agent-governance-toolkit/stargazers)
[![Forks](https://img.shields.io/github/forks/microsoft/agent-governance-toolkit?style=flat-square&label=forks)](https://github.com/microsoft/agent-governance-toolkit/network/members)
[![OWASP Agentic Top 10](https://img.shields.io/badge/OWASP_Agentic_Top_10-7_Full%2C_3_Partial-blue?style=flat-square)](https://github.com/microsoft/agent-governance-toolkit/blob/main/docs/compliance/owasp-agentic-top10-architecture.md)

That OWASP number is a self-assessment against the published mapping, not a third-party audit. The
three partials are agentic supply chain (ASI04), memory and context poisoning (ASI06), and
human-agent trust exploitation (ASI09). AGT does not establish compliance with anything. It
produces the evidence an auditor asks for.

### What makes this different

| Capability | How it works |
|------------|--------------|
| **Execution Rings** | CPU ring-inspired privilege isolation (Ring 0 to 3) for agent actions |
| **VADP** | Cryptographic delegation chains where each step narrows scope and never widens it |
| **AgentMesh Identity** | DID/SPIFFE-based durable cryptographic identity rather than ephemeral session tokens |
| **Decision BOM** | Reverse-traceable decision provenance over Merkle chains |
| **GovernanceEventSink** | Pluggable observability backend, no vendor coupling |
| **Trust Score Decay** | Configurable half-life, because a trust score from deployment day says nothing 6 months later |

## Writing

- **[Architecting at Scale](https://github.com/imran-siddique/Architecting-at-Scale)** (Packt). 16
  chapters in which each one solves the problem the previous chapter's solution created, following a
  single system, ShopFlow, from a monolith at 100 orders a day out to a globally distributed one.
  The companion repo carries the per-chapter code and all 73 Architect's Prompts.
- **Proof, Not Promises**, a weekly newsletter on LinkedIn. One project an edition, explained to the
  point where a reader could verify it.
- **[Notes](https://imransiddique.com)**, shorter and more frequent: a specific thing that broke, a
  spec line that does not hold, a fix that changed no behavior.
- **[awesome-ai-governance](https://github.com/agentrust-io/awesome-ai-governance)** and
  **[awesome-auditable-ai](https://github.com/imran-siddique/awesome-auditable-ai)**, curated
  reading for the same problem.

## Standards and working groups

| Body | What I work on |
|------|----------------|
| Linux Foundation | TRACE Specification, a Series of LF Projects, LLC |
| Agentic AI Foundation | Security and Privacy working group, and the TRACE sandbox proposal |
| CoSAI | WS1 software supply chain security, WS4 secure design for agentic systems |
| IETF SCITT | `draft-mih-scitt-agent-action-capsule`, `draft-mih-sokolov-scitt-payload-binding` |
| OWASP ASI | Agentic security integration, Top 10 for Agentic Applications |
| OpenSSF | Scorecard improvements, supply chain security patterns |
| Google ADK | `AgentGovernancePlugin`, governance lifecycle hooks for the ADK agent runtime |
| Oracle Agent Spec | `ToolPolicy`, `ExecutionGuard`, `PolicyViolation` tracing additions |

## Integrations

<p align="center">
  <a href="https://github.com/run-llama/llama_index/pull/20644"><img src="https://img.shields.io/badge/LlamaIndex-Merged-success?style=for-the-badge" alt="LlamaIndex"></a>
  <a href="https://github.com/github/awesome-copilot/pull/755"><img src="https://img.shields.io/badge/GitHub_Copilot-Merged-success?style=for-the-badge" alt="Copilot"></a>
  <a href="https://github.com/microsoft/agent-lightning/pull/478"><img src="https://img.shields.io/badge/Agent_Lightning-Merged-success?style=for-the-badge" alt="Agent-Lightning"></a>
  <a href="https://github.com/BrightbeamAI/chap"><img src="https://img.shields.io/badge/CHAP-TRACE_integration-success?style=for-the-badge" alt="CHAP"></a>
</p>

## Featured in

<p align="center">
  <a href="https://github.com/Shubhamsaboo/awesome-llm-apps/pull/467"><img src="https://img.shields.io/badge/awesome--llm--apps-listed-orange?style=flat-square" alt="awesome-llm-apps"></a>
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

**[imransiddique.com](https://imransiddique.com)** | **[agentrust-io.com](https://agentrust-io.com)**

</div>
