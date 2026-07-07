<!-- SHIZAI — pixel workshop profile, v2: SVGs decorate, markdown informs. -->

<div align="center">

<img src="./assets/header.svg" width="100%" alt="SHIZAI — agent runtime reliability · Shenzhen. A pixel robot fixing bugs beside an orbiting pixel solar system." />

</div>

**I daily-drive AI coding agents and patch the layer where they break — streaming parsers, native forwarders, watchdogs, teardown paths.** Every quest below started as a crash I personally hit.

<img src="./assets/divider.svg" width="100%" alt="" />

## ⚔️ Quest Log

| Campaign | Battlefield | Loot |
|---|---|---|
| [**qwen-code**](https://github.com/QwenLM/qwen-code) | streaming tool-call parser | 🏅 **1 merged** — maintainer-verified E2E |
| [**omnigent**](https://github.com/omnigent-ai/omnigent) | harness runtime · kimi / qwen native forwarders | 🏅 **5 merged** · ⚔️ 8 in flight · 📜 12 issues filed |
| [**OpenHands SDK**](https://github.com/OpenHands/software-agent-sdk) | conversation & runtime internals | 🏅 **2 merged** |
| [**OpenHands**](https://github.com/OpenHands/OpenHands) | agent platform | 🏅 **1 merged** |
| [**open-design**](https://github.com/nexu-io/open-design) | daemon & run lifecycle | ⚔️ 6 in flight · ✅ 3 approved |

### 🏆 Recent boss drops

- 🐉 [**qwen-code #6250**](https://github.com/QwenLM/qwen-code/pull/6250) — *The Silent Tool-Call Eater.* The streaming parser swallowed no-argument tool calls whole, trapping llama.cpp-style providers in infinite retry loops. Root-caused in [#6249](https://github.com/QwenLM/qwen-code/issues/6249), survived four review rounds, maintainer-verified end-to-end. **Slain & merged.**
- 🗡️ [**omnigent #1677**](https://github.com/omnigent-ai/omnigent/pull/1677) — kimi-native now mirrors reasoning (think blocks) to the web transcript. **Merged.**
- 🗡️ [**omnigent #1834**](https://github.com/omnigent-ai/omnigent/pull/1834) — idle reaper re-checks liveness atomically with unregister; one release/reap race, deleted. **Merged.**
- 🧩 [**omnigent #1760**](https://github.com/omnigent-ai/omnigent/pull/1760) — new playable character: a `kimi-acp` harness driving `kimi acp` over ACP — MCP, images, resume, cancel, live steering. *Boss fight in progress.*

<img src="./assets/divider.svg" width="100%" alt="" />

## 🛠️ House Rules

1. **Daily-drive what you patch** — no tourist PRs; every fix comes from my own stack trace.
2. **Issue first, minimal diff** — the root-cause analysis lives in the issue; the PR stays surgical.
3. **Prove it twice** — layered repro before the fix, mutation A/B after it.
4. **One niche, dug deep** — the agent ↔ process boundary: parsers, forwarders, watchdogs, teardown.

<img src="./assets/divider.svg" width="100%" alt="" />

<div align="center">

<img src="./assets/pressstart.svg" width="480" alt="Press start — open an issue, let's collaborate." />

<sub>22.5429°N 114.0596°E · Shenzhen · UTC+8 — past the process boundary it's someone else's code; I build the layer that survives it.</sub>

</div>
