---
permalink: /research-interests/
title: "Research & Professional Interests"
author_profile: true
---

With the rapid proliferation of AI agents across science, business, and society — from coding assistants
and autonomous research tools to autonomous driving and financial automation — questions of reasoning,
tool use, and model behavior are becoming central not just to capability, but to safe deployment.
The same systems that unlock tremendous productivity gains also introduce novel attack surfaces:
information leakage through jailbreaks, selective disclosure failures, sleeper agent vulnerabilities,
and adversarial behaviors ranging from manipulation to
[deception and blackmail](https://www.anthropic.com/claude-4-system-card).
At the same time, with agents increasingly acting on behalf of humans, we face urgent questions
around identity, accountability, and [proof of humanship](https://www.identity.org/why-ai-agents-need-verified-digital-identities/).

Incorporating safety and security is not a constraint on AI progress — it is the enabler that makes
AI deployable in the environments where it matters most: safety-critical systems, regulated industries,
and scientific research. I wish to contribute to these challenges, with particular focus on reasoning,
AI safety and security, and the interface to cybersecurity and human–AI interaction.

## Areas of Expertise
- Generative AI, LLMs, and NLP
- Deep Learning
- Cybersecurity and Usable Security
- Human-Computer Interaction (HCI) and Human–AI Interaction (HAI)

## Research Interests
### AI Safety and (Cyber-)Security
As AI systems grow more capable and autonomous, ensuring their safe and robust behavior under
real-world conditions becomes critical. This encompasses both technical robustness and alignment
with user intent, values, and ethics — and has direct overlap with cybersecurity.
- **Alignment and model behavior analysis** — from controlled sandboxes to rich environments like
  [world models (Genie 3)](https://deepmind.google/blog/genie-3-a-new-frontier-for-world-models/)
- **Adversarial behaviors** — deception, manipulation, and [blackmail under pressure](https://www.anthropic.com/claude-4-system-card),
  as documented in the Claude 4 system card; broader [agentic misalignment](https://www.anthropic.com/research/agentic-misalignment)
- **Model steerability and ["sleeper agents"](https://arxiv.org/abs/2401.05566)** — models that behave
  safely under normal conditions but shift behavior when triggered, posing insider-threat-level risks
- **Selective information disclosure and jailbreaks** — how models can be prompted to bypass
  guardrails, including [secret exfiltration via coding agents](https://www.aikido.dev/blog/promptpwnd-github-actions-ai-agents)
  and prompt injection in CI/CD pipelines
  ([Black Hat USA 2025](https://i.blackhat.com/BH-USA-25/Presentations/US-25-Lynch-From-Prompts-to-Pwns.pdf))
- **Pre-deployment certification of trustworthiness and live monitoring** — behavioral and reasoning
  evaluation before and during deployment, including self- and third-party correction

### Agentic AI, Tool Use, and Reasoning
Agentic systems that call tools, write and execute code, browse the web, or interact with databases
represent a qualitative leap in capability — and in risk surface. Understanding and shaping their
behavior is one of the core challenges in current AI research.
- **Tool calling and reasoning correctness** — when should a model call an external tool vs. reason
  internally, and how do we verify it makes the right call?
- **(Neuro-symbolic) reasoning** — integrating symbolic methods and formal tools to increase
  reliability and interpretability of LLM reasoning
  ([Neurosymbolic LLM Reasoning, EMNLP 2025](https://aclanthology.org/2025.emnlp-main.1556.pdf))
- **Chain-of-Thought analysis** — faithfulness, robustness, and correctness of reasoning traces
  (see [my work on ToM reasoning evaluation](https://arxiv.org/abs/2410.06271))
- **Goal-directed reasoning and emergent misalignment** — how agentic reasoning toward objectives
  can give rise to instrumental behaviors such as deception, manipulation, or self-preservation,
  even without explicit instruction
  ([Agentic Misalignment](https://www.anthropic.com/research/agentic-misalignment),
  [Claude 4 System Card](https://www.anthropic.com/claude-4-system-card))
- **Advanced agentic architectures** — memory, retrieval-augmented generation (RAG), hybrid models,
  and multi-agent coordination

### Human–AI Interaction and Theory of Mind
Trustworthy AI is not only about what a model does in isolation — it is about how it interacts with
humans who have incomplete information, cognitive biases, and diverse mental models of the system.
- **Theory of Mind (ToM) in LLMs** — probing whether models can reliably attribute beliefs,
  knowledge, and intentions to others, and whether this scales robustly
  (see [my EMNLP 2024 paper](https://arxiv.org/abs/2410.06271))
- **Correct user modeling** — building AI systems that form accurate representations of user intent,
  knowledge state, and expectations
- **Anticipating human behaviors in relation to AI** — understanding how humans adapt, over-trust,
  or resist AI systems in strategic and everyday contexts (current research at RC-Trust / HUAM)
- **Usable security and HCI** — making security properties understandable and actionable for users;
  designing interfaces that do not create false impressions of safety
- **Proof of identity and humanship** — as agents proliferate, distinguishing human from AI
  actors becomes a fundamental challenge for trust, accountability, and digital identity
  ([AI agent identity verification](https://www.identity.org/why-ai-agents-need-verified-digital-identities/))

### Decentralized, Local, and Privacy-Preserving AI
Most production AI inference today runs on third-party cloud infrastructure — which creates
dependencies, potential conflicts of interest, and data sovereignty issues that are unacceptable
in many security-sensitive, regulated, or simply privacy-conscious settings.
- **On-premise LLM deployment** — running full inference pipelines locally, with no data leaving
  controlled infrastructure
- **Fine-tuning and adaptation** — reducing dependence on external model providers by training and
  adapting models to local demands and data
- **Privacy-preserving architectures** — GDPR-compliant, self-hosted stacks using tools like
  [Ollama](https://ollama.com/), [vLLM](https://github.com/vllm-project/vllm), and containerized
  inference (Docker / Kubernetes)
- **Space-based and distributed compute** — emerging infrastructures for resilient, independent AI
  deployments, including [SpaceX's planned orbital AI data center constellation](https://www.reuters.com/business/aerospace-defense/spacex-seeks-fcc-nod-solar-powered-satellite-data-centers-ai-2026-01-31/)
  and its [convergence with xAI](https://www.cnbc.com/2026/02/02/musks-xai-needs-spacex-for-money-data-centers-in-space-are-a-dream.html)

### Distributed Ledger Technology × AI
My earlier work on DLT, SSI, and smart contracts at Fraunhofer FIT laid a foundation that becomes
increasingly relevant as AI agents become first-class actors in digital systems.
- **Self-Sovereign Identity (SSI) for AI agents** — decentralized identity frameworks that allow
  agents and humans to establish accountability without central authorities
- **Smart contracts and AI** — with agents capable of executing complex tasks at high speed, their
  interaction with programmable on-chain logic is a natural and underexplored frontier
- **DLT as trust infrastructure** — using distributed ledgers to provide tamper-proof audit trails
  for AI-assisted decisions in regulated domains

## Key Research Questions
- How can we detect or increase model steerability — including model personality and values,
  detecting sleeper agents, and selective disclosure (for Theory of Mind or in production
  according to user access levels) and jailbreak resistance?
- How do we evaluate model behavior and reasoning, from simulation-based approaches to
  pre-deployment certification of trustworthiness and live monitoring during deployment?
- How do hybrid systems of human and AI agents behave under different incentives, information
  asymmetries, and personality configurations — and what behavioral patterns should we anticipate
  and design for? *(current: Social Agents and strategic interaction project)*
- How do we train, fine-tune, and host inference locally while preserving capability and security?