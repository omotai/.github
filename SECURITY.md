# Security policy

Omotai builds security tooling, so we take reports seriously and are grateful for them.

## Reporting a vulnerability

**Do not open a public issue.** Use GitHub's private vulnerability reporting instead:

1. Go to the **Security** tab of the affected repository.
2. Click **Report a vulnerability** and describe the issue, how to reproduce it and its impact.

We aim to acknowledge reports within **7 days** and to share a remediation plan within **30 days**. Fixes are published as GitHub Security Advisories, crediting the reporter unless they prefer otherwise.

## What counts as a vulnerability

In the runtime, anything that breaks a guarantee documented as **deterministic** in the threat model, for example:

- a secret value reaching the model's context or leaving to an origin it is not bound to;
- a request to a non-allowlisted origin that the network guard fails to block;
- an action requiring confirmation that executes without human approval;
- audit log tampering that goes undetected.

Attacks against guarantees documented as **partial / residual risk** are still valuable, but please submit them as attack scenarios to the [eval](https://github.com/omotai/eval) suite rather than as vulnerabilities.

## Supported versions

The projects are pre-alpha. Only the latest commit on `main` receives fixes.
