# Omotai

Open-source security tooling for AI agents that operate on the web.

Agents today control browsers built for humans: whatever the model decides to click, it clicks, and any text on any page can end up acting as an instruction. Omotai explores a different split: **the model proposes, a deterministic runtime decides**.

| Repository | What it is | Status |
| --- | --- | --- |
| [runtime](https://github.com/omotai/runtime) | MCP server that sits between an agent and the browser: policy engine, secret vault, network guard, human confirmation and tamper-evident audit log | Pre-alpha |
| [eval](https://github.com/omotai/eval) | Reproducible benchmark for web-agent security: mock sites, attack scenarios and a harness that compares any defense against a baseline | Pre-alpha |

Both projects are Apache-2.0 licensed. Contributions are welcome, especially **new attack scenarios** for the eval suite. See [CONTRIBUTING](https://github.com/omotai/.github/blob/main/CONTRIBUTING.md) and report vulnerabilities privately as described in [SECURITY](https://github.com/omotai/.github/blob/main/SECURITY.md).
