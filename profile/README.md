<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=recodeee&fontSize=80&fontColor=ffffff&fontAlignY=36&animation=fadeIn&desc=Tooling%20for%20people%20who%20run%20a%20lot%20of%20AI%20agents&descSize=18&descAlignY=58" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=2800&pause=900&color=70A5FD&center=true&vCenter=true&multiline=false&width=820&height=50&lines=Local-first+orchestration+for+fleets+of+coding+agents;Isolation+%E2%80%A2+locking+%E2%80%A2+observability+%E2%80%A2+handoffs;Open+source+%26+MIT-licensed.+Built+in+Slovakia+%F0%9F%87%B8%F0%9F%87%B0)](https://git.io/typing-svg)

[![Followers](https://img.shields.io/github/followers/recodeee?logo=github&style=for-the-badge&color=0891b2&labelColor=1c1917&label=followers)](https://github.com/recodeee)
[![Stars](https://img.shields.io/github/stars/recodeee?style=for-the-badge&logo=github&color=0891b2&labelColor=1c1917&label=org%20stars)](https://github.com/recodeee)
[![License](https://img.shields.io/badge/license-MIT-22c55e?style=for-the-badge&labelColor=1c1917)](https://opensource.org/licenses/MIT)
[![Slovakia](https://img.shields.io/badge/built%20in-Slovakia%20%F0%9F%87%B8%F0%9F%87%B0-7c3aed?style=for-the-badge&labelColor=1c1917)](https://github.com/recodeee)

</div>

---

## Why this org exists

Most "multi-agent" tools assume you're running two or three agents in parallel. We built these because we're running **thirty** — and the usual advice (be careful, use branches, review diffs) stops working around agent number five.

At that point you need actual infrastructure: **isolation, locking, orchestration, and a way to see what every agent is doing without opening thirty terminals.**

Everything in this org is open source and MIT-licensed.

---

## 🚀 Flagship Projects

<table>
  <tr>
    <td valign="top" width="33%">
      <h4>🛡️ <a href="https://github.com/recodeee/gitguardex">GitGuardex</a></h4>
      <p>Run many Codex &amp; Claude agents in parallel without them overwriting each other. Isolated worktrees, file locks, PR-only merges. Auto-wires Oh My Codex, Oh My Claude, OpenSpec, and Caveman into every worktree.</p>
      <p>
        <a href="https://guardextutorial.com/">Tutorial</a> ·
        <code>npm i -g @imdeadpool/guardex</code>
      </p>
      <p>
        <img alt="Stars" src="https://img.shields.io/github/stars/recodeee/gitguardex?style=flat-square&logo=github&color=0891b2&labelColor=1c1917">
        <img alt="Language" src="https://img.shields.io/github/languages/top/recodeee/gitguardex?style=flat-square&labelColor=1c1917">
      </p>
    </td>
    <td valign="top" width="33%">
      <h4>🐜 <a href="https://github.com/recodeee/colony">Colony</a></h4>
      <p>Local-first coordination substrate for fleets of coding agents. A SQLite store at <code>~/.colony</code> that holds claims, handoffs, plans, and memory — so Claude Code, Codex, Cursor, Gemini CLI, and OpenCode read a compact ~400-token state instead of replaying 30k-token repo handoffs.</p>
      <p>
        <img alt="Stars" src="https://img.shields.io/github/stars/recodeee/colony?style=flat-square&logo=github&color=0891b2&labelColor=1c1917">
        <img alt="Language" src="https://img.shields.io/github/languages/top/recodeee/colony?style=flat-square&labelColor=1c1917">
      </p>
    </td>
    <td valign="top" width="33%">
      <h4>🚁 <a href="https://github.com/recodeee/codex-fleetui">Codex FleetUI</a></h4>
      <p>Multi-account Codex worker pool with tmux dashboards, a force-claim dispatcher, and auto-rescue supervisors. Steer dozens of parallel Codex sessions from one terminal.</p>
      <p>
        <img alt="Stars" src="https://img.shields.io/github/stars/recodeee/codex-fleetui?style=flat-square&logo=github&color=0891b2&labelColor=1c1917">
        <img alt="Language" src="https://img.shields.io/github/languages/top/recodeee/codex-fleetui?style=flat-square&labelColor=1c1917">
      </p>
    </td>
  </tr>
  <tr>
    <td valign="top" width="33%">
      <h4>🔑 <a href="https://github.com/recodeee/authmux">authmux</a></h4>
      <p>Multi-identity helper for the Codex CLI. Auto-detects <code>codex login</code> and snapshots the account so you can list, switch, and rotate every account you've ever authed with one command.</p>
      <p>
        <code>npm i -g @imdeadpool/codex-account-switcher</code>
      </p>
      <p>
        <img alt="Stars" src="https://img.shields.io/github/stars/recodeee/authmux?style=flat-square&logo=github&color=0891b2&labelColor=1c1917">
        <img alt="Language" src="https://img.shields.io/github/languages/top/recodeee/authmux?style=flat-square&labelColor=1c1917">
      </p>
    </td>
    <td valign="top" width="33%">
      <h4>🧠 <a href="https://github.com/recodeee/claude-memory-manager-daemon">Claude Memory Manager</a></h4>
      <p>Long-running Claude Code agent that tends the file-based memory lane in a real-time tick loop — keeps user, feedback, project, and reference memories tidy and de-duplicated across sessions.</p>
      <p>
        <img alt="Stars" src="https://img.shields.io/github/stars/recodeee/claude-memory-manager-daemon?style=flat-square&logo=github&color=0891b2&labelColor=1c1917">
        <img alt="Language" src="https://img.shields.io/github/languages/top/recodeee/claude-memory-manager-daemon?style=flat-square&labelColor=1c1917">
      </p>
    </td>
    <td valign="top" width="33%">
      <h4>🧩 <a href="https://github.com/recodeee/claude-integrator">claude-integrator</a></h4>
      <p>Claude Code / Codex skill that scans <code>examples/</code> for vendored open-source repos, scores them on fit/cost/risk/value with license gates, and drafts OpenSpec integration proposals automatically.</p>
      <p>
        <img alt="Stars" src="https://img.shields.io/github/stars/recodeee/claude-integrator?style=flat-square&logo=github&color=0891b2&labelColor=1c1917">
        <img alt="Language" src="https://img.shields.io/github/languages/top/recodeee/claude-integrator?style=flat-square&labelColor=1c1917">
      </p>
    </td>
  </tr>
</table>

---

## 🛠️ Stack

<div align="center">

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![tmux](https://img.shields.io/badge/tmux-1BB91F?style=for-the-badge&logo=tmux&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Claude](https://img.shields.io/badge/Claude-d97706?style=for-the-badge&logo=anthropic&logoColor=white)
![Codex](https://img.shields.io/badge/Codex-111111?style=for-the-badge&logo=openai&logoColor=white)

</div>

---

## 🧪 What we're working on

```text
🪨 Recodee            Rust orchestrator for running dozens of coding agents — shipping soon
🤝 Handoffs           Smoother flows for when an agent hits its usage limit mid-task
🧩 OmX / OmC          Deeper integrations with Oh My Codex & Oh My Claude
🧠 Memory lanes       Cross-agent, file-based memory that survives session resets
📊 Observability      One pane of glass for every active agent, worktree, and account
```

---

## 📦 More from the org

<div align="center">

[`react-grab`](https://github.com/recodeee/react-grab) · [`oh-my-codex-colony`](https://github.com/recodeee/oh-my-codex-colony) · [`open-design`](https://github.com/recodeee/open-design) · [`copydesingskill`](https://github.com/recodeee/copydesingskill) · [`seomachine`](https://github.com/recodeee/seomachine) · [`medusa-plugins`](https://github.com/recodeee/medusa-plugins) · [`codex-plugins`](https://github.com/recodeee/codex-plugins)

</div>

---

## 📫 Contact & community

<div align="center">

[![Website](https://img.shields.io/badge/recodee.com-0A66C2?style=for-the-badge&logo=safari&logoColor=white)](https://recodee.com)
[![GitHub](https://img.shields.io/badge/recodeee-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/recodeee)
[![Email](https://img.shields.io/badge/nagy.viktordp%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:nagy.viktordp@gmail.com)

</div>

Issues and PRs welcome on any repo above — we read every one. If you're also building multi-agent tooling, **we'd love to compare notes**: open an issue on the most relevant project.

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&animation=twinkling"/>

*One must imagine a multi-agent system happy.*

**🪨 The boulder never stops.**

</div>
