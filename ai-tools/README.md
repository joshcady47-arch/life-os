# AI Tools 🛠️

All AI-powered tools and apps built for the Cady family. Each folder is a self-contained project.

## Tools

| Folder | Status | Who It's For | What It Does |
|---|---|---|---|
| [`avery-bedtime-story/`](./avery-bedtime-story/) | 🔜 Build next | Avery (4) | Generates custom princess bedtime stories via Alexa |
| [`elias-minecraft-helper/`](./elias-minecraft-helper/) | 🔜 Planned | Elias (8) | Explains school concepts using Minecraft |
| [`family-dashboard/`](./family-dashboard/) | 🔜 Planned | Everyone | Shared family schedule + info display |
| [`job-hunt-tools/`](./job-hunt-tools/) | 🔜 Planned | Josh | Resume optimizer, application tracker, cover letter gen |
| [`household-automation/`](./household-automation/) | 🔜 Planned | Everyone | Alexa routines, meal planning, reminders |

## Stack

All tools run on:
- **Local inference**: Ollama `qwen3:4b` on Josh's MacBook (fast, private, no API costs)
- **Heavy inference**: `project-insight` Ollama API at `http://100.116.219.9:11434`
- **Python**: Conda base environment (xgboost, numpy, scipy installed)
- **Serving**: Simple Flask/FastAPI or static HTML — accessible on local network or Fire tablets

## Design Principles
1. **Works on Fire tablets** — simple HTML, no heavy JS frameworks
2. **Alexa-compatible where possible** — use Alexa routines + webhooks
3. **Kid-safe** — no scary content, always age-appropriate
4. **Offline-first** — local LLMs mean no internet dependency for family tools
5. **Fast** — responses in under 5 seconds for kids' tools
