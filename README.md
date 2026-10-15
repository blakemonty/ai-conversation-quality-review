# AI Conversation Quality Review

A manual quality review of 120 AI-assisted customer support conversations, built to demonstrate a structured QA workflow for evaluating conversational AI.

> **Disclosure:** North Ridge Outfitters is a fictional outdoor retailer created for this portfolio project. The 120 conversation transcripts are synthetic. The review process, scoring, findings, and analysis are real work I did against that data.

## What this project does

A newly "deployed" AI customer support assistant was evaluated across 120 conversations spanning seven support scenarios — shipping delays, returns, warranty, product recommendations, general inquiries, billing, and account access. Each conversation was scored against four quality dimensions, and any conversation that fell short was tagged with a specific finding and severity so the issues could be analyzed as a set, not just flagged one by one.

## Methodology

Every conversation was reviewed against four dimensions:

| Dimension | What it checks |
|---|---|
| **Accuracy** | Is the information the assistant gives factually correct and verifiable? |
| **Tone** | Does the register match the situation (measured for a complaint, warm for a routine ask)? |
| **Completeness** | Does the response fully resolve what the customer actually needed? |
| **Policy Compliance** | Does the response stay within what the assistant can accurately promise? |

Each dimension was scored Pass/Fail. Where a conversation failed, it received a **severity level** (Low/Medium/High) and a **Primary QA Finding** — a single label capturing the main issue — plus a written reviewer note explaining the reasoning.

## Key findings

25 of 120 conversations (21%) were flagged with at least one finding:

| Primary QA Finding | Count |
|---|---|
| Incorrect Information | 9 |
| Incomplete Response | 8 |
| Missing Escalation | 5 |
| Generic Recommendation | 2 |
| Missing Empathy | 1 |

**The standout pattern:** Almost every piece of Incorrect Information followed the exact same pattern. Instead of making nine unrelated factual errors, the AI made the same mistake repeatedly: it confidently promised a specific delivery date for delayed shipments without any tracking data to back it up. This means we aren't looking at random bugs, but a single, easily coachable habit—the AI making unverified claims just to reassure the user.

## Repo contents

- `executive_summary.docx` — the top-level findings and recommendations, written for a non-technical stakeholder
- `supporting_evidence_workbook.xlsx` — the full review log (all 120 conversations), every flagged conversation with its transcript and reviewer rationale, and a dedicated breakdown of the delivery-date pattern
- `data/` — the underlying conversation transcripts and review log the analysis was built from

Start with the executive summary for the findings; open the workbook if you want to see the actual conversation behind any given number.

> **Note:** GitHub doesn't render `.docx` or `.xlsx` files inline. Click into either file and select **"View raw"** (or the download icon) to open it locally in Word or Excel.

## Skills demonstrated

AI conversation evaluation • quality assurance methodology design • error/finding taxonomy design • pattern identification across a dataset • technical writing for mixed audiences • spreadsheet-based evidence tracking

## About this project

Built as part of a portfolio. Feedback welcome.
