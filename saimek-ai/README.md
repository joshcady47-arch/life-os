# Saimek AI Work 🤖

Josh's work with Greg's AI company, Saimek AI.

## Overview
Josh is getting up to speed on LLMs, machine learning, and AI infrastructure. His primary starting point is managing **TOWER** and all its services, then expanding into AI projects and prototypes.

## Folders

| Folder | Purpose |
|---|---|
| [`tower/`](./tower/) | TOWER server management — monitoring, docs, scripts |
| [`tower/monitoring/`](./tower/monitoring/) | Health check scripts, alerts, service status tools |
| [`tower/docs/`](./tower/docs/) | TOWER architecture, service configs, runbooks |
| [`tower/scripts/`](./tower/scripts/) | Utility scripts for managing TOWER remotely |
| [`projects/`](./projects/) | Active Saimek AI projects and prototypes |
| [`learning/`](./learning/) | Study notes specifically for Saimek AI topics |
| [`notes/`](./notes/) | Meeting notes, Greg's instructions, decisions |

## Infrastructure Reference

### TOWER (Media/Storage Server)
- **IP**: `100.73.185.39` (Tailscale) or alias `tower`
- **Role**: 100TB+ content storage — NOT a compute node
- **Services**: SABnzbd (8080), Sonarr (8989), Radarr (7878), Plex (32400)
- **OS**: TrueNAS SCALE (Linux)

### project-insight (AI Compute Server)
- **IP**: `100.116.219.9` (Tailscale) or alias `project-insight`
- **Role**: Heavy LLM inference — use this for anything over 8B parameters
- **Services**: Ollama API (11434) — DeepSeek-R1 32B, Qwen3 32B, Gemma4 26B
- **Hardware**: Mac Studio, 64GB Unified Memory

### Local MacBook (Josh's Machine)
- **Role**: Daily work, coding, light inference
- **Local LLM**: Ollama + qwen3:4b (2.5GB, fast, private)
- **Python**: Conda base — xgboost, numpy, scipy installed

## Connect to Servers
```bash
ssh tower           # TrueNAS SCALE media server
ssh project-insight # Mac Studio AI server
```
