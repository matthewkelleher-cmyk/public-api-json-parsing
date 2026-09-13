# Project: [Name — TBD] — Databricks AI/BI Hackathon

## What this project is
- Entry in a 3-week, open-ended company hackathon exploring Databricks AI/BI:
  AI/BI Dashboards, Genie Agents (conversational analytics), Genie space
  (business-user front end), and the Unity Catalog semantic layer underneath.
- Running on a trial Databricks workspace, live for 30 days.
- The goal is exploration, not polish: try things the team doesn't already
  know how to do. What we build matters, but so does documenting the
  experience — what was easy, what took real effort, what needed outside help.
- Data: [TBD — public/open dataset, synthetic data, or TIL internal data].
  No client data, ever, in this repo or the workspace.

## Workflow / environment
- Local development happens in VS Code. This repo is a GitHub mirror of
  Databricks notebooks — there is no direct Databricks CLI or terminal
  integration set up for Claude in this project, intentionally.
- Loop: edit locally → commit → push to the `Matthew` branch → pull that
  branch into the Databricks workspace via a Git folder to actually run it.
- Because Claude can't execute anything against the live workspace, treat all
  notebook edits as proposed code changes to be reviewed and tested in
  Databricks, not as verified-working output.

## Notebook format
- Notebooks are plain `.ipynb` files. Edit them as standard Jupyter
  notebooks — cell by cell, preserving existing cell boundaries and order
  unless asked to restructure them.

## Data / catalog
- Unity Catalog catalog.schema: TBD
- Key tables / views: TBD
- Any Genie space(s) or AI/BI dashboard(s) this code feeds: TBD

## Team & conventions
- Team: TBD
- Working branch: `Matthew`
- Notebook / file naming conventions: TBD

## Hackathon deliverables — keep these in view
1. **Live build** — must actually run in the trial workspace, demoed there,
   not just committed code.
2. **One-page writeup**, covering:
   - What we built and why we picked it
   - What came together quickly vs. what took real effort
   - Where a client doing this alone would want a hand
   - What we'd try next with another three weeks

Consider keeping a running `NOTES.md` (or similar) alongside this file to log
friction points, surprises, and dead ends as they happen — it's much easier
to write the one-pager from real-time notes than to reconstruct three weeks
of exploration from memory at the deadline.
