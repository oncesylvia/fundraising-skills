---
name: warm-path-finder
description: Find the right human at an investor (the partner / principal / senior investment manager who owns your deal) AND map the warm-connection paths to reach them. Use when a founder says "who at <firm> should I talk to", "how do I get a warm intro to <investor>", "find a connection to <fund>", "who can introduce me", or is stuck going from a target firm to an actual person and a path in. Works from the founder's own authorized data (Gmail, exported LinkedIn connections, contacts) + public sources — never scrapes private data or guesses personal emails.
---

# Warm path finder

Targeting tells a founder *which firms*. This skill closes the gap everyone gets
stuck on: **which specific human to reach, and who can warmly introduce them.**
It does two jobs:

1. **Pinpoint the person** — the partner / principal / senior investment manager
   who actually owns your sector and stage at the target firm (pitching the
   wrong person wastes the shot). See `references/finding-the-person.md`.
2. **Map & rank warm paths to that person** — surface every legitimate route
   from the founder's network, score by trust × reachability, and hand the best
   one to the `warm-intro` skill. See `references/connection-mapping.md`.

Read `shared/references/outreach-ethics.md` first. The whole skill lives or dies
on staying inside what's **authorized and public** (see the data-source tiers
below). Same anti-hallucination rule as the other research skills: a person or a
connection you assert must come from real data or live research, with a source —
never invent a partner, a title, or a mutual contact.

## The hard line on data (read this before doing anything)

| ✅ Allowed | ❌ Not allowed |
|---|---|
| The founder's **own authorized data**: their Gmail, their Google/phone contacts, a LinkedIn **connections export** *they* downloaded | Reading the founder's LinkedIn graph via API or scraping (no API exists; scraping breaks ToS and risks a ban) |
| **Public** info: X/Twitter bios, firm team pages, portfolio lists, podcasts, conference speakers, Crunchbase/AngelList people | Crawling login-walled content at scale |
| The founder **manually** checking shared connections / DM-open status while logged in | Guessing or buying personal email addresses to blast |

If a step would cross this line, stop and tell the founder.

## Step 1 — Pinpoint the right person

For a target firm, identify the specific decision-maker, not "the firm." See
`references/finding-the-person.md`. In short:

- Find the partner/principal who **leads your sector & stage** — via the firm's
  team page, who **led the round** for portfolio companies like yours (search
  "<analogous company> <round> <firm> partner"), their public thesis/posts.
- A **senior associate / principal / senior investment manager** who covers your
  space can be the better first target than a famous GP — they're more reachable
  and looking to source. Note who *sources* vs. who *decides*.
- Capture their **public footprint**: firm bio, LinkedIn URL, X handle, recent
  writing/podcasts. This is research input, not contact-harvesting.

## Step 2 — Search the founder's own authorized data first (Tier 1)

This is where the real warm paths hide, and it's 100% authorized. Ask the
founder which they can provide, then mine it. If they don't know how to get the
data, point them to `references/exporting-your-data.md` (step-by-step LinkedIn
export + Gmail/contacts, EN + 中文).

- **Gmail** (if connected): search their history for anyone already linked to the
  target firm or person — past threads, shared recipients, intros they've
  received. An existing thread *is* a warm path.
- **Exported LinkedIn connections CSV**: have the founder export it themselves
  (LinkedIn → Settings → Data Privacy → Get a copy of your data → Connections).
  Then cross-reference names/companies against the target firm and its portfolio.
- **Contacts**: Google/phone contacts for the same matching.

Match on: people *at* the firm, people who are *portfolio founders* of the firm
(highest-trust introducers), and people who share an employer/school with the
target person.

## Step 3 — Map public-network paths (Tier 2)

For paths not in the founder's own data, find them in the open:

- **Portfolio-founder paths** (best): a founder the firm already backed vouching
  for you is the strongest intro. Find portfolio cos near your space; the
  founder may know one, or know someone who does.
- **X/Twitter**: locate the firm's partners/managers, their public thesis, and
  whether they're reachable (open DMs / active repliers). The founder confirms
  DM-open status on the profile; you draft the message.
- **Shared communities**: accelerator alumni, university/employer networks,
  angel syndicates, founder Slacks/Discords, mutual advisors.
- **Events**: who from the firm is speaking where — a live intro beats a cold DM.

See `references/connection-mapping.md` for how to mine each surface.

## Step 4 — Score and rank the paths

For every path found, score it so the founder spends their best shots well.
Rank by **trust × reachability** (see the rubric in `connection-mapping.md`):

- **Trust**: how much does the target person trust the introducer? (portfolio
  founder > close peer/colleague > acquaintance > weak tie)
- **Reachability**: how easily can the founder actually ask this introducer, and
  how likely are they to say yes and follow through?

Output a ranked shortlist, not a dump. The **best connector is the one the target
actually replies to and who genuinely rates you** — not the most senior name.

## Step 5 — Hand off

- **If a warm path exists** → pass the top path + the named introducer to the
  **`warm-intro`** skill to write the ask + forwardable blurb.
- **If no warm path** → the strongest direct route (an open-DM partner who posts
  about your space, a firm's submit page) → hand to **`cold-email`** /
  **`cold-call`**, anchored on the specific person and their public thesis.
- Always note the **contact route + DM-open/submit status** you found, and a
  reminder to re-verify it right before reaching out.

## Output format

- **The person**: name, title, why them (sector/stage fit), public footprint,
  source links, confidence flag.
- **Ranked warm paths**: introducer → relationship → trust×reachability score →
  how the founder knows them (Tier 1/2 source).
- **Recommended next move**: the single best path, and which skill to use next.
- **Coverage note**: which data the founder did/didn't provide (e.g., "no
  LinkedIn export yet — here's how to get it and what it would unlock").

## Bilingual / China market (中文)

If the founder is raising in the **China market**, read
`shared/references/china-market-playbook.md` and use
`references/zh-talk-tracks.md`. LinkedIn is effectively gone in China and WeChat has no clean contact export, so
**do not** ask a China founder for a LinkedIn CSV. Instead have them fill the
**focused contact sheet** (`references/contact-sheet-template.csv`) from their
phone contacts export, CamCard/名片全能王 export, alumni rosters, and WeChat tags
— then mine that. Full how-to (中文) is in `references/exporting-your-data.md`.
Online paths: 脉脉 (Maimai), 微信好友/群, 校友圈; X applies only for 欧美 investors.

## Refuse / push back when

- Asked to scrape LinkedIn or read the connection graph via API — explain the
  authorized export route instead.
- Asked to guess or obtain personal emails to mass-contact — refuse; route to a
  warm path or a public submit form.
- Asked to assert a "mutual connection" that isn't backed by the founder's data
  or a real source — never fabricate a relationship.
