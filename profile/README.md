# Omotai

Open-source security tooling for AI agents that operate on the web.

Agents today control browsers built for humans: whatever the model decides to click, it clicks, and any text on any page can end up acting as an instruction. Omotai explores a different split: **the model proposes, a deterministic runtime decides**.

| Repository | What it is | Status |
| --- | --- | --- |
| [runtime](https://github.com/omotai/runtime) | MCP server that sits between an agent and the browser: policy engine, secret vault, network guard, human confirmation and tamper-evident audit log | Pre-alpha |
| [eval](https://github.com/omotai/eval) | Reproducible benchmark for web-agent security: mock sites, attack scenarios and a harness that compares any defense against a baseline | Pre-alpha |

Both projects are Apache-2.0 licensed. Contributions are welcome, especially **new attack scenarios** for the eval suite. See [CONTRIBUTING](https://github.com/omotai/.github/blob/main/CONTRIBUTING.md) and report vulnerabilities privately as described in [SECURITY](https://github.com/omotai/.github/blob/main/SECURITY.md).

## Status do Projeto (Setembro/2026)
- [x] **Planejamento e Modelo de Ameaças:** Concluído.
- [x] **Harness de Avaliação (`omotai/eval`):** Portal mock com 11 variantes de ataque.
- [x] **Runtime v0.1 (`omotai/runtime`):** Implementado com proxy MCP, política estrita de rede, injeção de sessão e ferramenta `back`.
- [x] **Validação de Utilidade:** Concluída com **Qwen 2.5 7B local** (80% de sucesso vs. 0% na baseline Playwright MCP, com 83% menos tokens).
- [ ] **Validação de Segurança:** Em andamento com `gpt-4o-mini` para medição da redução de 90% em injeções de prompt indiretas.
