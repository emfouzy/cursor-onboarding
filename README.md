# Cursor IDE Onboarding — Setup Report

## Tools Installed

### 1. Cursor IDE
- Downloaded and installed from https://cursor.com/
- Version: 0.50.x (latest)
- Platform: Windows 11

### 2. Claude Code Extension
- Installed via Cursor Extensions panel (search: "Claude Code")
- Logged in using Anthropic Console account (API key)

### 3. Codex Extension
- Installed via Cursor Extensions panel (search: "Codex")
- Installed by OpenAI (6.4M downloads)

---

## Steps Completed

1. ✅ Installed Cursor IDE from the official website
2. ✅ Installed Node.js v24.16.0 (required for Claude Code CLI)
3. ✅ Installed Git for Windows
4. ✅ Searched and installed the **Claude Code** add-on from the Extensions panel
5. ✅ Logged in to Claude Code via Anthropic Console (API key)
6. ✅ Searched and installed the **Codex** add-on from the Extensions panel
7. ✅ Created a public GitHub repository
8. ✅ Cloned and opened the repository in Cursor IDE
9. ✅ Created this `README.md` file
10. ✅ Committed and pushed to GitHub

---

## Issues Encountered & Solutions

### Issue 1: `npm` not recognized after installing Node.js
> Running `npm install` in PowerShell returned "term not recognized" error.

**Solution:** Closed and reopened Cursor IDE so PowerShell could reload the PATH environment variable.

### Issue 2: PowerShell execution policy blocked npm scripts
> Error: "running scripts is disabled on this system"

**Solution:** Ran `Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned` in PowerShell.

### Issue 3: SSL certificate error during Claude Code install
> `npm error UNABLE_TO_VERIFY_LEAF_SIGNATURE`

**Solution:** Used `--strict-ssl=false` flag: `npm install -g @anthropic-ai/claude-code --strict-ssl=false`

### Issue 4: Claude Code login requires Pro/Max subscription
> Browser showed "Claude Max atau Pro diperlukan untuk terhubung ke Claude Code"

**Solution:** Used Anthropic Console API key instead. Set `ANTHROPIC_API_KEY` environment variable and selected option 2 (Console account) during login.

### Issue 5: `git` not recognized
> Running `git clone` returned "term not recognized" error.

**Solution:** Downloaded and installed Git for Windows from https://git-scm.com/download/win, then reopened Cursor.

---

## Notes

- This repository was created as part of a technical onboarding/assessment task.
- All tools were installed and configured successfully on June 2026.