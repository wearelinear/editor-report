# SOP: Weekly Creative Output Report Refresh

**Live report:** https://wearelinear.github.io/editor-report/
**Tracks:** Naqeeb, Lucas, Rami, Felipe, Matt, Ardee, Bruno Volpe, Rodrigo, Pilar

---

## Running a Refresh (Any Machine)

Open **Claude Code** and type:

> "Refresh the creative output report for the last 7 days"

Claude will search all three Slack channels, add new entries, push to GitHub, and the live site updates within ~1 minute.

---

## First-Time Setup on a New Machine

You need three things: **Claude Code**, **Slack connected**, and **GitHub connected**.

### 1. Install Claude Code
Download from https://claude.ai/code and sign in.

### 2. Connect Slack
In Claude Code settings, add the Slack MCP server and connect it to the **Linear** Slack workspace. Claude needs read access to public and private channels.

### 3. Connect GitHub
Install the GitHub CLI: https://cli.github.com
Then run in a terminal:
```
gh auth login
```
Sign in with the `wearelinear` GitHub account (or an account that has write access to the `wearelinear` org).

### 4. Clone the report repo
In a terminal, run:
```
gh repo clone wearelinear/editor-report
```
This creates an `editor-report/` folder — that's where Claude will make edits and push from.

### 5. Tell Claude where the repo is
When you first run a refresh on a new machine, tell Claude:

> "Refresh the creative output report for the last 7 days — the repo is cloned at [full path to editor-report folder]"

After the first run, Claude will remember the path.

---

## Custom Date Ranges

> "Refresh the creative output report from March 11 to March 17"
> "Check the last 2 weeks for the creative output report"

---

## Adding a New Team Member

> "Add [Name] to the creative output report — their Slack ID is [ID], they're in Pod [X]"

---

## Reference

| Thing | Location |
|---|---|
| GitHub repo | https://github.com/wearelinear/editor-report |
| Live URL | https://wearelinear.github.io/editor-report/ |
| Pods 1 & 2 channels | #linear-pod-1-qc-requests, #linear-pod-2-qc-requests |
| Pod 4 channel | #linear-pod-4-creative-production |
