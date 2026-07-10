<div align="right">

**English** ｜ [繁體中文](README.zh-TW.md)

</div>

# 🔍 Competitor Sprint

> Give it one competitor, get a full intel report — **feature matrix + SWOT + market gaps + strategic recommendations** — in ~2 minutes, produced by **5 AI roles working in a pipeline**.
>
> Built for **founders / PMs / marketing freelancers**. No $10k/yr SaaS, no self-hosted Python stack — just paste a command. Reports come out in **your language** (defaults to Traditional Chinese; use `--lang en` for English), with first-class localization for Taiwan/Chinese sources (PTT / Dcard / 104).

![status](https://img.shields.io/badge/Claude_Code-Skill-blue) ![lang](https://img.shields.io/badge/繁中%20%2F%20EN-✓-green) ![license](https://img.shields.io/badge/License-MIT-yellow)

---

## Install (Claude Code)

```
/plugin marketplace add av8d-levelup/competitor-sprint
/plugin install competitor-sprint@competitor-sprint
```

## Usage

Two ways to invoke it after install:

**① Just tell Claude (recommended — auto-triggers)**
```
Run a competitor sprint on Notion, competitors: Coda, Obsidian, Craft
Analyze competitor: AI note-taking apps. My product is "MyNotes App". --lang en
```

**② As a command** (the full skill name is `competitor-sprint:competitor-sprint`)
```
/competitor-sprint:competitor-sprint Notion --competitors "Coda, Obsidian, Craft" --lang en
/competitor-sprint:competitor-sprint SaaS project management --competitors "Asana, monday, ClickUp" --hiring-signals
```

| Flag | What it does |
|---|---|
| `--competitors "A, B, C"` | Set the competitor list (omit → auto-discovers 4–6) |
| `--我方 "your product"` / `--me "your product"` | Add your own product to the feature matrix for a head-to-head |
| `--招聘信號` / `--hiring-signals` | Optional: adds a "hiring signals" section — infer a rival's next move from who they're hiring |
| `--lang en` | Optional: force English output (defaults to your input language) |

---

## Why it's different

- 🧑‍💼 **5-role pipeline**: Researcher → Analyst → Product → Strategist → Evaluator — a small intel team, not one prompt
- ✅ **Quality reflection loop**: the Evaluator scores 6 dimensions and auto re-searches if it scores below 7
- 🕵️ **Hiring signals** (optional): read a competitor's next strategic move from their job postings (104 / LinkedIn)
- 🗂️ **Markdown incremental fact-base**: one `db/<competitor>.md` per rival (YAML fields + changelog). Re-runs diff the old values and accumulate a timeline — plain text, git-versionable, so you can see exactly what a rival changed over the last 6 months
- 🌏 **Bilingual**: reports follow your input language (繁中 / English), with first-class Taiwan/Chinese source coverage
- ⏰ **Scheduled monitoring**: run weekly on a schedule and get pushed a change summary

## Example output

See [`examples/Notion競品/`](examples/Notion競品/):
- [`report.md`](examples/Notion競品/report.md) — full report (feature matrix / SWOT / market gaps / strategy)
- [`_index.md`](examples/Notion競品/_index.md) — a 4-way comparison overview
- [`db/`](examples/Notion競品/db/) — the structured fact-base

> There's also a local-business example, [`examples/台灣手搖飲品牌/`](examples/台灣手搖飲品牌/) (brick-and-mortar competitors; per-store Google reviews need the Places API).

---

## Who it's for

| ✅ Good fit | ❌ Not for |
|---|---|
| Founders / PMs doing PRDs & market analysis | Enterprise competitive-intel teams (need first-party traffic/ad data) |
| Marketing freelancers doing competitor briefs for pitches | — use Crayon / Similarweb for that |
| Indie devs scanning a space before building | |

**Positioning**: this is a *competitive sketch*, not an *intel platform*. Data comes from public web search — ideal for people with no intel budget who still need competitor insight.

---

## Want to skip the detours?

<div align="center">

Running one sprint is just the start — I show you how to wire AI into a full "ideate → produce → monetize" workflow.

### AV8D LevelUp｜Follow me, skip the detours

[![Facebook](https://img.shields.io/badge/Facebook-Follow%20AV8D%20LevelUp-1877F2?logo=facebook&logoColor=white)](https://www.facebook.com/AV8D.levelup)

**👉 https://www.facebook.com/AV8D.levelup**

</div>

---

## License

MIT © 2026 AV8D LevelUp. Commands and pricing referenced may change across versions — always check official docs.
