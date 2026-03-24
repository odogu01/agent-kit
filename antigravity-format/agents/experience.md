---
name: experience
description: Systematic documentation of all learnings, mistakes, corrections, and debugging insights. Built from real errors encountered during development. Use this to avoid repeating mistakes and work faster.
tools: [read_file, grep_search, glob, write_file]
model: gemini-2.0-flash
skills: clean-coder
---

# 🧠 Experience - Documented Learnings

> "Those who cannot remember the past are condemned to repeat it." - George Santayana

---

## Purpose

This skill captures every mistake, correction, and insight gained through real development work. Each entry follows the format:

```
PROBLEM → LEARNING → ACTION
```

---

## 📋 All Experience Entries

### Table of Contents
1. [Antigravity Setup](#1-antigravity-setup)
2. [Git Workflow](#2-git-workflow)
3. [PowerShell vs Bash](#3-powershell-vs-bash)
4. [Path Handling](#4-path-handling)
5. [File Permissions](#5-file-permissions)

---

## 1. Antigravity Setup

### 1.1 - Antigravity Data Location

**❌ Mistake/Error:**
```
Cloned agent-kit to ~/.gemini/skills/ or ~/.config/antigravity/skills/
Commands not appearing in Antigravity
```

**✅ Correction:**
```
Antigravity stores data in ~/.gemini/ NOT ~/.config/antigravity/
Antigravity uses TWO folders inside ~/.gemini/:
- agents/  (35 .md files)
- commands/ (36 .toml files)
```

**📝 Insight:**
```
Antigravity is built ON TOP of Gemini CLI, not separate.
It reuses ~/.gemini/ folder structure.
skills/ folder is for Gemini CLI skills, NOT Antigravity.
```

**⚡ Action Item:**
```
For Antigravity: git clone https://github.com/odogu01/agent-kit.git ~/.gemini
For Gemini CLI:  git clone https://github.com/odogu01/agent-kit.git ~/.gemini/skills
```

---

### 1.2 - Antigravity Agent Format

**❌ Mistake/Error:**
```
Skills in SKILL.md format don't work as Antigravity commands
Expected /react-best-practices but nothing happens
```

**✅ Correction:**
```
Antigravity uses TWO formats:
1. AGENTS: .md files in agents/ folder
   - YAML frontmatter with name, description, tools, skills
   - Full markdown instructions

2. COMMANDS: .toml files in commands/ folder
   - name, description, prompt fields
   - Shortcut to invoke agents
```

**📝 Insight:**
```
Skills are CONTENT that teaches behavior.
Agents are CONFIGURATION that enables behavior.
Commands are SHORTCUTS that trigger agents.
All three work together.
```

**⚡ Action Item:**
```
When adding skills to Antigravity:
1. Convert SKILL.md → agents/{skill}.md
2. Create commands/{skill}.toml
3. Restart Antigravity
4. Type / to see commands
```

---

### 1.3 - Command Not Loading After Install

**❌ Mistake/Error:**
```
Installed agents and commands but /commands don't appear
Restart didn't help
```

**✅ Correction:**
```
1. Verify files are in correct location:
   - ls ~/.gemini/agents/ (should have .md files)
   - ls ~/.gemini/commands/ (should have .toml files)

2. Check file permissions:
   - Files must be readable

3. Verify Antigravity settings:
   - experimental.enableAgents: true
```

**📝 Insight:**
```
Antigravity caches command list.
Sometimes needs full restart (not just new chat).
Sometimes needs Antigravity app restart.
```

**⚡ Action Item:**
```
After installing commands:
1. Close Antigravity completely
2. Reopen Antigravity
3. Type / to verify commands appear
```

---

## 2. Git Workflow

### 2.1 - Git Identity Not Set

**❌ Mistake/Error:**
```
*** Please tell me who you are.
Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

fatal: unable to auto-detect email address
```

**✅ Correction:**
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

**📝 Insight:**
```
Git needs identity BEFORE first commit.
Global config applies to all repos.
Can override per-repo with --local flag.
```

**⚡ Action Item:**
```
Before ANY git work, check identity:
git config user.name
git config user.email
If empty, set them first.
```

---

### 2.2 - Branch Name Mismatch

**❌ Mistake/Error:**
```
error: src refspec main does not match any
error: failed to push some refs to '...'
```

**✅ Correction:**
```
Local branch was 'master' but tried to push 'main'
Fix: git branch -M main
```

**📝 Insight:**
```
GitHub defaults to 'main' now.
Local repo might have been initialized with 'master'.
Must rename local branch to match remote.
```

**⚡ Action Item:**
```
After git init, immediately:
git branch -M main
```

---

### 2.3 - Push Without Remote

**❌ Mistake/Error:**
```
fatal: not a git repository
```

**✅ Correction:**
```
Need to add remote first:
git remote add origin [URL]
git push -u origin main
```

**📝 Insight:**
```
git clone auto-sets remote.
git init does NOT.
Must add remote manually for new repos.
```

**⚡ Action Item:**
```
After git init for new repo:
1. git remote add origin [URL]
2. git branch -M main
3. git push -u origin main
```

---

## 3. PowerShell vs Bash

### 3.1 - ls -la Not Working

**❌ Mistake/Error:**
```
Get-ChildItem : A parameter cannot be found that matches parameter name 'la'.
```

**✅ Correction:**
```
PowerShell: Get-ChildItem -Path [path] -Force
NOT: ls -la (bash syntax)

Aliases:
- ls = Get-ChildItem
- -la flags don't work the same way
```

**📝 Insight:**
```
PowerShell uses PARAMETERS, not flags like bash.
-la is two flags (-l and -a) in bash.
PowerShell uses -Force for hidden files.
```

**⚡ Action Item:**
```
On Windows, when using PowerShell:
- ls -la → Get-ChildItem -Force
- cat → Get-Content
- rm → Remove-Item
- cp → Copy-Item
- mv → Move-Item
```

---

### 3.2 - Environment Variable Expansion

**❌ Mistake/Error:**
```
Cannot find path 'C:\Users\USER\:USERPROFILE\.gemini'
```

**✅ Correction:**
```
$env:USERPROFILE works in PowerShell directly.
But passing to bash/powershell -Command needs careful quoting.
```

**📝 Insight:**
```
Bash doesn't expand $env:USERPROFILE.
Need to use explicit C:\Users\[username]
Or use PowerShell for PowerShell commands.
```

**⚡ Action Item:**
```
When running PowerShell commands:
- Use explicit paths: C:\Users\USER\...
- Or run in PowerShell directly, not bash -Command
```

---

### 3.3 - Path Differences

**❌ Mistake/Error:**
```
Path not found errors on Windows paths
```

**✅ Correction:**
```
Windows uses: \
Linux/macOS uses: /

PowerShell often needs different syntax than bash.
```

**📝 Insight:**
```
Different shells have different path handling.
Git Bash on Windows handles / paths.
Pure PowerShell prefers \ paths.
```

**⚡ Action Item:**
```
Match shell to path format:
- PowerShell: C:\Users\... 
- Bash/Git Bash: /c/Users/... or /home/...
```

---

## 4. Path Handling

### 4.1 - Tilde Expansion

**❌ Mistake/Error:**
```
~/.config/... paths not working in some contexts
```

**✅ Correction:**
```
~ doesn't expand in all contexts.
Use full path or ensure shell supports tilde.
```

**📝 Insight:**
```
~ is shell feature, not OS feature.
Some tools don't support it.
USERPROFILE is Windows equivalent.
```

**⚡ Action Item:**
```
Prefer explicit paths:
- Windows: $env:USERPROFILE\.config\...
- Linux: /home/username/...
```

---

### 4.2 - Nested Folder Creation

**❌ Mistake/Error:**
```
Path does not exist when trying to clone
```

**✅ Correction:**
```
Create parent directories first:
mkdir -p ~/.config/opencode/skills
git clone ... ~/.config/opencode/skills
```

**📝 Insight:**
```
git clone won't create parent folders.
Parent must exist first.
-p flag creates parents as needed.
```

**⚡ Action Item:**
```
Before git clone to new path:
mkdir -p [parent/path]
git clone [url] [destination]
```

---

## 5. File Permissions

### 5.1 - File In Use

**❌ Mistake/Error:**
```
Cannot remove item ... because it is being used by another process.
```

**✅ Correction:**
```
Close any programs using the folder.
Try again in a few seconds.
Sometimes Antigravity locks its own folders.
```

**📝 Insight:**
```
Windows is more strict about file locks.
Antigravity/Gemini might be running and using files.
Close the app first.
```

**⚡ Action Item:**
```
Before modifying Antigravity folders:
1. Close Antigravity
2. Wait a moment
3. Then modify
```

---

### 5.2 - Symbolic Link Creation

**❌ Mistake/Error:**
```
New-Item : Administrator privilege required
```

**✅ Correction:**
```
Symlinks require admin on Windows by default.
Either:
1. Run PowerShell as Admin
2. Use junction instead (no admin needed)
3. Copy files instead of symlink
```

**📝 Insight:**
```
Linux/Mac: symlinks are easy
Windows: symlinks need admin or Developer Mode enabled
```

**⚡ Action Item:**
```
On Windows, prefer:
- Copy files (simple, works everywhere)
- Or enable Developer Mode for symlinks
```

---

## 🎯 Quick Reference Card

### Antigravity
```
✅ Correct path: ~/.gemini/
❌ Wrong path: ~/.gemini/skills/
❌ Wrong path: ~/.config/antigravity/
```

### Git
```
git config --global user.name "..."
git config --global user.email "..."
git branch -M main
git remote add origin [URL]
```

### PowerShell
```
Get-ChildItem -Force     (not ls -la)
Get-Content              (not cat)
Remove-Item -Recurse     (not rm -rf)
Copy-Item -Recurse       (not cp -r)
```

### Windows Paths
```
Environment: $env:USERPROFILE
Home folder: C:\Users\username
Config: C:\Users\username\.config\
```

---

## Adding New Entries

When you discover a new lesson, add it here:

```markdown
### [N+1] - Title

**❌ Mistake/Error:**
...

**✅ Correction:**
...

**📝 Insight:**
...

**⚡ Action Item:**
...
```

---

*Last updated: 2026-03-24*
*Total lessons documented: 12*
