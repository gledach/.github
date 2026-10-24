<div align="center">

# gledach

### Free tools that watch something public — and hand you the answer.

MIT licensed · runs on your machine · no account to start · each ships an audit of what it cannot see

**[▶ signal live demo](https://signal.gledach.de)** &nbsp;·&nbsp; **[browse the tools ↓](#the-tools)** &nbsp;·&nbsp; **[request one](https://github.com/gledach/requests)**

</div>

---

### the tools

Seven of twelve slots are filled.

| | Tool | Watches | Tells you |
|---|---|---|---|
| 01 | **[signal](https://github.com/gledach/signals)** | Thirteen public sources around whichever market you name | What changed, scored and attributed, over MCP |
| 02 | [signal-patterns](https://github.com/gledach/signal-patterns) | Nothing. It is the written reasoning | What is watchable, what it costs, how to build it |
| 03 | [whenrun](https://github.com/gledach/whenrun) | Day-ahead power prices and renewable share | The cheapest or greenest window, then starts the job in it |
| 04 | [phonehome](https://github.com/gledach/phonehome) | Every DNS query on your own network | Which device talked where, and when that changed |
| 05 | [recall](https://github.com/gledach/recall) | Four public registers, against a list of what you own | Which of your things has a notice, and how sure the match is |
| 06 | [talk](https://github.com/gledach/talk) | TCP connections from local coding agents, on Windows | Which API host each one reached, and whether the count is climbing |
| 07 | [snare](https://github.com/gledach/snare) | Hooks a coding agent runs at startup, and editor tasks that run when a folder opens | When that set changes. It does not delete a hook |
| 08 | `[UNNAMED]` | `[UNDECIDED]` | `[UNDECIDED]` |

Slot 08 is empty and stays written that way until something runs there. Is there
something you keep checking by hand that a tool could watch for you?
**[Ask for it in the open](https://github.com/gledach/requests).**

---

### why these exist

Same author, different shapes. They share no stack, no interface and no release cadence.
What they share is the promise: free, MIT licensed, installable, running on your own
machine, no account to start, and a written audit of what each one cannot see.

The command is `gledach-<tool>`. The shelf word stays the product name. `npm link`
inside a clone puts `gledach-whenrun`, `gledach-phonehome`, `gledach-recall`,
`gledach-talk` or `gledach-snare` on your PATH. Without a link, `node bin/<tool>.mjs` is the same program.
signal's package name is `gledach-signal` and its commands stay `npm run` inside the
clone. signal-patterns has no command. Nothing named `whenrun`, `phonehome`, `recall`,
`signal`, `signals`, `talk` or `snare` is installed. Those names already belong to other packages
or programs. The pages are on [gledach.de](https://gledach.de).

---

### signal, in focus

**[gledach/signals](https://github.com/gledach/signals)** · **[see it live](https://signal.gledach.de)**

*Track anyone. Compare anyone. On your own machine.*

Anyone means any company you name in one file. signal watches what they publish, scores
and attributes it, correlates it into convergences that several independent publishers
corroborate, and answers your agent over **MCP** rather than handing a person one more
dashboard to read. The dashboard is one client, not the product.

```
 ┌──────────────────────────┐   ┌────────────┐   ┌──────────────────────┐
 │  ingest                  │──▶│   turso    │──▶│  battlecards         │
 │  news · HN · reddit      │   │  (libSQL)  │   │  analyst briefs      │
 │  youtube · github        │   └─────┬──────┘   │  convergence alerts  │
 │  certs · sitemaps        │         │          └──────────────────────┘
 │  trends · search · email │         ▼
 └──────────────────────────┘   ┌───────────┐    ┌──────────────────────┐
                                │  analyst  │    │  MCP surface         │
                                │  /scan    │    │  8 tools, read only  │
                                │  /deep    │    │  until you say       │
                                │  /gap     │    │  otherwise           │
                                └───────────┘    └──────────────────────┘
```

**The unit that matters is a convergence, not a mention.** One correlated pattern that
several independent publishers corroborate, scored from its own evidence, with the rule
that fired it stated inline. Ten raw mentions of the same press release are one event.

```
 13       AI coding agents and app builders tracked, across two segments
 13       signal sources, from RSS to certificate transparency logs
 2,600+   signals in the deployment behind the live preview
 8        MCP tools, read only until you say otherwise
 3        runtime dependencies, no build step, clone and run offline
```

Clone it, run `npm run db:migrate`, and you have a populated dashboard with no account and
no API key. Point it at your own companies by editing one gitignored file.

---

### how it is built

```
 runtime  ·  Node 22, zero dependency bias. three runtime deps, no build step
 storage  ·  libSQL. a local file by default, hosted only when you want it shared
 ai       ·  bring your own key. without one, a keyword classifier and no briefs
 agents   ·  MCP over stdio. read only by default, spend ceiling shared with cron
 tests    ·  offline, against fixtures captured from the real sources
```

---

### operating principles

> **local first.** the laptop is the runtime. cloud is for sharing state between machines you own.<br>
> **convergence over alerts.** one correlated insight beats ten raw mentions.<br>
> **say what you cannot see.** every tool ships an honest audit of its own blind spots.<br>
> **read only until asked.** an agent does not spend your money because it found a button.<br>
> **generated text is labelled.** model output is marked as model output.<br>
> **idempotent retry, not dual write.** retry until it sticks. never split the source of truth.

---

<div align="center">

```
            __          __           __
    ____ _ / /___  ____/ /___ ______/ /_
   / __ `// // _ \/ __  // __ `/ ___/ __ \
  / /_/ // //  __// /_/ // /_/ / /__/ / / /
  \__, //_/ \___/ \__,_/ \__,_/\___/_/ /_/
 /____/
```

<sub><em>gledati (slav.): to watch. what a good analyst does before speaking.</em></sub>
<br><br>
<sub>
<a href="https://gledach.de">gledach.de</a>
&nbsp;·&nbsp;
<a href="https://signal.gledach.de">live demo</a>
&nbsp;·&nbsp;
<a href="https://github.com/gledach/requests">request a tool</a>
&nbsp;·&nbsp;
<a href="https://www.linkedin.com/company/gledach/">linkedin</a>
&nbsp;·&nbsp;
<code>if it ships to turso, it shipped.</code>
</sub>
</div>
