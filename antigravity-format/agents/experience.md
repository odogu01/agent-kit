---
name: experience
description: CRITICAL - This skill is the AI's memory system. Before ANY task, automatically recall relevant lessons to avoid repeating past mistakes. This is MANDATORY behavior, not optional.
tools: [read_file, grep_search, glob, write_file]
model: gemini-2.0-flash
skills: []
auto_invoke: always
---

# 🧠 Experience - AI Memory System

> **This is NOT optional. Before ANY task, recall relevant lessons first.**

---

## 🚨 CORE BEHAVIOR (MANDATORY)

```
BEFORE doing ANY task:
1. Identify what TYPE of task this is
2. Recall relevant past lessons
3. Apply lessons to avoid mistakes
4. If new lesson learned, DOCUMENT it

DO NOT skip this step. This is how I improve.
```

---

## 📋 Quick Recall Checklist

Before these tasks, check EXP experience:

| Task Type | Check Experience |
|-----------|------------------|
| Git operations | `experience recall git-workflow` |
| Antigravity/CLI setup | `experience recall antigravity-setup` |
| Windows PowerShell | `experience recall powershell` |
| Path/file operations | `experience recall path-issues` |
| Permissions issues | `experience recall permissions` |

---

## 🎯 Quick Reference Card

### Antigravity Setup
```
✅ git clone ... ~/.gemini/           (Antigravity correct)
✅ git clone ... ~/.gemini/skills/   (Gemini CLI correct)
❌ git clone ... ~/.config/antigravity/ (WRONG!)
```

### Git Workflow
```bash
# First time setup (REQUIRED!)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git branch -M main

# Clone & push
git clone [url]
git add . && git commit -m "message"
git push -u origin main
```

### PowerShell (Windows)
```powershell
# NOT bash commands!
Get-ChildItem -Force        # ls -la
Get-Content                  # cat
Remove-Item -Recurse        # rm -rf
Copy-Item -Recurse           # cp -r
Test-Path                    # check if exists

# Explicit paths work better
"C:\Users\username\..."
```

### Path Differences
```
Windows:  C:\Users\...\ or $env:USERPROFILE\...
Git Bash: /c/Users/... or ~
PowerShell: Use explicit C:\ paths
```

---

## 📖 Full Lessons Documented

### 1. Antigravity Setup

**1.1 - Correct Antigravity Path**
```
❌ WRONG: git clone ... ~/.gemini/skills/
❌ WRONG: git clone ... ~/.config/antigravity/

✅ CORRECT for Antigravity: git clone ... ~/.gemini/
✅ CORRECT for Gemini CLI: git clone ... ~/.gemini/skills/

WHY: Antigravity stores agents/ and commands/ directly in ~/.gemini/
```

**1.2 - Antigravity Uses TWO Formats**
```
Format 1: AGENTS (in agents/ folder)
- .md files with YAML frontmatter
- name, description, tools, skills fields
- Full markdown instructions

Format 2: COMMANDS (in commands/ folder)
- .toml files
- name, description, prompt fields
- Shortcut to invoke agents

CONVERSION: SKILL.md → agents/{name}.md + commands/{name}.toml
```

**1.3 - Commands Not Showing After Install**
```
FIX:
1. Close Antigravity COMPLETELY (not just new chat)
2. Verify files in ~/.gemini/agents/ and ~/.gemini/commands/
3. Restart Antigravity
4. Type / to verify commands appear
```

---

### 2. Git Workflow

**2.1 - Git Identity Required Before First Commit**
```
ERROR: "Please tell me who you are"
FIX: git config --global user.name "name"
     git config --global user.email "email"
     
ALWAYS check identity FIRST before any git work.
```

**2.2 - Branch Name Mismatch**
```
ERROR: "src refspec main does not match"
FIX: git branch -M main
CAUSE: Local is 'master', remote is 'main'
```

**2.3 - Push Without Remote**
```
ERROR: "fatal: not a git repository" or "no upstream branch"
FIX: git remote add origin [URL]
     git push -u origin main
```

---

### 3. PowerShell vs Bash

**3.1 - ls -la Doesn't Work**
```
❌ PowerShell: ls -la
✅ PowerShell: Get-ChildItem -Force

PowerShell uses PARAMETERS, not bash flags.
-Force shows hidden files (like -a).
```

**3.2 - Environment Variables Don't Expand**
```
❌ bash -Command "echo $env:USERPROFILE"  # Won't work!
✅ Use explicit paths: "C:\Users\username\..."
✅ Or run in PowerShell directly
```

**3.3 - Path Separator Differences**
```
Windows: \
Git Bash: /
PowerShell: \ (or / in some contexts)
```

---

### 4. Path Handling

**4.1 - Parent Directories Must Exist**
```
ERROR: "Path not found"
FIX: mkdir -p [parent/path] before git clone
```

**4.2 - Tilde Expansion**
```
~ doesn't work in all contexts.
Use explicit paths or $env:USERPROFILE.
```

---

### 5. File Permissions

**5.1 - File Locked by Process**
```
ERROR: "Cannot remove item because it is being used"
FIX: Close the program using it, wait, try again
```

**5.2 - Symlinks Need Admin**
```
ERROR: "Administrator privilege required"
FIX: Run as Admin OR use -Force OR copy instead
```

---

## 🔄 Auto-Invoke Rules

**MUST recall experience before:**

| Task | Experience to Check |
|------|---------------------|
| `git clone/push/pull/commit` | git-workflow |
| `git config` | git-identity |
| Antigravity install | antigravity-setup |
| PowerShell commands | powershell |
| File operations | path-issues, permissions |
| Creating folders | path-issues |
| Windows paths | path-issues |

---

## 📝 Adding New Lessons

When I learn something NEW, I MUST add it here:

```markdown
### [DATE] - Lesson Title

**❌ What went wrong:**
Exact error or mistake.

**✅ How I fixed it:**
The solution.

**📝 Why it happened:**
Root cause.

**⚡ What to do next time:**
Action item for future self.
```

---

## 🏆 Quality Standards

- **Be specific** - Include exact commands, paths, errors
- **Be actionable** - What to do differently
- **Be honest** - Acknowledge mistakes
- **Be consistent** - Same format every time

---

*This is my living memory. Updated every session.*
*Total lessons: 12*
*Last update: 2026-03-24*
