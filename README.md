# Imran Siddique

**Chief Platform Officer at [OPAQUE](https://opaque.co) · Creator of the [Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit)**

[Website](https://imransiddique.com) · [AgenTrust](https://agentrust-io.com) · [LinkedIn](https://linkedin.com/in/imransiddique1986) · [Sponsor](https://github.com/sponsors/imran-siddique)

I build confidential AI infrastructure and verifiable agent systems. Before OPAQUE, I spent
18 years at Microsoft working on cloud, developer, and AI platforms.

My approach is **Scale by Subtraction**: remove unnecessary complexity, put policy checks on the
action path, and make claims testable by someone outside the system that produced them.

## Current work

At OPAQUE, my work connects three layers:

| Layer | What it provides |
|---|---|
| Behavioral policy | Explicit rules for tool calls and delegated authority, enforced outside the model's reasoning |
| Confidential computing | Workload isolation and attestation within a stated platform threat model |
| Runtime evidence | Signed records that bind claims to a signer, with independently verified evidence needed to establish those claims |

Hardware attestation does not establish policy correctness or eliminate side channels. A valid
record signature establishes integrity and signer identity; it does not, by itself, prove the
recorded action happened.

## AgenTrust: the open stack

[Documentation](https://agentrust-io.com) · [Verification demo](https://agentrust-io.com/verify) · [Runnable demos](https://agentrust-io.com/demos)

| Project | Purpose | Status and source |
|---|---|---|
| [TRACE](https://github.com/agentrust-io/trace-spec) | Portable signed records of agent runs, with a specification and verification rules | Spec v0.2; [hosted at the Linux Foundation](https://www.linuxfoundation.org/press/linux-foundation-welcomes-trace-to-advance-verifiable-runtime-evidence-for-ai-workloads). [AAIF sandbox proposal](https://github.com/aaif/project-proposals/issues/42) remains open |
| [cMCP](https://github.com/agentrust-io/cmcp) | MCP gateway that evaluates Cedar policy on tool calls and emits TRACE evidence | [Releases](https://github.com/agentrust-io/cmcp/releases/latest); [gateway and attestation limits](https://github.com/agentrust-io/cmcp/blob/main/LIMITATIONS.md) |
| [Agent Manifest](https://github.com/agentrust-io/agent-manifest) | Signed deployment manifests covering prompts, policy, tools, model identity, and other agent artifacts | Spec v0.2, Python and TypeScript SDKs; [CoSAI WS4 RFC](https://github.com/cosai-oasis/ws4-secure-design-agentic-systems/issues/149) remains open |
| [cA2A](https://github.com/agentrust-io/ca2a) | Attenuated delegation, peer appraisal, and provenance as a profile on A2A | [Releases](https://github.com/agentrust-io/ca2a/releases/latest); [developer-preview limits](https://github.com/agentrust-io/ca2a/blob/main/LIMITATIONS.md) |
| [Weight Custody Manifest](https://github.com/agentrust-io/weight-custody-manifest) | A protocol for conditional model-weight release and custody evidence | Pre-1.0 [public review](https://github.com/agentrust-io/weight-custody-manifest); [key-service, platform, and hardware-owner limits](https://github.com/agentrust-io/weight-custody-manifest/blob/main/LIMITATIONS.md) |
| [TRACE test suite](https://github.com/agentrust-io/trace-tests) | Executable conformance checks for TRACE records | Public suite; results apply to the properties tested |

## Agent Governance Toolkit

[AGT](https://github.com/microsoft/agent-governance-toolkit) is the open-source agent governance
project I created, hosted by Microsoft under MIT. It brings together policy enforcement,
agent identity and trust, runtime supervision, and reliability controls.

```bash
pip install "agent-governance-toolkit[full]"
```

The repository includes Python, .NET, TypeScript, Go, and Rust SDKs, plus governance integrations
for coding agents. See its [documentation](https://github.com/microsoft/agent-governance-toolkit#readme)
for current packages, installation paths, and supported integrations.

[![Stars](https://img.shields.io/github/stars/microsoft/agent-governance-toolkit?style=flat-square)](https://github.com/microsoft/agent-governance-toolkit)

The published [OWASP Agentic Top 10 mapping](https://github.com/microsoft/agent-governance-toolkit/blob/main/docs/compliance/owasp-agentic-top10-architecture.md)
self-assesses seven categories as full and three as partial: supply chain, memory/context
poisoning, and human-agent trust exploitation. This is a project mapping, not an independent
audit or compliance certification. Deployment-specific controls still matter.

## Book, patterns, and writing

- **[Architecting at Scale](https://www.packtpub.com/en-in/product/architecting-at-scale-9781807420963)**,
  published by Packt. Follow ShopFlow from a monolith to a distributed system across 16 technical
  chapters. The [companion repository](https://github.com/imran-siddique/Architecting-at-Scale)
  contains the code, chapter notes, and 73 Architect's Prompts.
- **[Agentic Architecture](https://github.com/imran-siddique/agentic-architecture)**: four patterns
  for routing, grounded context, constrained execution, and evidence, with executable checks
  and explicit limits.
- **Proof, Not Promises**, my LinkedIn newsletter on verifiable claims in AI systems.
- **[Notes](https://imransiddique.com)** on implementation findings, specification gaps, and fixes.
- **[awesome-ai-governance](https://github.com/agentrust-io/awesome-ai-governance)** and
  **[awesome-auditable-ai](https://github.com/imran-siddique/awesome-auditable-ai)**: curated reading.

## Standards and upstream work

My standards work includes TRACE at the Linux Foundation, the AAIF sandbox proposal, CoSAI
software supply chain and agentic-system design discussions, OWASP agentic security, and OpenSSF
supply chain practices. An open proposal is not an adopted standard.

Selected merged contributions:

- [LlamaIndex](https://github.com/run-llama/llama_index/pull/20644): AgentMesh trust-layer integration.
- [GitHub Copilot](https://github.com/github/awesome-copilot/pull/755): agent-governance skill.
- [Agent Lightning](https://github.com/microsoft/agent-lightning/pull/478): Agent OS integration for training governance.

<!-- Profile claims and linked project status reviewed 2026-09-25. Release links intentionally replace static runtime version numbers. -->
