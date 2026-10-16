# Awesome-LLM-Observability

# Top LLM Observability Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Tracing, Evaluation & Production Monitoring for AI Applications*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **LLM Observability**. These tools provide tracing, debugging, evaluation, cost tracking, and production monitoring for LLM applications, RAG pipelines, and AI agents — enabling teams to understand what their AI systems are actually doing and why they fail.

**Examples** include Datadog LLMOps, LangSmith, Langfuse, Arize Phoenix, Helicone, WhyLabs, Fiddler AI, Braintrust, TruEra, and Arthur AI (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, OpenTelemetry-native instrumentation, and transparent evaluation — ideal for AI engineers, platform teams, and organizations building vendor-neutral LLM observability infrastructure.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Datadog LLMOps](https://www.datadoghq.com/)**  
  Extends Datadog's industry-leading APM platform to AI applications with end-to-end tracing from LLM calls to infrastructure metrics. Unified monitoring across traditional and AI workloads, prompt injection detection, and automatic cost estimation. **Caution**: Premium automatically activates at $120/day when LLM spans are detected with no opt-out .

- **[LangSmith](https://smith.langchain.com/)**  
  LangChain's observability, evaluation, and deployment platform — framework-agnostic with support for any LLM stack. Features detailed step-by-step tracing, real-time cost/latency monitoring, automatic conversation clustering for insight discovery, and self-hosting options for data-sensitive organizations. OTel support available .

- **[WhyLabs](https://whylabs.ai/)**  
  AI Control Center for observability, security, and optimization. Privacy-preserving telemetry works with 100% of data (no sampling) using open-source whylogs and LangKit. Features segment analysis for bias detection, anomaly feeds, and real-time guardrails for GenAI applications .

- **[Fiddler AI](https://www.fiddler.ai/)**  
  AI observability platform with ML and LLM monitoring. Features the LLM Enrichments Framework using proprietary Trust Models for high-accuracy scoring of faithfulness, answer relevance, toxicity, jailbreak, and PII metrics. OTel SDK provides framework-agnostic tracing with automatic LangChain, LangGraph, and Google ADK instrumentation .

- **[TruEra](https://truera.com/)**  
  LLM observability for evaluating, debugging, and monitoring applications at scale. Workflow spans experimentation (testing prompts, parameters, structures) through production monitoring with feedback functions for quality assessment .

- **[Arthur AI](https://www.arthur.ai/)**  
  Model and agent observability platform for monitoring, evaluating, and governing AI systems. Features agentic tracing with execution visualization, tool selection accuracy metrics, and governance policies with attestation workflows for regulated industries .

## Open-Source GitHub Projects

- **[Langfuse](https://github.com/langfuse/langfuse)**  
  **The most widely-adopted open-source LLM engineering platform** — 15,000+ GitHub stars, YC W23. Features observability, metrics, evals, prompt management, playground, and datasets. Integrates with OpenTelemetry, LangChain, LlamaIndex, OpenAI SDK, LiteLLM, and more. Self-hostable with no data leaving your infrastructure .

- **[Arize Phoenix](https://github.com/Arize-ai/phoenix)**  
  **Open-source AI observability for experimentation, evaluation, and troubleshooting** — 8,000+ stars. Built on OpenTelemetry with auto-instrumentation for LangChain, LlamaIndex, DSPy, Haystack, CrewAI, OpenAI, Anthropic, and 20+ frameworks. Features tracing, evaluation with LLM-as-judge, datasets, experiments, playground, and prompt management. Runs locally, in Jupyter, Docker, or Kubernetes .

- **[Helicone](https://github.com/Helicone/helicone)**  
  **Open-source LLM observability with built-in AI Gateway** — 4,300+ stars, YC W23. One-line integration for monitoring, metrics, evals, agent tracing, and prompt management. Features session tracking for multi-step agents, user-level cost attribution, automatic fallback chains (GPT-4o: OpenAI → Vertex → Bedrock), and prompt versioning with instant deployment. 0% markup on model routing compared to OpenRouter's 5.5% .

- **[TruLens](https://github.com/truera/trulens)**  
  **OpenTelemetry-native evaluation and tracing framework** — 2,800+ stars. Features RAG Triad metrics (groundedness, answer relevance, context relevance), agentic evaluators, and export to any OTLP backend (Jaeger, Grafana Tempo, Datadog). TruLens 2.13 adds Trends for time-series quality monitoring, run comparison with statistical significance testing, and offline BatchEvaluator .

- **[Opik (Comet ML)](https://github.com/comet-ml/opik)**  
  Open-source platform for debugging, evaluating, and monitoring LLM applications, RAG systems, and agentic workflows. Features comprehensive tracing, automated evaluations, and production-ready dashboards .

- **[Laminar](https://github.com/lmnr-ai/lmnr)**  
  Open-source all-in-one platform for engineering AI products with a data flywheel approach. Features traces, evals, datasets, and labels. YC S24 .

- **[OpenLIT](https://github.com/openlit/openlit)**  
  OpenTelemetry-native LLMOps platform with observability, evaluation, and guardrails. Supports 30+ LLM providers with one-line instrumentation .

- **[Agenta](https://github.com/Agenta-AI/agenta)**  
  Open-source LLMOps platform combining prompt playground, prompt management, LLM evaluation, and observability. 3,000+ stars .

- **[Radicalbit AI Monitoring](https://github.com/radicalbit/radicalbit-ai-monitoring)**  
  Comprehensive solution for monitoring AI models in production .

### Additional Strong Open-Source Options

- **[coze-loop](https://github.com/coze-dev/coze-loop)** — Next-generation AI Agent Optimization Platform with full-lifecycle management from development, debugging, and evaluation to monitoring .
- **[Palico AI](https://github.com/palico-ai/palico-ai)** — Build, improve performance, and productionize LLM applications with an integrated framework .
- **[llm-accounting](https://github.com/matdev83/llm-accounting)** — Python package for tracking and analyzing LLM usage across models and applications, designed for integration into agentic workflow tooling .
- **[MyScale Callback](https://github.com/myscale/myscale_callback)** — Integrates with LangChain Callbacks to capture trace data and store it in MyScale database .
- **[streamlit-chatbot-analytics](https://github.com/AndrMoura/streamlit-chatbot-analytics)** — Streamlit-based chatbot with PostHog-LLM logging and monitoring .

**Frameworks for building custom systems**: Combine **Langfuse** for end-to-end observability, **Phoenix** for OpenTelemetry-native tracing, **TruLens** for quality evaluation, and **Helicone** for gateway-level monitoring and fallback routing. For OTel-native stacks, emit **gen_ai.* semantic conventions** (semconv 1.30-1.32) and let vendor adapters translate — this makes migration between observability vendors trivial .

**Key architectural insight**: The **OpenTelemetry GenAI semantic conventions** (semconv 1.30-1.32) are the cross-vendor pivot for LLM observability. Datadog LLM Obs, New Relic AI Monitoring, Honeycomb, and Langfuse all ingest these natively as of late 2025. Emit OTel GenAI attributes in your SDK and map at the Collector — avoid vendor-proprietary tags for portability .

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- LLM observability tools capture sensitive prompt and completion data; ensure proper encryption, access controls, and compliance with GDPR/CCPA when self-hosting.
- **Pricing awareness**: Datadog LLM Observability automatically activates premium at $120/day when LLM spans are detected with no opt-out . Helicone offers 0% markup on gateway routing vs OpenRouter's 5.5% .
- Self-hosted solutions require infrastructure maintenance and regular security updates.

---

**Made for AI engineers, platform teams, MLOps practitioners, and observability enthusiasts.**  
Let's make LLM observability more open, transparent, and vendor-neutral.
