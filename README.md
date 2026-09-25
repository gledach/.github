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

<sub><em>This repo holds the organisation profile. The rendered version is at
<a href="https://github.com/gledach">github.com/gledach</a> — edit
<code>profile/README.md</code>, not this file, and keep the two in step.</em></sub>

---

### what this is

Tools that turn **public noise into structured signal** — and hand it to an agent
rather than to a dashboard nobody opens.

The pattern is the same every time: watch a set of sources continuously, score and
attribute what comes back, notice when several independent sources say the same thing,
and expose the result as data something else can query. Competitors are the first
subject. They are not the only one that shape fits.

---

### 🔭 signal — our first public repo

**[gledach/signals](https://github.com/gledach/signals)** · **[see it live →](https://signal-v1.gledach.de)**

*Competitive intelligence your agents can query.*

Watches a market, turns public noise into scored and attributed signals, exposes them
over **MCP** — eight tools and `signal://` resources, so Claude Code or any MCP client
can ask "what changed at the tools we track this week?" and get structured data back.
The dashboard is one client, not the product.

```
 ┌──────────────────────────┐   ┌────────────┐   ┌──────────────────────┐
 │  ingest                  │──▶│   turso    │──▶│  battlecards         │
 │  news · HN · reddit      │   │  (libSQL)  │   │  analyst briefs      │
 │  youtube · github        │   └─────┬──────┘   │  convergence alerts  │
 │  certs · sitemaps        │         │          └──────────────────────┘
 │  trends · search · email │         ▼
 └──────────────────────────┘   ┌───────────┐    ┌──────────────────────┐
                                │  analyst  │    │  MCP surface         │
                                │  /scan    │    │  8 tools · 30 res.   │
                                │  /deep    │    │  read-only by        │
                                │  /gap     │    │  default             │
                                └───────────┘    └──────────────────────┘
```

**The unit that matters is a convergence** — not a mention. One correlated pattern that
several independent publishers corroborate, scored from its own evidence, with the rule
that fired it stated inline. Ten raw mentions of the same press release are one event.

```
 13       AI coding agents + app builders tracked, across two segments
 13       signal sources, from RSS to certificate-transparency logs
 2,600+   signals in turso
 8        MCP tools · read-only until you say otherwise
 3        runtime dependencies · no build step · clone and run offline
```

Clone it, run `npm run db:migrate`, and you get a populated dashboard with no account
and no API key. Point it at your own market by editing one gitignored file.

---

### 🛠 how it is built

```
 runtime  ·  Node.js, zero-dep bias — three runtime dependencies, no build step
 ai       ·  Claude via OpenRouter · Haiku triage · Sonnet synthesis · Opus depth · BYOK
 data     ·  Turso · libSQL · SQLite · markdown-in-git
 agents   ·  MCP over stdio · read-only by default · spend ceiling shared with cron
 ux       ·  dense, Linear-inspired dashboards · Playwright visual checks
```

---

### 🧭 operating principles

> **local-first.** the laptop is the runtime. cloud is for sharing state.<br>
> **convergence over alerts.** one correlated insight beats ten raw mentions.<br>
> **signal over polish.** output quality before dashboard aesthetics — but both.<br>
> **say what you cannot see.** every tool ships an honest audit of its own blind spots.<br>
> **read-only until asked.** an agent does not spend your money because it found a button.<br>
> **idempotent retry, not dual-write.** retry until it sticks; never split the source of truth.

---

<div align="center">
<sub>
<a href="https://github.com/gledach/signals">signal</a>
&nbsp;·&nbsp;
<a href="https://signal-v1.gledach.de">live demo</a>
&nbsp;·&nbsp;
<a href="mailto:hi@aleksandarperisic.com">email</a>
&nbsp;·&nbsp;
<code>if it ships to turso, it shipped.</code>
</sub>
</div>
