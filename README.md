# recodeee

**Tooling for people who run a lot of AI agents.**

Most "multi-agent" tools assume you're running two or three agents in parallel. We built these because we're running thirty — and the usual advice (be careful, use branches, review diffs) stops working around agent number five. At that point you need actual infrastructure: isolation, locking, orchestration, and a way to see what every agent is doing without opening thirty terminals.

Everything here is open source and MIT-licensed.

---

## Projects

### 🦖 [GitGuardex](https://github.com/recodeee/gitguardex)

Safety layer for parallel Codex/Claude agents in git repos. Each agent gets its own worktree, claims the files it's editing, and can't clobber files another agent has claimed. Auto-merges Oh My Codex, Oh My Claude, OpenSpec, and Caveman into every worktree so every agent starts tuned, not bare.

```sh
npm i -g @imdeadpool/guardex
```

Tutorial: [guardextutorial.com](https://guardextutorial.com/)

### 🔑 [codex-account-switcher](https://github.com/recodeecom/codex-account-switcher-cli)

Multi-identity Codex CLI. Auto-detects `codex login` and registers the account to a dashboard so you can see every account you've ever authed and switch with one command. Built because managing 30 agents across 30 accounts by hand is impossible.

```sh
npm i -g @imdeadpool/codex-account-switcher
```

### 🎨 [guardex-frontend](https://github.com/Webu-PRO/guardex-frontend)

Dashboard UI for GitGuardex. Shows every active agent, worktree status, file locks, account health, and live usage across all Codex accounts. Rust proxy + telemetry on the backend.

---

## What we're working on

- **Recodee** — orchestrator for running dozens of coding agents with a Rust runtime, shipping soon.
- Better handoff flows for when an agent hits its usage limit mid-task (currently the ugliest part of running at scale).
- More integrations with Oh My Codex / Oh My Claude so agents in Guardex worktrees start even smarter by default.

---

## Contact & community

Issues and PRs welcome on any of the repos above. We read every one.

If you're also building multi-agent tooling, we'd love to compare notes — open an issue or reach out on any of the project repos.
