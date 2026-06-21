---
name: investor-targeting
description: Build a tiered, stage- and sector-fit list of investors (VCs, angels, micro-funds, accelerators) for a founder's raise, using free public sources and live web search. Use when a founder asks "who should I raise from", "find investors for my startup", "which funds invest in <sector> at <stage>", or wants to build or qualify a fundraising target list. Never invents firms or partners — every name is researched live and carries a source link.
---

# Investor targeting

Help a founder build a **tiered target list** of investors that actually fit
their stage, sector, geography, and check size — grounded in live research, not
memory. A wrong or invented name wastes the founder's scarcest resource (warm
intros and credibility), so the prime directive is: **research, cite, flag —
never fabricate.**

Read `shared/references/outreach-ethics.md` before producing output.

## The hard rule on hallucination

You do **not** have a reliable investor database in your weights. Fund theses,
partner moves, check sizes, and "are they actively deploying" change constantly.
Therefore:

- **Do not name a specific firm, partner, or angel from memory as a
  recommendation.** Every name in the final list must come from a live
  `WebSearch` / `WebFetch` performed in this session.
- Each entry carries a **source link** and a **confidence flag**
  (`verified` / `likely` / `unverified — check`).
- If research is thin for a niche, say so. A short honest list beats a long
  fabricated one. It is correct to return "I found 6 strong fits; here are 4
  search angles to find more" rather than padding to 30.

## Step 1 — Profile the raise (ask before searching)

Collect these from the founder. If they're missing, ask; don't assume.

1. **One-liner**: what you do, for whom, the wedge.
2. **Stage & round**: pre-seed / seed / Series A; how much you're raising; how
   much is committed. (See `references/stage-map.md` for what each stage means
   for targeting.)
3. **Sector / category** + business model (B2B SaaS, consumer, deep tech,
   fintech, hardware, marketplace, AI infra, etc.). See
   `references/sector-taxonomy.md`.
4. **Geography**: where you're based, where you can take money from (some funds
   only invest in their region/jurisdiction).
5. **Traction**: the 1–2 metrics that make you fundable right now (revenue,
   growth, users, LOIs, a notable design partner). This drives *who* is a fit —
   a fund's check size must match your stage.
6. **Any constraints**: strategic investors to court or avoid, conflicts
   (competing portfolio cos), values requirements.

## Step 2 — Search across complementary angles

Don't rely on one query. Use several angles so you don't miss whole pockets.
See `references/free-data-sources.md` for the full source list. Core moves:

- **Thesis search**: `"<sector> <stage> investors"`, `"funds investing in
  <category> 2025"`, `"<sub-niche> seed funds"`.
- **Portfolio-analogy search**: find a few non-competing companies one notch
  ahead of you in the same category, then search **who funded their seed/A**.
  Their investors have proven appetite for your space. ("who invested in
  <company> seed round").
- **Operator-angel search**: search for angels who built or led in your
  category ("<category> angel investors", notable operators who now angel
  invest). Angels move faster and are often the first checks.
- **Accelerator search**: if pre-seed/idea stage, search accelerators/studios
  that focus on your sector or geography.
- **Directory search**: OpenVC, NFX Signal, the fund's own "submit a deal"
  page, recent SEC Form D filings, AngelList/Wellfound syndicates, relevant
  newsletters and "VC thesis" posts.

For each promising hit, `WebFetch` the firm/angel's own site to confirm:
stage focus, check size, sector, geography, and **how they want to be
contacted** (many list a submit form or a partner's preferred path).

## Step 3 — Qualify and tier

Score each candidate on fit, then sort into tiers:

- **Stage fit** — does their typical check match your round?
- **Sector fit** — explicit thesis or portfolio evidence in your space?
- **Geo/jurisdiction fit** — can they legally/practically invest in you?
- **No conflict** — not already backing a direct competitor.
- **Reachability** — is there a warm path or a clear public contact route?

Tier the output:

- **Tier A (high conviction, lead with these)** — strong on all five, clear
  contact path. Aim for a focused set you can deeply personalize.
- **Tier B (good fit, second wave)** — solid fit, weaker on one axis or no warm
  path yet.
- **Tier C (worth watching / opportunistic)** — plausible but unverified, or
  fit is partial.

## Step 3.5 — Sequence the outreach (don't burn your best leads first)

Recommend running outreach in waves: start with a few Tier B firms to pressure-
test the pitch and gather objections, refine, **then** approach Tier A with the
sharpened version and your best warm intros. Hand the Tier A targets to the
`warm-intro` and `cold-email` skills.

## Step 4 — Deliver

Output a table the founder can paste into a tracker (the `pipeline-tracker`
format if present), with columns:

| Firm / Angel | Tier | Why they fit | Stage & check | Contact path | Source | Confidence |
|---|---|---|---|---|---|---|

Then add:
- **Coverage note**: which angles you searched and which you didn't, so the
  founder knows what's *not* covered.
- **Next searches**: 3–5 concrete queries to extend the list themselves.
- **Verify-before-send reminder**: re-check each firm's current stage focus and
  contact preference right before reaching out — these go stale.

## Bilingual / China market (中文)

If the founder is raising in the **China market**, read
`shared/references/china-market-playbook.md` first. The free data sources differ
— use **IT桔子 / 企查查 / 天眼查 / 36氪 / 投资界** instead of Crunchbase to
verify a fund's deals and whether it's an RMB or state-backed fund (人民币/国资,
which changes its mandate and process). Same anti-hallucination rule: research
live, cite the source, never invent a 机构 name.

## Anti-patterns to refuse

- Producing a long list "from knowledge" without searching.
- Guessing partner email addresses.
- Recommending a fund whose stage clearly doesn't match (e.g., a growth fund
  for a pre-seed idea) just to lengthen the list.
- Dropping source links "to keep it clean." The links are the point.
