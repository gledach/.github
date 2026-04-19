<div align="center">

```
            __          __           __
    ____ _ / /___  ____/ /___ ______/ /_
   / __ `// // _ \/ __  // __ `/ ___/ __ \
  / /_/ // //  __// /_/ // /_/ / /__/ / / /
  \__, //_/ \___/ \__,_/ \__,_/\___/_/ /_/
 /____/
```

<sub><em>gledati (slav.) — to watch. <br>
what a good analyst does before speaking.</em></sub>

<br>

![capercaillie + signal graph](https://raw.githubusercontent.com/gledach/.github/main/profile/avatar.jpg)

</div>

---

### live dashboard

```
╭───────────────────  competitive intelligence  ───────────────────╮
│                                                                   │
│   signal sources     ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓░░░░░  8 streams live    │
│   competitors        ▓▓▓▓▓▓▓▓▓▓▓▓░░░░░░░░░░░░  17 across voice-AI│
│   signals in turso   ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  1,398 & counting  │
│   llm spend / mo     ▓▓░░░░░░░░░░░░░░░░░░░░░░  ~$20              │
│   operators          ▓░░░░░░░░░░░░░░░░░░░░░░░  1                  │
│                                                                   │
│   > cat plans/*.md | grep -c READY                    11 shipped  │
│   > cat commits/main | grep -c verified               ✓ all       │
│                                                                   │
╰───────────────────────────────────────────────────────────────────╯
```

---

### 🔭 featured

**[cia](https://github.com/gledach/cia)** — *Competitive Intelligence Agent*

A single-operator CI platform for the voice-AI category. Tracks 17 competitors
across RSS, Algolia HN, YouTube transcripts, Tavily search, certificate-transparency
logs, sitemap + robots diffs, and Google Trends. Classifies with **Claude Haiku**,
synthesizes battlecards with **Claude Sonnet**, red-teams its own pipeline with
**Claude Opus**. Stores everything in **Turso** (hosted libSQL); serves a
Linear-style dashboard at `localhost:5180`. Built over weekends. Runs every
30 minutes. ~$20/mo.

```
 ┌─────────────────────┐    ┌────────────┐    ┌───────────────────┐
 │  ingest · 8 sources │───▶│   turso    │───▶│  battlecards +    │
 │  RSS · HN · YT      │    │  (libSQL)  │    │  Linear dashboard │
 │  certs · sitemaps   │    └─────┬──────┘    └───────────────────┘
 │  trends · Tavily    │          │
 └─────────────────────┘          ▼
                            ┌─────────────┐
                            │  analyst    │   /scan  /deep  /gap
                            │  (Opus 4.7) │   /outside  /brief
                            └─────────────┘
```

---

### 🛠 stack

```
 runtime  ·  Node.js (zero-dep bias) · Python where ML needs it
 ai       ·  Claude via OpenRouter  · Haiku · Sonnet · Opus  · BYOK
 data     ·  Turso · libSQL · SQLite · Markdown-in-git
 ux       ·  Linear-inspired dense dashboards · Playwright visual-regression
 shell    ·  bash + PowerShell (Windows, corporate-TLS hardened)
```

---

### 🧭 operating principles

> **local-first.** laptop is the runtime. cloud is for sharing state.<br>
> **single-operator.** no multi-tenancy until there's a second tenant.<br>
> **signal over polish.** output quality before dashboard aesthetics — but both.<br>
> **convergence over alerts.** one correlated insight > ten raw mentions.<br>
> **idempotent retry, not dual-write.** retry until it sticks; don't split sources of truth.

---

<div align="center">
<sub>
<a href="mailto:hi@aleksandarperisi.com">email</a>
&nbsp;·&nbsp;
<a href="https://github.com/gledach/cia">the agent</a>
&nbsp;·&nbsp;
<code>if it ships to turso, it shipped.</code>
</sub>
</div>
