# Manual-Import Bundle — Perplexity Spaces / ChatGPT Projects / Claude Projects / NotebookLM / Telegram Saved Messages

These destinations do **not** offer a public write API, so the agent cannot push directly. The bundle below is the minimum clean package + the exact steps to import each one in under 60 seconds.

## Files to import
1. `terminal-audit.md` — full audit
2. `roadmap.csv` — 50 rows
3. `roadmap-notebook.md` — condensed knowledge base

---

## Perplexity Spaces
1. Open Perplexity → Spaces → **New Space** named "Wallestars Ultimate Workspace".
2. Add files: drag `terminal-audit.md` + `roadmap-notebook.md` + `roadmap.csv`.
3. Set Space instructions: paste the "Executive Summary" + "Priority Matrix" sections.
4. Pin three starter threads: *Fix SSH to srv1201204*, *Rotate GitHub PAT*, *Phase-1 kickoff*.

## ChatGPT Projects
1. ChatGPT → sidebar → **New project** "Wallestars Ops".
2. Upload the three files to the project Files panel.
3. In "Project instructions" paste the "Environment Signals" + "Derived Action Items" sections.

## Claude Projects
1. Claude → Projects → **Create project** "Wallestars Ops".
2. Attach the three files to Project knowledge.
3. In "Custom instructions": paste "Environment Signals" + "Priority Matrix".

## NotebookLM
1. NotebookLM → **New notebook** "Wallestars Ops".
2. Add sources: upload `terminal-audit.md` and `roadmap-notebook.md`.
3. Generate Audio Overview and FAQ; pin to top.

## Telegram Saved Messages
1. On phone/desktop Telegram, open **Saved Messages**.
2. Forward/upload the three files (max 2 GB each).
3. Pin message with the executive summary paragraph.

## Notion (writable via connector)
The agent handles this automatically in the "Wallestars HQ" workspace.

## GitHub
Automatically written to a new branch + PR.

## Supabase
Automatically loaded into `ops.roadmap_steps`.

## Linear
Automatically created as project + 50 issues.

## Google Docs + Drive
Automatically uploaded to `Wallestars / Operations`.

## Slack + Discord + Outlook + OneDrive
Summary delivered automatically.
