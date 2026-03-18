# SOP: Weekly Editor Report Refresh

**Live report:** https://wearelinear.github.io/editor-report/
**Tracks:** Naqeeb, Lucas, Rami, Felipe
**Channels:** #linear-pod-1-qc-requests & #linear-pod-2-qc-requests

---

## Running a Refresh (Any Machine)

Open **Claude Code** and type:

> "Refresh the editor report for the last 7 days"

Claude will search both QC Slack channels, add new entries, push to GitHub, and the live site updates within ~1 minute.

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

> "Refresh the editor report for the last 7 days — the repo is cloned at [full path to editor-report folder]"

After the first run, Claude will remember the path.

---

## Custom Date Ranges

> "Refresh the editor report from March 11 to March 17"
> "Check the last 2 weeks for the editor report"

---

## Adding a New Editor

> "Add [Name] to the editor report — their Slack ID is [ID]"

---

## Reference

| Thing | Location |
|---|---|
| GitHub repo | https://github.com/wearelinear/editor-report |
| Live URL | https://wearelinear.github.io/editor-report/ |
| Slack channels | #linear-pod-1-qc-requests, #linear-pod-2-qc-requests |
