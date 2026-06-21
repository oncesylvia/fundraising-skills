# Pipeline tracker templates

Two ready-to-use formats. Pick one and create it in the founder's project.

## CSV (good for spreadsheets / import)

Save as `fundraising-pipeline.csv`:

```csv
Investor,Partner,Tier,Stage,Source,Last contact,Next action,Next action date,Check/Interest,Notes
Acme Ventures,Jane Doe,A,Engaged,Intro via Sam,2026-06-18,Send deck + data room,2026-06-22,Lead ~$1.5M,"Liked the wedge; wants retention cohort data"
Beta Capital,John Roe,B,Contacted,Cold email,2026-06-17,Follow-up #1 (add new MRR),2026-06-23,Unknown,"No reply yet"
Angel: Lee Wong,—,A,Met,Intro via founder of Porta,2026-06-15,Send SAFE terms,2026-06-21,$50–100K,"In; wants to fill not lead"
```

## Markdown table (good for reading in-repo)

Save as `fundraising-pipeline.md`:

```markdown
# Fundraising pipeline — <round>, target $<amount>

_Updated: <date>_

| Investor | Partner | Tier | Stage | Source | Last contact | Next action | Due | Check/Interest | Notes |
|---|---|---|---|---|---|---|---|---|---|
| Acme Ventures | Jane Doe | A | Engaged | Intro via Sam | 2026-06-18 | Send deck + data room | 2026-06-22 | Lead ~$1.5M | Wants retention cohorts |
| Beta Capital | John Roe | B | Contacted | Cold email | 2026-06-17 | Follow-up #1 | 2026-06-23 | ? | No reply yet |
| Lee Wong (angel) | — | A | Met | Intro via PortaCo founder | 2026-06-15 | Send SAFE | 2026-06-21 | $50–100K | Fills, won't lead |

## Funnel snapshot
- Researched: 24
- Contacted: 11
- Engaged: 5
- Met: 3
- Diligence: 1
- Committed: 0  (target: $<amount>, soft-circled: $<amount>)

## Due now
- Beta Capital — follow-up #1 (today)
- Lee Wong — send SAFE terms (today)

## Passed (and why) — this is signal, not just history
- Gamma Partners — "too early, come back at $50K MRR"
- Delta VC — "outside our geo"
```

## Stage reference

`Researched → Contacted → Engaged → Met → Diligence → Term sheet/Committed`
(plus `Passed` and `Dormant` as terminal states).

## Rules of thumb baked in

- Every investor in **Contacted → Diligence** must have a non-empty **Next
  action** and **Due** date.
- Two value-adding follow-ups, then move to **Dormant** — don't pester.
- Record **why** on every **Passed** row; repeated reasons = a fixable problem.
- Keep adding to **Researched** until you have signed commitments.
