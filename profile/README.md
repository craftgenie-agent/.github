# CraftGenie

Spring Boot agent that drives Claude Code to generate and refactor Java enterprise codebases, plus a deterministic library of **Domain Enhancement Patterns** (auditability, soft‑delete, multi‑tenancy, outbox, catch‑weight, …) that the agent applies to a JHipster JDL model with no LLM round‑trip.

## Repos

| Repo | What it is |
|---|---|
| [`craftgenie-parent`](https://github.com/craftgenie-agent/craftgenie-parent) | Top‑level driver scripts, test JDL fixtures, `bootstrap.sh`. Start here. |
| [`craftgenie-agent`](https://github.com/craftgenie-agent/craftgenie-agent) | Spring Boot service · pattern library · JDL parser · scaffold patcher. |
| [`craftgenie-sheets-sidecar`](https://github.com/craftgenie-agent/craftgenie-sheets-sidecar) | HMAC‑signed Google Sheets bridge. |
| [`craftgenie-ui`](https://github.com/craftgenie-agent/craftgenie-ui) | React/TS frontend that streams agent SSE. |

## Quick start

```bash
git clone git@github.com:craftgenie-agent/craftgenie-parent.git
cd craftgenie-parent
./bootstrap.sh
./pipeline.sh recipe-manager --reset --verify --with-agents
```
