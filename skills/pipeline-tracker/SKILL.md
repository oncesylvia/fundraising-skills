---
name: pipeline-tracker
description: Run a fundraise like a sales pipeline — track every investor conversation, its stage, the next action, and follow-up timing in a simple file-based CRM. Use when a founder says "track my fundraising", "set up an investor CRM", "who do I need to follow up with", "update my pipeline", or wants to manage investor outreach and momentum. Produces and maintains a plain-text/CSV tracker, no SaaS required.
---

# Fundraising pipeline tracker

A raise is a sales process, and the founder is running it against time. Momentum
is everything: a tight, parallel process creates urgency; a slow, serial one
leaks energy and signals weakness. This skill sets up and maintains a **simple
file-based CRM** so nothing falls through and the founder always knows the next
action.

Read `shared/references/outreach-ethics.md` — follow-up discipline here must stay
on the right side of persistent-vs-pestering.

## Set it up (first run)

Create a tracker file in the user's project (default:
`fundraising-pipeline.csv`, or Markdown table if they prefer). Use the template
in `references/pipeline-template.md`. Columns:

| Field | What it holds |
|---|---|
| Investor | Firm or angel name |
| Partner | The specific person you're working |
| Tier | A / B / C (from `investor-targeting`) |
| Stage | Pipeline stage (see below) |
| Source | How you got in (warm intro via X / cold / inbound) |
| Last contact | Date of last touch |
| Next action | The single next thing *you* owe |
| Next action date | When to do it |
| Check / interest | Indicated check size or interest level |
| Notes | Anything said — objections, who they cc'd, asks |

## Pipeline stages

Keep it simple and linear; every investor sits in exactly one:

1. **Researched** — qualified as a fit, not yet contacted.
2. **Contacted** — first outreach sent (cold or intro requested).
3. **Engaged** — they replied / a call is booked.
4. **Met** — first meeting done.
5. **Diligence** — follow-up meetings, data room, partner meeting.
6. **Term sheet / Committed** — verbal or written commitment.
7. **Passed** — they said no (record *why* — it's signal).
8. **Dormant** — no response after the follow-up sequence ended.

## Running it (ongoing)

When the founder gives an update ("had a call with X", "Y passed", "Z asked for
the deck"), you:

1. **Update the row** — move the stage, set Last contact, write the Notes.
2. **Set the next action + date** — every *active* investor must have a next
   action owned by the founder. No row in stages 2–6 should have an empty next
   action.
3. **Surface what's due** — list who needs a follow-up today/this week, and draft
   it via the `cold-email` or `warm-intro` skill if asked.
4. **Watch the funnel** — report simple counts (e.g., 24 researched, 11
   contacted, 4 met, 1 in diligence) so the founder sees conversion and knows
   whether to add more top-of-funnel.

## Momentum coaching (the point of tracking)

- **Run in parallel, not serial.** Batch outreach so meetings cluster — multiple
  interested investors at once creates real (not fake) urgency and better terms.
- **Mind the follow-up cadence.** Persistent = two value-adding follow-ups, then
  stop (per the `cold-email` sequence). Pestering = more. The tracker enforces
  the gap, not just the nudge.
- **Log every pass and why.** Five passes for the same reason = a pitch or
  targeting problem to fix, not just bad luck.
- **Keep top-of-funnel full** until you have committed term sheets. A thin
  pipeline tempts founders to over-chase one lukewarm investor.

## Output

- On setup: the tracker file, created and explained.
- On update: confirm what changed, then a short **"due now / due this week"**
  action list and the current **funnel counts**.
- Never invent investor names or activity to fill the tracker — it holds only
  what the founder reports or what was researched (with sources) in
  `investor-targeting` / `investor-research`.
