<div align="center">

# 🔐 Vaulted

### by Ilmnos Lab ・ One portable Obsidian vault committed alongside every code project — shared second brain for you and every AI coding agent. Claude Code / Cursor / Windsurf / GitHub Copilot Agent / Devin ready.

</div>

---

<div align="center">

**[🚀 Quick Start](#-quick-start--3-phases) ・ [📦 What's in the box](#-whats-in-the-box) ・ [📋 4 Non-Negotiable Rules](#-4-non-negotiable-rules-memorize-these) ・ [🐛 Troubleshooting](#-troubleshooting-top-3) ・ [📜 License](#-license)**

</div>

<div align="center">

[![Vault structure — guide compliant](https://img.shields.io/badge/vault%20structure-guide%E2%80%94compliant-2ea44f?style=flat-square)](.obsidian-vault)
[![AI agents — 6 supported](https://img.shields.io/badge/AI%20agents-6%20supported-7C3AED?style=flat-square)](#-mirrors-auto-generated--never-hand-edit)
[![Sync script — PowerShell](https://img.shields.io/badge/sync%20script-PowerShell-5B8C5A?style=flat-square)](sync-agent-briefings.ps1)
[![License — MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](#-license)

</div>

---

## 🤔 What this is

A drop-in **`.obsidian-vault/` folder** you copy into ANY new or existing code project
(JavaScript / Python / Rust / Swift / Go / Data Science / Mobile) and commit. It gives you and every AI coding agent
a structured, instantly-readable second brain — plain Markdown, inside Git, zero SaaS lock-in. It is the portable context layer that sits between "what the code literally says" and "what the AI actually needs to know to work safely without pestering you."

```
your-repo/
├── src/                          ← Your real code (as usual)
├── .obsidian-vault/             ← THIS TEMPLATE  drop it in, commit it, done.
│   ├── daily/                   ← Session logs + saved reusable prompt files
│   ├── decisions/               ← Architecture Decision Records (ADRs)
│   ├── specs/                   ← Feature specifications
│   ├── bugs/                    ← Bug investigations + repro steps
│   ├── retro/                   ← Milestone reflections / lessons learned
│   ├── templates/               ← Obsidian Templater templates
│   ├── CLAUDE.md                ← ✅ CANONICAL AI BRIEFING  edit ONLY this file
│   ├── OPERATIONAL_GUIDE.md     ← Full human onboarding guide (visible in Obsidian GUI)
│   └── Dashboard.md             ← Dataview-powered project overview
├── CLAUDE.md                    ← 📦 mirror (do NOT edit; auto-generated)
├── .cursorrules                 ← 📦 mirror (do NOT edit; auto-generated)
├── .windsurfrules               ← 📦 mirror (do NOT edit; auto-generated)
├── .github/
│   └── copilot-instructions.md  ← 📦 mirror (do NOT edit; auto-generated)
└── sync-agent-briefings.ps1     ← < 0.3 s  canonical → mirrors, zero drift.
```

---

## ✨ 6 features that make it different

| # | Feature | Why you care |
|---|---|---|
| 🧩 | **Stack-agnostic by design** | Replace the placeholder content in [CLAUDE.md](.obsidian-vault/CLAUDE.md) → ready for Python / Rust / Swift / data-science / mobile in 60 seconds. No TS / Next / YouTube-course hardcode pollution. |
| 🤖 | **6 AI agents supported, zero rename needed** | Claude Code CLI, Cursor, Windsurf, GitHub Copilot Agent + two future keyword-search aliases. Each agent reads its native-convention file at its exact hardcoded scan path. |
| 🚀 | **Saved prompts: 2 copy-paste one-liners a day** | Session End prompt generates your daily log. Session Triage prompt updates canonical CLAUDE.md Current State + drafts bugs / ADRs / specs into their folders with bidirectional breadcrumbs. |
| 🪞 | **Canonical + mirror pattern: edit ONE file** | ✅ Edit ONLY `.obsidian-vault/CLAUDE.md`. 🚫 Never touch the 6 mirrors. `& .\sync-agent-briefings.ps1` pushes updates in < 0.3 seconds. Zero drift. |
| 🪟 | **Obsidian GUI-native knowledge base** | The operational guide, bug notes, specs, ADRs, retro notes, and live Dataview Dashboard all live inside the actual second-brain vault — not an afterthought in a VS Code sidebar. |
| 🔐 | **100% Markdown, 100% Git, zero lock-in** | Every file is portable text committed alongside your source code. Delete the `.obsidian-vault/` folder and you lose nothing. |

---

## 📦 What's in the box

### 🗂️ Vault (`.obsidian-vault/`)

All 6 required folders + 7 core files, committed alongside your code:

| Path | Purpose |
|---|---|
| `daily/` | Every coding day: scratchpad logs + the two saved AI prompt files (Session End + Session Triage). |
| `specs/` | Pre-coding feature specifications. Status: `Draft` → `Done`. |
| `decisions/` | Architecture Decision Records (ADRs). Status: `Proposed` → `Accepted` / `Superseded`. |
| `bugs/` | Bug investigation write-ups with reproduction steps, root cause, resolution. Status: `Open` → `Done`. |
| `retro/` | Milestone reflections. Lessons learned. Permanent Do-Not / Key-Decision candidates. |
| `templates/` | Obsidian Templater templates: `_template-adr.md`, `_template-spec.md`, `_template-bug.md`. |
| [CLAUDE.md](.obsidian-vault/CLAUDE.md) | ✅ **CANONICAL AI BRIEFING — this is the ONE file you edit and sync.** |
| [OPERATIONAL_GUIDE.md](.obsidian-vault/OPERATIONAL_GUIDE.md) | Full human onboarding guide. Read it before writing code. Shown in the Obsidian GUI. |
| [Dashboard.md](.obsidian-vault/Dashboard.md) | Dataview-powered project dashboard: Open Bugs / Open Specs / Recent Decisions at a glance. |
| [AGENT.md](.obsidian-vault/AGENT.md) | Generic "agent" keyword alias inside the vault (ranks for unknown future agents). |
| [AI_BRIEFING.md](.obsidian-vault/AI_BRIEFING.md) | Generic "briefing" keyword alias inside the vault. |

### 🪞 Mirrors (auto-generated — NEVER hand-edit)

Six files kept byte-identical to canonical [.obsidian-vault/CLAUDE.md](.obsidian-vault/CLAUDE.md) every time you run the sync script:

| Mirror file | Agent convention |
|---|---|
| `CLAUDE.md` (project root) | **Anthropic Claude Code CLI** — auto-loads `./CLAUDE.md` from launch CWD (does not scan subfolders). |
| `.cursorrules` | **Cursor IDE by Anysphere** — native rules file read from project root. |
| `.windsurfrules` | **Windsurf IDE by Codeium / Cascade** — native rules file read from project root. |
| `.github/copilot-instructions.md` | **GitHub Copilot Agent** (VS Code / github.dev) — Microsoft official convention, loaded preferentially. |
| `.obsidian-vault/AGENT.md` | Generic keyword alias for future unknown agents that rank on "agent". |
| `.obsidian-vault/AI_BRIEFING.md` | Generic keyword alias for future unknown agents that rank on "briefing". |

Every mirror file starts with a DO-NOT-EDIT warning header on line 1 so no AI or human ever edits the wrong copy by accident.

### 🔌 Required Obsidian Plugins (pre-installed)

Listed in [community-plugins.json](.obsidian-vault/.obsidian/community-plugins.json):

| # | Plugin | Configured for |
|---|---|---|
| 1 | **Templater** | `templates_folder: "templates"`. Placeholders: `<% tp.file.title %>`, `<% tp.date.now("YYYY-MM-DD") %>`. |
| 2 | **Dataview** | Live Dashboard queries against bug/spec/decision frontmatter. |
| 3 | **Obsidian Git** | `autoBackupAfterFileChange: true`, `autoSaveInterval: 10` minutes. Auto-commits the vault. |
| 4 | **Linter** | Markdown formatting standardization on save. |

### ⚙️ Project root files

| File | Purpose |
|---|---|
| [sync-agent-briefings.ps1](sync-agent-briefings.ps1) | Read canonical `.obsidian-vault/CLAUDE.md` once → write all 6 mirrors with the DO-NOT-EDIT warning header. < 0.3 s. Run after EVERY edit to canonical. |
| [.gitignore](.gitignore) | Ignores transient Obsidian workspace state (`.obsidian-vault/.obsidian/workspace.json`, `workspace-mobile.json`) so each dev retains their own UI layout. |
| `Obsidian Project.code-workspace` | VS Code workspace file that hides `.obsidian/` plugin binaries from the file explorer. |

---

## 🚀 Quick Start — 3 phases

### Phase 1 — Day 0 setup (5 minutes, once per project)

```bash
# 1) Copy this entire template folder into your project root, then cd into your project.

# 2) Init git if brand new:
git init

# 3) Open Obsidian on the .obsidian-vault/ folder (NOT the project root — this is the #1 mistake)
#    Obsidian → File → Open vault → Choose folder → click on `.obsidian-vault/` → Select Folder.
#    Confirm the vault top level shows 6 folders: decisions, specs, bugs, daily, retro, templates.

# 4) Open your CODE EDITOR (VS Code / Cursor / Windsurf) on the PROJECT ROOT folder.

# 5) Fill in the canonical AI briefing — inside Obsidian GUI or in VS Code:
#    - Open  .obsidian-vault/CLAUDE.md
#    - Replace `# [YOUR PROJECT NAME]`
#    - Write 1–2 sentences in `## What this is`
#    - Fill the `## Tech stack` table, delete inapplicable rows
#    - Write initial `## Current state` bullets + today's date on `Last updated: YYYY-MM-DD`
#    - DELETE every InvoiceFlow example inside every section (they are labeled DELETE)
#    - SAVE.

# 6) Run sync script (PowerShell terminal at project root):
& .\sync-agent-briefings.ps1

# 7) First commit — code + vault + mirrors together:
git add -A
git commit -m "Initial commit: Vaulted wired up by Ilmnos Lab."
```

Expected output of Step 6:
```
  [OK] Synced  ->  CLAUDE.md
  [OK] Synced  ->  .cursorrules
  [OK] Synced  ->  .windsurfrules
  [OK] Synced  ->  .github\copilot-instructions.md
  [OK] Synced  ->  .obsidian-vault\AGENT.md
  [OK] Synced  ->  .obsidian-vault\AI_BRIEFING.md

===============================================================
  [DONE] sync-agent-briefings.ps1 - complete
===============================================================
  Canonical source : .obsidian-vault/CLAUDE.md
  Mirrors updated  : 6
  Dirs created     : 0
  Next step: commit code + vault + mirrors together in Git.
```

If PowerShell shows the red error `File … cannot be loaded because running scripts is disabled on this system`, run once and then immediately retry sync:
```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass -Force
```
Or for a one-time permanent developer-safe fix (account scope; CWD does not matter):
```powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned -Force
```

### Phase 2 — Daily Loop (every coding day; < 10 minutes total)

1. **Code normally.** Commit frequently every 30–90 minutes: `git commit -m "feat: …"`.
2. **End of day → AI generates your daily log.** Paste this one-liner into your AI agent chat:
   ```
   Read this file exactly: .obsidian-vault/daily/_PROMPT-session-end-generate-daily-note.md. Then execute the prompt instructions it contains. Use today's actual date.
   ```
3. **3-minute hard-limit human edit** on the generated `daily/YYYY-MM-DD.md`: add the *why* behind decisions, offline Slack/Zoom research context that the AI did not have access to, and delete obvious hallucinations. SAVE.
4. **Run Triage prompt → AI migrates quality items automatically:**
   ```
   Read this file exactly: .obsidian-vault/daily/_PROMPT-triage-daily-note-migrate.md. Then execute the prompt instructions it contains. Use today's actual date.
   ```
   AI updates canonical `.obsidian-vault/CLAUDE.md` → Current State section; drafts bugs/specs/ADRs into their folders with 🚧 status badges; adds bidirectional breadcrumb links back to the daily note; prints a final report table with 🟡/🟢 per-file review flags.
5. **60-second human review:** open every 🟡-flagged draft file → keep, quick-edit, or delete the junk. If Triage auto-drafted a retro file on a random day and no milestone ended: DELETE IT IMMEDIATELY (false positive).
6. **Run sync script again to push the canonical CLAUDE.md update to all 6 mirrors:**
   ```powershell
   & .\sync-agent-briefings.ps1
   ```
7. **One single Git commit of code + vault + mirrors together (guide rule — vault and code are one artifact):**
   ```powershell
   git add -A
   git commit -m "daily: YYYY-MM-DD session + triage migrations."
   ```

### Phase 3 — Milestone Loop (every 2–8 weeks: shipped v0.1, sprint ended, integration shipped, rewrite done)

1. Run the normal daily session + triage on the milestone-final day. If the daily note contains milestone-end language, the Triage prompt auto-drafts a `retro/NNN-milestone-name.md` for you.
2. Open the retro draft. **You write the real postmortem:** 5 sections recommended — (1) goals vs reality, (2) what worked, (3) what failed + root cause, (4) 3–10 concrete action items / process rules, (5) link map back to evidence daily notes / bugs / commits / PRs.
3. **MANUALLY (and only when earned)** promote real rules into canonical [.obsidian-vault/CLAUDE.md](.obsidian-vault/CLAUDE.md):
   - Into `## Key decisions made` → each entry MUST link to a new ADR in `decisions/NNN-slug.md`.
   - Into `## Do Not` → 🛠️ project-specific hard rules.
   - Into `## Current state` → milestone-complete status.
   (The Triage prompt never auto-edits permanent sections. YOU are the gatekeeper. This is deliberate.)
4. Run sync script → commit the retro note + ADR drafts + CLAUDE.md + mirrors together as one milestone commit.

That's the whole system. Do the daily loop and the second brain builds itself.

---

## 📋 4 Non-Negotiable Rules (memorize these)

Break any of these → silent data loss or the next AI reads stale context and redoes 1–4 hours of work.

| # | Rule | Why it matters |
|---|---|---|
| 🔒 1 | **Edit ONLY files INSIDE `.obsidian-vault/`. NEVER outside.** | Any file OUTSIDE `.obsidian-vault/` that sounds like a briefing (root `CLAUDE.md`, `.cursorrules`, `.windsurfrules`, `.github/copilot-instructions.md`) is a **disposable auto-generated mirror**. The sync script **overwrites it every run**. Hand-edit a mirror and the next sync permanently deletes your edit. Mirror files literally start with a `DO NOT EDIT THIS FILE` warning on line 1 — read it. |
| 🔒 2 | **There are TWO files named `CLAUDE.md`. Know exactly which one to edit.** | ✅ **EDIT: `.obsidian-vault/CLAUDE.md` — this is the CANONICAL source of truth.** <br> ❌ **NEVER touch: `./CLAUDE.md` (project root, next to `.gitignore`) — this is a disposable mirror.** |
| 🔒 3 | **After EVERY edit to `.obsidian-vault/CLAUDE.md` → run `& .\sync-agent-briefings.ps1` at the project root BEFORE `git commit`.** | Keeps all 6 mirrors byte-consistent. Skipping = the next AI agent reads outdated context. Takes < 0.3 seconds. Just run it. |
| 🔒 4 | **Code + vault = ONE Git repo, ONE end-of-day commit.** | The vault IS the project's documentation. Treat it exactly like code: commit it, branch it, PR it, ship it. Split them and they drift apart and everything silently breaks. |

---

## 💯 Bonus: Drop into an EXISTING code project

1. Copy this entire template folder into the existing project root. If a `.github/` folder already exists, just merge it — the only file inside is `copilot-instructions.md` which you want to keep as the authoritative briefing mirror.
2. **If the existing project already has good content in root `CLAUDE.md`, `.cursorrules`, `.windsurfrules`, or `.github/copilot-instructions.md`** → copy ALL that content into the canonical `.obsidian-vault/CLAUDE.md` file FIRST, merging manually into the right 7-section shape. THEN run the sync script. The good content ends up identical across all files and you now have a single source of truth.
3. Open Obsidian on `.obsidian-vault/` → fill the briefing → commit. From the next coding day on, follow Phase 2 (Daily Loop) as normal. No other setup.

---

## 🐛 Troubleshooting (Top 3)

Full 9-row table lives in [OPERATIONAL_GUIDE.md → Section 5](.obsidian-vault/OPERATIONAL_GUIDE.md). Here are the three you will hit:

| ID | Symptom | Root cause (99% of the time) | Exact fix |
|---|---|---|---|
| **TS-01** | PowerShell red error: `sync-agent-briefings.ps1 : File … cannot be loaded because running scripts is disabled on this system.` | Windows ships with script execution disabled by default. | **Per-session safe (try first):** `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass -Force` then immediately re-run sync. **One-time permanent fix:** `Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned -Force`. Close and reopen the terminal. |
| **TS-02** | Obsidian file explorer shows `.gitignore`, `sync-agent-briefings.ps1`, `.cursorrules` at the top level. Dashboard shows zero bugs / zero specs. | The #1 new-user mistake — you opened Obsidian on the **project root** folder instead of the `.obsidian-vault/` vault subfolder. | 1. Obsidian → Settings → Vault → Close vault. 2. File → Open vault → Browse INTO your project → click ONCE on the `.obsidian-vault/` folder → Select Folder. 3. Confirm top level shows the 6 folders: decisions / specs / bugs / daily / retro / templates. 4. Open Dashboard → Dataview now works correctly. 5. If files were accidentally written to the project root from the wrong vault, delete them. |
| **TS-03** | Sync script ran `[OK]` × 6 successfully → but next time you open Cursor it still reads OLD CLAUDE.md content from a previous version. | Either (a) you **directly edited a mirror file** at some point in the last 24h and sync overwrote it (but Cursor cached stale content in memory), or (b) you skipped Rule 🔒 3 and forgot to run sync after editing the canonical. | 1. Close ALL AI agents + VS Code / Cursor / Windsurf FULLY (Quit, not just close window). Wait 10 s. 2. Open ONLY the canonical file: `.obsidian-vault/CLAUDE.md`. Confirm its content looks correct. 3. Re-run sync once: `& .\sync-agent-briefings.ps1`. 4. Reopen your editor. Now the agent reads fresh context. 5. If still broken: `git diff` → do you see mirror edits? If yes: `git checkout -- CLAUDE.md .cursorrules .windsurfrules .github/copilot-instructions.md .obsidian-vault/AGENT.md .obsidian-vault/AI_BRIEFING.md` → fix the canonical properly → run sync again. |

---

## 📚 Full documentation

All documentation lives INSIDE the vault (second-brain-native):

| Link | Contents |
|---|---|
| [.obsidian-vault/OPERATIONAL_GUIDE.md](.obsidian-vault/OPERATIONAL_GUIDE.md) | Full human step-by-step operational manual for every scenario: Day 0 / Daily / Milestone / Retro / Project End. Includes the full 9-row Troubleshooting table + how to rescue mirror edits. |
| [.obsidian-vault/daily/_PROMPT-session-end-generate-daily-note.md](.obsidian-vault/daily/_PROMPT-session-end-generate-daily-note.md) | Saved reusable Session End prompt. Generates today's daily log (5 sections) from git history + chat context. Copy the one-liner invocation from inside the file. |
| [.obsidian-vault/daily/_PROMPT-triage-daily-note-migrate.md](.obsidian-vault/daily/_PROMPT-triage-daily-note-migrate.md) | Saved reusable Session Triage prompt. Migrations: updates CLAUDE.md Current State, drafts bugs/ADRs/specs/retros, adds bidirectional breadcrumbs, produces 🟡/🟢 human-review report table. |

---

## 🤝 Contributing

Found a bug? Missing a feature? Open an issue or PR on the template repository.

Especially welcome contributions:
- New agent-native mirror conventions (add them to the `$Mirrors` array in [sync-agent-briefings.ps1](sync-agent-briefings.ps1)).
- New saved prompt files in `.obsidian-vault/daily/` for recurring workflows (bug-fix triage, release checklist, incident postmortem, etc.).
- A cross-platform Bash/Zsh equivalent of `sync-agent-briefings.ps1` for macOS / Linux teams.

---

## 🙏 Credits & Inspiration

**Vaulted by Ilmnos Lab** is built on top of the excellent written guideline and work published by **HermesZum**:

👉 **[HermesZum / Obsidian-VS-Code-Copilot-AI-Second-Brain-Per-Project-Setup](https://github.com/HermesZum/Obsidian-VS-Code-Copilot-AI-Second-Brain-Per-Project-Setup)**

The following core architecture and design all originate from that project:
- The 6-folder `.obsidian-vault/` layout (decisions / specs / bugs / daily / retro / templates).
- The specific 4-plugin Obsidian community stack (Templater, Dataview, Obsidian Git, Linter) and its settings.
- The idea of storing a canonical AI briefing file inside the vault and keeping code + vault in one Git repository.
- The Obsidian Dataview Dashboard pattern, `file.mtime` timestamp semantics, and uppercase status filters (`Open`, `Draft`, `Done`).

Additions and refinements in **Vaulted by Ilmnos Lab**:
- Universal / stack-agnostic `.obsidian-vault/CLAUDE.md` template with 7-section layout and realistic InvoiceFlow placeholders.
- **Canonical + 6-mirror** briefing distribution pattern (vault canonical → root `CLAUDE.md`, `.cursorrules`, `.windsurfrules`, `.github/copilot-instructions.md`, vault `AGENT.md`, vault `AI_BRIEFING.md`) + the `sync-agent-briefings.ps1` PowerShell script that keeps them byte-consistent in < 0.3 seconds.
- **Ground-rule path-ambiguity hardening** so no AI ever edits a mirror file by accident (3-layer defense: ground rules table, no bare `CLAUDE.md` path references in any prompt, sync-script banner on every mirror line 1).
- Saved reusable **Session End** + **Session Triage** prompt files in `.obsidian-vault/daily/` with one-liner invocations that turn end-of-session bookkeeping from 45 minutes of manual writing into < 10 minutes of AI-assisted work + 3 minutes of human review.
- Milestone retro loop pattern + manual gatekeeping for permanent `Key decisions` / `Do Not` rules (the AI proposes; you approve).
- Full `.obsidian-vault/OPERATIONAL_GUIDE.md` human onboarding manual (Day 0 / Daily / Milestone / Retro / 9-row Troubleshooting / 4 Commandments).

---

## 📄 License

**MIT.** Do anything, use anywhere. No attribution required to ship Vaulted inside your own projects or company repos.

---

<div align="center">

**🔐 Vaulted — by Ilmnos Lab**

Made with 🧠 for teams that want their AI to stop asking "what the code, actually?"

</div>
