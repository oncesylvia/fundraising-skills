# Fundraising Skills

A small, **honest** toolkit for founder-led fundraising, built as
[Claude Code](https://claude.com/claude-code) Skills.

Most fundraising advice fails founders at two points: **finding the right
investors** for their stage and sector, and **reaching out** without sounding
like spam. These skills help with both — and they're built to refuse the two
things that quietly wreck a raise: **hallucinated investor lists** and
**spray-and-pray outreach**.

> Built for the US / Silicon Valley fundraising playbook, but the frameworks
> work globally. All investor research is done **live, from free public
> sources** — no paid databases, no made-up names.

## The fundraising funnel → which skill helps

```
  ① Find the list          ② Reach out
 ┌──────────────────┐    ┌───────────────────────────┐
 │ investor-        │    │ warm-intro  (best path)    │
 │ targeting        │ →  │ cold-email  (no warm path) │
 └──────────────────┘    └───────────────────────────┘
   who fits my stage,       turn a fit into a
   sector, check size?      conversation
```

This is the **MVP** (v0.1). Targeting + the two outreach motions cover the
highest-pain part of a raise. More skills (research/diligence on a single
investor, pipeline/CRM tracking, pitch narrative, cold-call scripts) are planned.

## Skills

| Skill | Use it when… | What you get |
|---|---|---|
| **[investor-targeting](skills/investor-targeting/SKILL.md)** | "Who should I raise from?" | A tiered (A/B/C) target list, each with a fit reason, **source link**, and confidence flag — researched live, never invented |
| **[cold-email](skills/cold-email/SKILL.md)** | You have a fit but no warm path | A short, personalized email + 2 subject lines + a polite follow-up sequence |
| **[warm-intro](skills/warm-intro/SKILL.md)** | You have a mutual connection | A forwardable double opt-in intro, the no-pressure ask to your connector, and the etiquette to not burn the relationship |

A **warm intro beats the best cold email** — if a path exists, start there.

## Two principles baked into every skill

1. **No hallucinated investors.** The model does not recommend funds, partners,
   or angels from memory. Every name is found via live web search and carries a
   source link + a "verify before sending" flag. A short true list beats a long
   fake one.
2. **No spray-and-pray.** Every message is to one named person, grounded in
   something specific and true about them. Truthful traction only. See
   [shared/references/outreach-ethics.md](shared/references/outreach-ethics.md).

## Install

This repo is a Claude Code plugin marketplace. In Claude Code:

```
/plugin marketplace add your-handle/fundraising-skills
/plugin install fundraising-skills@fundraising-skills
```

Then just talk to Claude naturally — "help me find seed investors for my fintech
startup", "write a cold email to this VC", "my friend can intro me to <fund>" —
and the matching skill triggers.

> You can also clone the repo and copy any `skills/<name>/` folder into your
> project's `.claude/skills/` directory to use a single skill on its own.

## A typical flow

1. **Target** — `investor-targeting` builds your tiered list from a profile of
   your raise (stage, sector, geo, check size, traction).
2. **Warm up your pitch** — approach a few Tier-B firms first to collect
   objections and sharpen the story.
3. **Go warm where you can** — `warm-intro` for any investor you have a path to.
4. **Go cold where you can't** — `cold-email` for the rest, one personalized
   email at a time.
5. Repeat, keep notes, follow up twice, and stop gracefully.

## Status & contributing

v0.1 — MVP. Issues and PRs welcome, especially: localized variants (non-US
markets), more sector search recipes, and the planned skills above. Nothing here
is legal or financial advice; founders are responsible for their own outreach
and compliance.

## License

MIT. Use it, fork it, improve it, share it.
