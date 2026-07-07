# ShiZai(石在)· Agent Runtime Reliability

**I daily-drive AI coding agents and fix the layer where they break — streaming parsers, native forwarders, process lifecycle, teardown paths.**

Building agents at a Shenzhen AI startup. Everything below is patch work on tools I actually run every day.

---

## 📊 Track record

| Project | What I fix there | Record |
|---|---|---|
| [**qwen-code**](https://github.com/QwenLM/qwen-code) | streaming tool-call parser | **1 merged** — maintainer-verified E2E |
| [**omnigent**](https://github.com/omnigent-ai/omnigent) | harness runtime · kimi / qwen native forwarders | **5 merged · 8 in review · 12 issues filed** |
| [**OpenHands SDK**](https://github.com/OpenHands/software-agent-sdk) | conversation & runtime internals | **2 merged** |
| [**OpenHands**](https://github.com/OpenHands/OpenHands) | agent platform | **1 merged** |
| [**open-design**](https://github.com/nexu-io/open-design) | daemon & run lifecycle | **6 in review · 3 approved** |

### ⭐ Highlights

- [**qwen-code #6250**](https://github.com/QwenLM/qwen-code/pull/6250) — streaming parser silently dropped no-argument tool calls, breaking llama.cpp-style providers with infinite retry loops. Root-caused in [#6249](https://github.com/QwenLM/qwen-code/issues/6249), survived four review rounds, verified end-to-end by the maintainer. **Merged.**
- [**omnigent #1760**](https://github.com/omnigent-ai/omnigent/pull/1760) — new `kimi-acp` harness driving `kimi acp` over ACP: unlocks MCP, images, resume, cancel, and live steering. *In review.*
- [**omnigent #1677**](https://github.com/omnigent-ai/omnigent/pull/1677) — kimi-native forwarder now mirrors reasoning (think blocks) to the web transcript. **Merged.**
- [**omnigent #1834**](https://github.com/omnigent-ai/omnigent/pull/1834) — idle reaper re-checks liveness atomically with unregister, killing a release/reap race. **Merged.**

---

## 🔧 How I work

1. **Daily-drive what I patch** — every fix starts from a failure I personally hit.
2. **Issue first, minimal diff** — root-cause analysis lives in the issue; the PR stays surgical.
3. **Prove it twice** — layered repro before the fix, mutation A/B testing after it.
4. **One niche, dug deep** — agent ↔ process boundary: parsers, forwarders, watchdogs, teardown.

---

## 📍 Now

Shenzhen · UTC+8 · building out the Kimi harness story in omnigent

📫 Fastest way to reach me: open an issue on anything above.

<sub>Past the process boundary it's someone else's code — I build the layer that survives it.</sub>
