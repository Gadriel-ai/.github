# Gadriel AI — The Complete AI Assurance Platform

[**Gadriel AI**](https://gadriel.ai) is the complete AI assurance platform covering the entire lifecycle of AI-assisted software development, autonomous agents, and production deployments across three integrated pillars:

1. **[Gadriel Code Assurance (GCA)](https://gadriel.ai/code-security)** — Local AI code security harness and MCP server (`@gadriel_ai/cli` / `gadriel`) that runs 6 deterministic security scanners on developer machines before AI-generated code or agent skills are committed.
2. **[Gadriel Behavior Assurance (GBA)](https://gadriel.ai/behavioral-assurance)** — Mathematical pre-production validation for autonomous AI agents, multi-agent workflows, and RAG pipelines.
3. **[Gadriel Deployment Assurance (GDA)](https://gadriel.ai/deployment-assurance)** — Continuous autonomous penetration testing and exploit validation for deployed applications, APIs, cloud infrastructure, and AI endpoints ([Order an Assessment](https://gadriel.ai/order-assessment)).

---

## 1. Gadriel Code Assurance (GCA) — Local AI Code Security Harness

AI coding agents write code fast—and introduce vulnerabilities just as fast. **[Gadriel Code Assurance](https://gadriel.ai/code-security)** integrates directly into your AI coding assistant as an MCP server, skill set, and pre-commit gate. Source code **never leaves your machine**.

### Six Local Security Scanners
- **SAST (`gadriel_sast_scan`):** Taint and pattern analysis across 30+ languages (SQLi, XSS, SSRF, command injection, path traversal, insecure deserialization, weak cryptography).
- **Secrets Detection (`gadriel_secrets_scan`):** High-entropy and structured credential detection across source files and git history.
- **SCA & SBOM (`gadriel_sca_scan`):** Dependency vulnerability scanning and CycloneDX / SPDX SBOM generation across 11 package ecosystems.
- **Container Security (`gadriel_container_scan`):** Dockerfile and container image vulnerability analysis.
- **IaC & Config (`gadriel_config_scan`):** Terraform, Kubernetes, CloudFormation, Helm, and CI/CD configuration hardening.
- **AI & Agentic Skills Security (`gadriel_ai_scan`):** OWASP LLM Top 10 and Agentic Skills Top 10 checks for prompt injection, tool poisoning, excessive agency, and unsafe MCP configurations.

### Quick Start

```bash
# Install the Gadriel CLI & MCP Server globally
npm install -g gadriel
# or via scoped package:
npm install -g @gadriel_ai/cli

# Start the local MCP server
npx -y gadriel code mcp
```

### Official IDE & Coding Agent Integrations
- **Claude Code:** [`Gadriel-ai/gadriel-claude-plugin`](https://github.com/Gadriel-ai/gadriel-claude-plugin)
- **Cursor:** [`Gadriel-ai/gadriel-cursor-plugin`](https://github.com/Gadriel-ai/gadriel-cursor-plugin)
- **GitHub Copilot:** [`Gadriel-ai/gadriel-copilot-plugin`](https://github.com/Gadriel-ai/gadriel-copilot-plugin) (Published on the Official MCP Registry as `io.github.Gadriel-ai/gadriel`)
- **OpenAI Codex CLI:** [`Gadriel-ai/gadriel-codex-plugin`](https://github.com/Gadriel-ai/gadriel-codex-plugin)
- **VS Code Extension:** [`Gadriel-ai/gadriel-vscode`](https://github.com/Gadriel-ai/gadriel-vscode) ([VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=GadrielAI.gadriel-security))

---

## 2. Benchmarks & Research

We benchmark Gadriel Code Assurance transparently against leading open-source and commercial scanners across multi-language vulnerable repositories ("6-Goat" SAST/SCA benchmark suite):

- [Gadriel vs. Semgrep — SAST & AI Code Security Benchmark](https://gadriel.ai/blog/gadriel-vs-semgrep.html)
- [Gadriel vs. Snyk — SAST, SCA & Secrets Benchmark](https://gadriel.ai/blog/gadriel-vs-snyk.html)
- [Gadriel vs. SonarQube — Static Analysis & Security Benchmark](https://gadriel.ai/blog/gadriel-vs-sonarqube.html)
- [Gadriel vs. Trivy — SCA, Container & Config Benchmark](https://gadriel.ai/blog/gadriel-vs-trivy.html)
- **Open Benchmark Repositories:**
  - [`Gadriel-ai/gadriel-vulnerable-cbom`](https://github.com/Gadriel-ai/gadriel-vulnerable-cbom) — Cryptographic Bill of Materials (CBOM) and post-quantum / weak-crypto test suite.
  - [`Gadriel-ai/gadriel-sca-test`](https://github.com/Gadriel-ai/gadriel-sca-test) — Multi-ecosystem SCA vulnerability test corpus across 11 package managers.

---

## 3. Documentation & Links

- **Platform Overview:** [https://gadriel.ai](https://gadriel.ai)
- **Gadriel Code Assurance:** [https://gadriel.ai/code-security](https://gadriel.ai/code-security)
- **Gadriel Behavior Assurance:** [https://gadriel.ai/behavioral-assurance](https://gadriel.ai/behavioral-assurance)
- **Gadriel Deployment Assurance:** [https://gadriel.ai/deployment-assurance](https://gadriel.ai/deployment-assurance)
- **Documentation Hub:** [https://gadriel.ai/docs](https://gadriel.ai/docs)
- **MCP Tools Reference:** [https://gadriel.ai/docs/gca/mcp-tools-reference.html](https://gadriel.ai/docs/gca/mcp-tools-reference.html)
- **Pricing & Plans:** [https://gadriel.ai/pricing](https://gadriel.ai/pricing)
