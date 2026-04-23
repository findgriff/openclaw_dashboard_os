## OpenClaw Dashboard

A zero-dependency local command center for OpenClaw AI agents.

When you run OpenClaw at scale — multiple agents, cron jobs, sub-agents, channels, and models — it gets hard to see what is happening. This dashboard gives you one place to monitor gateway health, costs, cron activity, sessions, sub-agent runs, model usage, and recent git changes without digging through logs or CLI output.

It is not a replacement for the OpenClaw CLI or chat interfaces. It is the fast, at-a-glance layer that shows whether your system is healthy and where your compute and money are going.

### What it includes
- 12 dashboard panels for system health, costs, cron jobs, sessions, token usage, sub-agents, charts, models, skills, git log, and AI chat
- Live top metrics bar for CPU, RAM, swap, disk, OpenClaw version, and gateway status
- Smart alerts for high cost, failed crons, high context usage, and gateway readiness issues
- Built-in AI chat for natural-language questions about your dashboard
- 6 built-in themes plus support for custom themes
- Responsive UI for desktop, tablet, and mobile
- Pure HTML/CSS/JS frontend with a single Go backend binary
- Local-only operation with no cloud services or external frontend dependencies

### Highlights
- Instant stale-while-revalidate refresh via `/api/refresh`
- Auto-refresh every 60 seconds
- Cross-platform support for macOS and Linux
- Rate-limited AI chat endpoint
- Live runtime observability through `/api/system`
- Accurate per-session and sub-agent model resolution

### Quick start
Install with Homebrew:

```bash
brew install mudrii/tap/openclaw-dashboard
openclaw-dashboard --refresh
openclaw-dashboard
