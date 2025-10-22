
# AI Security & AI-for-Security Resources (Living List)

> **Note:** This living list combines two complementary perspectives:
> 1. **Securing AI (AI Security)** – protecting AI systems themselves.
> 2. **Applying AI to Cybersecurity (AI for Security)** – using AI/LLMs to secure or attack traditional IT systems.


---

## 1 Securing AI (AI Security)

### 1.1 Open-Source Tools for AI Red Teaming

**Predictive AI**
- [The Adversarial Robustness Toolbox (ART)](https://github.com/Trusted-AI/adversarial-robustness-toolbox)
- [Armory](https://github.com/twosixlabs/armory)
- [Foolbox](https://github.com/bethgelab/foolbox)
- [DeepSec](https://github.com/ryderling/DEEPSEC)
- [TextAttack](https://github.com/QData/TextAttack)

**Generative AI**
- [PyRIT](https://github.com/Azure/PyRIT)
- [Garak](https://github.com/NVIDIA/garak)
- [Prompt Fuzzer](https://github.com/prompt-security/ps-fuzz)
- [Guardrail](https://github.com/guardrails-ai/guardrails)
- [Promptfoo](https://github.com/promptfoo/promptfoo) - Open-source framework and CLI for testing and red-teaming prompts/agents with CI/CD-friendly automated evaluations.
- [PlexyGlass](https://github.com/safellama/plexiglass)
- [PurpleLlama](https://github.com/facebookresearch/PurpleLlama)
- [jailbreak-evaluation](https://github.com/controllability/jailbreak-evaluation)
- [Deepteam](https://github.com/confident-ai/deepteam)

### 1.2 Prompt Firewall & Redaction

_Products that intercept prompts and responses and apply security or privacy rules to them. We've blended two categories here because some prompt firewalls just redact private data (and then reidentify in the response) while others focus on identifying and blocking attacks like injection attacks or stopping data leaks. Many of the products in this category do all of the above, which is why they've been combined._

- [Cisco AI Defense](https://www.cisco.com/site/us/en/products/security/ai-defense/index.html) - Model Evaluation, monitoring, guardrails, inventory, AI asset discovery, and more. (Robust Intelligence AI Firewall is now part of Cisco.)
- [Protect AI Rebuff](https://playground.rebuff.ai) - A LLM prompt injection detector. [![code](https://img.shields.io/github/license/protectai/rebuff)](https://github.com/protectai/rebuff/)
- [Protect AI LLM Guard](https://protectai.com/llm-guard) - Suite of tools to protect LLM applications by helping you detect, redact, and sanitize LLM prompts and responses. [![code](https://img.shields.io/github/license/protectai/llm-guard)](https://github.com/protectai/llm-guard/)
- [HiddenLayer AI Detection and Response](https://hiddenlayer.com/aidr/) - Security for AI models and agents spanning supply-chain scanning, runtime defense, posture management, and automated red-teaming.
- [Vigil LLM](https://github.com/deadbits/vigil-llm) - Detect prompt injections, jailbreaks, and other potentially risky Large Language Model (LLM) inputs. ![code](https://img.shields.io/github/license/deadbits/vigil-llm)
- [Lakera Guard](https://www.lakera.ai/lakera-guard) - Protection from prompt injections, data loss, and toxic content.
- [Arthur Shield](https://www.arthur.ai/product/shield) - Built-in, real-time firewall protection against the biggest LLM risks.
- [Prompt Security](https://www.prompt.security) - SDK and proxy for protection against common prompt attacks.
- [Private AI](https://www.private-ai.com) - Detect, anonymize, and replace PII with less than half the error rate of alternatives.
- [DynamoGuard](https://dynamo.ai/platform/dynamoguard) - Identify / defend against any type of non-compliance as defined by your specific AI policies and catch attacks.
- [Skyflow LLM Privacy Vault](https://www.skyflow.com/product/llm-privacy-vault) - Redacts PII from prompts flowing to LLMs.
- [Guardrails AI](https://www.guardrailsai.com) - Guardrails runs Input/Output Guards in your application that detect, quantify and mitigate the presence of specific types of risks. [![code](https://img.shields.io/github/license/guardrails-ai/guardrails)](https://github.com/guardrails-ai/guardrails/)

### 1.3 LLM Observability Platforms/Tools

_Open-source & self-hostable tools that capture LLM requests and generations, surface traces, and provide dashboards for cost, latency, and other metrics. All offer a free hosted tier (with usage limits)._

- [**PostHog**](https://github.com/PostHog/posthog) – All-in-one product & LLM observability platform that unifies tracing, analytics, session replay, feature flags, and A/B testing. **MIT · ≈25.6 k★**
- [**Langfuse**](https://github.com/langfuse/langfuse) – Full-stack LLM engineering suite with call tracing, prompt management, evaluation pipelines, datasets, and OpenTelemetry-compatible metrics. **MIT · ≈10.2 k★**
- [**Opik**](https://github.com/comet-ml/opik) – Tracing, annotation, prompt/model playground, and evaluation for LLM apps; tightly integrated with Comet’s broader model-development workflow. **Apache 2.0 · ≈6.2 k★**
- [**OpenLLMetry**](https://github.com/traceloop/openllmetry) – OpenTelemetry-based collector/SDK for LLM requests, vector DBs, and agent frameworks; exports spans to Traceloop, Datadog, Honeycomb, and more. **Apache 2.0 · ≈5.6 k★**
- [**Phoenix**](https://github.com/Arize-ai/phoenix) – AI observability platform (by Arize) providing tracing, evals, experiments, and prompt management; ships plugins & conventions complementary to OpenTelemetry. **Elastic License 2.0 · ≈5.3 k★**
- [**Helicone**](https://github.com/helicone/helicone) – Monitoring, debugging, and prompt-improvement proxy with async mode, playground, eval scoring, and feedback capture for LLM applications. **Apache 2.0 · ≈3.6 k★**
- More platforms can be found [here](https://docs.litellm.ai/docs/integrations/)

### 1.4 AI Red Teaming Guidance & Datasets

**Guidance**
- [OWASP's GenAI Red Teaming Guide](https://genaisecurityproject.com/resource/genai-red-teaming-guide/) - guide includes four areas: model evaluation, implementation testing, infrastructure assessment, and runtime behavior analysis.
- [OWASP's List of AI Security Tools](https://owaspai.org/docs/5_testing/#open-source-tools-for-predictive-ai-red-teaming)
- [Guidance from the OWASP Generative AI Security Project](https://genai.owasp.org/initiatives/#ai-redteaming)
- [Guidance from CSA](https://cloudsecurityalliance.org/artifacts/agentic-ai-red-teaming-guide)

**Datasets**
- [AttaQ Dataset](https://huggingface.co/datasets/ibm/AttaQ) - a red teaming dataset consisting of 1402 carefully crafted adversarial questions
- [HarmBench: A Standardized Evaluation Framework for Automated Red Teaming and Robust Refusal](https://arxiv.org/pdf/2402.04249)

### 1.5 Commercial AI Security Platforms & Services

_Commercial and venture-backed platforms focused on securing AI systems, agents, and the surrounding ecosystem._

- **Astrix Security** – Non-human (machine) identity and AI agent access security: discover, govern, and enforce least-privilege with full audit trails. X: @AstrixSecurity · LinkedIn: Astrix Security · Blog · Crunchbase · CEO: Alon Jackson · CTO: Idan Gour.
- **Aurascape** – AI-native security layer delivering real-time visibility of AI use, intent-based controls, and guardrails for embedded and shadow AI. X: @aurascape_ai · LinkedIn: Aurascape · Blog · Crunchbase · CEO: Moinul Khan · CTO: Patrick Xu.
- **Citadel AI** – Model risk testing and governance with jailbreak tests, monitoring, and standards-aligned reporting to minimize safety, security, and compliance risk. X: @CitadelAI · LinkedIn: Citadel AI · Blog · GitHub · Crunchbase · CEO: Hironori Kobayashi · CTO: Kenny Song.
- **Clutch Security** – Universal non-human identity security that discovers, governs, and enforces zero-trust for API keys, service accounts, and agent credentials. LinkedIn: Clutch Security · Blog · GitHub · Crunchbase · CEO: Ofir Har-Chen · CTO: Sagi Haas.
- **Confident AI** – Built by the creators of DeepEval to help engineering teams benchmark, safeguard, and improve LLM applications with metrics and tracing. X: @confident_ai · LinkedIn: Confident AI (YC W25) · Blog · GitHub · Crunchbase · CEO: Jeffrey Ip · CTO: Kritin Vongthongsri.
- **Cranium** – Enterprise AI governance and security platform to inventory AI systems, test for vulnerabilities, manage risk, and attest compliance across first- and third-party AI. X: @CraniumAi · LinkedIn: Cranium · Blog · Crunchbase · CEO: Jonathan Dambrot · CISO: Byron Hawkins.
- **Deepchecks** – Evaluation and monitoring for LLM apps/agents to define metrics, run tests, and add safety checks for reliable AI delivery. X: @deepchecks · LinkedIn: Deepchecks · Blog · GitHub · Crunchbase · CEO: Philip Tannor · CTO: Shir Chorev.
- **Descope** – Agentic identity and authentication for AI apps/agents, managing lifecycle, authorization, and policy guardrails for agent identities. X: @descopeinc · LinkedIn: Descope · Blog · GitHub · Crunchbase · CEO: Slavik Markovich · CISO: Omer 🐈 Cohen.
- **Dream** – AI cyber defense for governments and critical infrastructure with real-time insight, predictive defense, and resilience. LinkedIn: Dream · Blog · Crunchbase · CEO: Shalev Hulio · CTO: Gil D.
- **Dreadnode** – Offensive AI security platform automating red-teaming and adversarial evaluation to uncover and exploit vulnerabilities in AI systems with operational tooling and training. X: @dreadnode · LinkedIn: Dreadnode · Blog · GitHub · Crunchbase · CEO: Will Pearce · CTO: Nick Landers.
- **Fiddler** – AI observability and guardrails platform to evaluate, explain, and monitor LLMs/agents in real time, reducing risk and improving reliability. X: @fiddler_ai · LinkedIn: Fiddler AI · Blog · GitHub · Crunchbase · CEO: Krishna Gade.
- **Giskard** – LLM security and testing offering continuous red-teaming to uncover jailbreaks, hallucinations, and safety flaws before and after deployment. X: @giskard_ai · LinkedIn: Giskard · Blog · GitHub · Crunchbase · CEO: Alex Combessie 🐢 · CTO: Matteo Dora.
- **Harmonic Security** – Data security for AI adoption with real-time visibility into AI usage, sensitive-data detection, and “human-like” protection and coaching. X: @harmonicsec · LinkedIn: Harmonic Security · Blog · Crunchbase · CEO: Alastair Paterson · CTO: Bryan Woolgar-O'Neil.
- **Irregular** – Frontier AI security lab that adversarially evaluates advanced models for misuse and builds defenses before release. X: @irregular · LinkedIn: Irregular (formerly Pattern Labs) · Publications · Crunchbase · CEO: Dan Lahav · CTO: Omer Nevo.
- **Knostic** – Enterprise AI security and compliance platform delivering need-to-know access controls and policy enforcement to prevent oversharing in copilots and LLMs. X: @knosticai · LinkedIn: Knostic · Blog · Crunchbase · CEO: Gadi Evron · CTO: Sounil Yu.
- **Lasso** – GenAI security platform that monitors AI use, detects risks in real time, and adds runtime defense/guardrails for applications, employees, and developers. X: @LassoSecurity · LinkedIn: Lasso · Blog · GitHub · Crunchbase · CEO: Elad Schulman · CTO: Lior Ziv.
- **Mindgard** – Automated AI red-teaming and runtime controls to map the AI attack surface, validate risk, and deliver AI detection and response. X: @MindgardAI · LinkedIn: Mindgard · Blog · GitHub · Crunchbase · CEO: James F. Brear.
- **Noma Security** – Agentic AI security platform to discover agent risks, monitor behavior, and enforce safeguards for safe large-scale adoption. X: @NomaSecurity · LinkedIn: Noma Security · Blog · Crunchbase · CEO: Niv Braun · CTO: Alon Tron · CISO: Diana Kelley.
- **Pillar Security** – LLM/agent security across the lifecycle with fingerprinting, inventory, automated red-teaming, and enforceable guardrails. X: @Pillar_sec · LinkedIn: Pillar Security · Blog · Crunchbase · CEO: Dor Sarig · CTO: Ziv Karliner.
- **Prime Security** – Design-stage security assistant automating design reviews and risk mitigation for engineering teams. Blog · LinkedIn: Prime Security · CEO: Michael N. · CTO: Danny H.
- **Protecto** – Privacy guardrails for GenAI to discover and mask PII/PHI while preserving context so AI apps remain useful and compliant. X: @ProtectoAI · LinkedIn: Protecto · Blog · GitHub · Crunchbase · CEO: Amar Kanagaraj · CTO: Baskaran Alagarsamy.
- **SPLX AI** – End-to-end AI security delivering scalable red-teaming, runtime threat detection/response, and automated governance and remediation. X: @SplxAI · LinkedIn: SPLX · Blog · GitHub · Crunchbase · CEO: Kristian Kamber · CTO: Ante Gojsalic · CISO: Sandy Dunn.
- **Straiker** – Agentic AI security to detect prompt injection, hallucinations, and rogue behaviors with red-teaming and guardrails for AI apps. X: @straikerai · LinkedIn: Straiker · Blog · Crunchbase · CEO: Ankur Shah · CTO: Sreenath Kurupati.
- **Theori** – AI-driven offensive testing with automated vulnerability discovery, LLM red-teaming, and guardrails; took 3rd place in DARPA’s AIxCC Finals at DEF CON 33. X: @theori_io · LinkedIn: Theori · Blog · GitHub · CEO: Brian Pak · CTO: Andrew Wesie.
- **TrojAI** – Secure-AI platform combining build-time model red-teaming with runtime protection to mitigate prompt attacks, data leaks, and unsafe outputs. X: @TrojAISec · LinkedIn: TrojAI · Blog · GitHub · Crunchbase · CEO: Lee Weiner · CTO: James Stewart, Ph.D.
- **WitnessAI** – Secure AI enablement platform offering visibility of AI use, policy controls, and sensitive data protection across the enterprise. LinkedIn: WitnessAI · Blog · Crunchbase · CEO: Rick Caccia · CTO: Gil Spencer.
- **XBOW** – AI-powered offensive security with autonomous agents that pentest apps at scale, discovering, validating, and exploiting real vulnerabilities with reproducible traces. X: @xbow · LinkedIn: XBOW · Blog · GitHub · Crunchbase · CEO: Oege de Moor.
- **Zenity** – AISPM and agent security platform to govern and secure AI agents with posture management, policies, and threat prevention across environments. X: @zenitysec · LinkedIn: Zenity · Blog · Crunchbase · CEO: Ben Kliger · CTO: Michael Bargury.

## 2 Applying AI to Cybersecurity (AI for Security)

### 2.1 Models

**Specialized Security Models**
- [Foundation-Sec-8B](https://huggingface.co/fdtn-ai/Foundation-Sec-8B) - Recent 8B parameter security-specialized model outperforming Llama 3.1 8B by +3.25% on CTI-MCQA and +8.83% on CTI-RCM, rivaling 70B models with 10x fewer parameters.
- [Llama-Primus-Base](https://huggingface.co/trendmicro-ailab/Llama-Primus-Base) - Foundation model with cybersecurity-specific pretraining on proprietary corpus.
- [Llama-Primus-Merged](https://huggingface.co/trendmicro-ailab/Llama-Primus-Merged) - Combined model through pretraining and instruction fine-tuning.
- [Llama-Primus-Reasoning](https://huggingface.co/trendmicro-ailab/Llama-Primus-Reasoning) - Reasoning-specialized model enhancing security certification through o1-distilled reasoning patterns.

### 2.2 Datasets

**Pre-Training Datasets**
- [Primus-FineWeb](https://huggingface.co/datasets/trendmicro-ailab/Primus-FineWeb) - Filtered cybersecurity corpus (2.57B tokens) derived from FineWeb using classifier-based selection.

**IFT & Capability Datasets**
- [Primus-Reasoning](https://huggingface.co/datasets/trendmicro-ailab/Primus-Reasoning) - Cybersecurity reasoning tasks with o1-generated reasoning steps and reflection processes.
- [Primus-Instruct](https://huggingface.co/datasets/trendmicro-ailab/Primus-Instruct) - Expert-curated cybersecurity scenario instructions with GPT-4o generated responses spanning diverse tasks.

### 2.3 Benchmarks & Evaluation

This section covers frameworks and methodologies for evaluating AI systems within security contexts.

**Vulnerability Assessment**
- [AutoPatchBench](https://engineering.fb.com/2025/04/29/ai-research/autopatchbench-benchmark-ai-powered-security-fixes/) - Benchmark for automated repair of fuzzing-detected vulnerabilities, pioneering evaluation standards.
- [SecLLMHolmes](https://github.com/ai4cloudops/SecLLMHolmes) - Automated framework for systematic LLM vulnerability detection evaluation across multiple dimensions.

**Threat Intelligence**
- [CTI-Bench](https://huggingface.co/datasets/AI4Sec/cti-bench) - Benchmark suite for evaluating LLMs on cyber threat intelligence tasks.
- [SECURE](https://github.com/aiforsec/SECURE) - Practical cybersecurity scenario dataset focusing on extraction, understanding, and reasoning capabilities.

**Offensive Security**
- [NYU CTF Bench](https://github.com/NYU-LLM-CTF/NYU_CTF_Bench) - Dockerized CTF challenges repository enabling automated LLM agent interaction across categories.

**General Security Knowledge**
- [CyberSecEval 4](https://meta-llama.github.io/PurpleLlama/CyberSecEval/docs/intro) - Comprehensive benchmark suite for assessing LLM cybersecurity vulnerabilities with multi-vendor evaluations.
- [SecBench](https://huggingface.co/datasets/secbench-hf/SecBench) - Largest comprehensive benchmark dataset distinguishing between knowledge and reasoning questions.
- [MMLU Computer Security](https://huggingface.co/datasets/cais/mmlu/viewer/computer_security?views%5B%5D=computer_security_test) - Standard benchmark with dedicated computer security evaluation subset for general LLMs.
- [MMLU Security Studies](https://huggingface.co/datasets/cais/mmlu/viewer/security_studies?views%5B%5D=security_studies_test) - General benchmark's security studies subset providing broader security knowledge assessment.

### 2.4 Publications

Academic and industry research on AI applications in security.

**Models & Datasets**
- [Foundation-Sec Technical Report](https://huggingface.co/fdtn-ai/Foundation-Sec-8B/blob/main/Technical_Report.pdf) - Detailed methodology for domain-adaptation of Llama-3.1 for cybersecurity applications.
- [Primus Paper](https://arxiv.org/abs/2502.11191) - First open-source cybersecurity dataset collection addressing critical pretraining corpus shortage.

**Benchmarking & Evaluations**
- [SecBench Paper](https://arxiv.org/abs/2412.20787) - Multi-dimensional benchmark dataset with unprecedented scale for LLM cybersecurity evaluation.
- [NYU CTF Bench Paper](https://arxiv.org/abs/2406.05590) - First scalable benchmark focusing on offensive security through CTF challenges.
- [SECURE Paper](https://arxiv.org/abs/2405.20441) - Industry-focused benchmark targeting Industrial Control System security knowledge evaluation.
- [CyberMetric Paper](https://arxiv.org/abs/2402.07688) - RAG-based cybersecurity benchmark with human-validated questions across diverse knowledge areas.
- [SecLLMHolmes Paper](https://arxiv.org/abs/2312.12575v3) - Comprehensive analysis revealing significant non-robustness in LLM vulnerability identification capabilities.
- [LLM Offensive Security Benchmarking](https://arxiv.org/abs/2504.10112v1) - Analysis of evaluation methodologies for LLM-driven offensive security tools with recommendations.

**Other**
- [OffsecML Playbook](https://wiki.offsecml.com) - Comprehensive collection of offensive and adversarial techniques with practical demonstrations.
- [MCP-Security-Checklist](https://github.com/slowmist/MCP-Security-Checklist) - Comprehensive security checklist for MCP-based AI tools by SlowMist.

### 2.5 Tools & Frameworks

**Adversarial ML**
- [DeepFool](https://github.com/lts4/deepfool) - Simple yet accurate method for generating adversarial examples against deep neural networks.
- [Counterfit](https://github.com/Azure/counterfit) - Automation layer for comprehensive ML system security assessment across multiple attack vectors.
- [Charcuterie](https://github.com/moohax/Charcuterie) - Collection of code execution techniques targeting ML libraries for security evaluation.

**Security Testing**
- [garak](https://github.com/leondz/garak/) - Specialized security probing tool designed specifically for LLM vulnerability assessment.
- [Snaike-MLFlow](https://github.com/protectai/Snaike-MLflow) - MLflow-focused red team toolsuite for attacking ML pipelines and infrastructure.
- [MCP-Scan](https://github.com/invariantlabs-ai/mcp-scan) - Security scanning tool specifically designed for Model Context Protocol servers.

**Learning Environments**
- [Malware Env for OpenAI Gym](https://github.com/endgameinc/gym-malware) - Reinforcement learning environment enabling malware manipulation for AV bypass learning.
- [Deep-pwning](https://github.com/cchio/deep-pwning) - Framework for assessing ML model robustness against adversarial attacks through systematic evaluation.

### 2.6 Security Agents

AI systems designed to perform security-related tasks with varying degrees of autonomy.

**Autonomous Agents**
- [HackingBuddyGPT](https://github.com/ipa-lab/hackingBuddyGPT) - Autonomous pentesting agent with corresponding benchmark dataset for standardized evaluation.
- [Agentic Radar](https://github.com/splx-ai/agentic-radar) - Open-source CLI security scanner for agentic workflows with automated detection.

**Red Team Agents**
- [HackGPT](https://github.com/NoDataFound/hackGPT) - LLM-powered tool designed specifically for offensive security and ethical hacking.
- [agentic_security](https://github.com/msoedov/agentic_security/) - LLM vulnerability scanner specializing in agentic systems and workflows.

### 2.7 Related Awesome Lists

Other collections and lists that may be of interest.

- [Awesome AI for Cybersecurity](https://github.com/Billy1900/Awesome-AI-for-cybersecurity) - Earlier comprehensive resource collection, focusing on pre-LLM machine learning applications.
- [Awesome ML for Cybersecurity](https://github.com/jivoi/awesome-ml-for-cybersecurity) - Established resource for traditional ML approaches in security, predating modern LLM era.
- [Awesome AI Security](https://github.com/ottosulin/awesome-ai-security) - Complementary list focusing on AI security rather than AI for security applications.
- [Awesome AI4DevSecOps](https://github.com/awsm-research/Awesome-AI4DevSecOps) - Recent integration of AI technologies within DevSecOps frameworks and methodologies.
- [Awesome-MCP-Security](https://github.com/Puliczek/awesome-mcp-security) - Definitive resource covering all aspects of Model Context Protocol security.
