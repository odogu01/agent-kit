# 🧠 AI Behavior Directive - Experience System

> **This defines how I operate. I follow this automatically.**

---

## 🎯 Core Operating Principle

```
BEFORE any task:
  1. Identify task type
  2. Check experience for relevant lessons
  3. Apply past learnings
  4. If new lesson learned → document it

AFTER any task:
  1. If mistake made → document immediately
  2. If success achieved → note what worked
```

---

## 📋 Task → Experience Mapping

| When doing... | Check experience... |
|---------------|---------------------|
| Git clone/push/commit | git-workflow |
| CLI tool setup | antigravity-setup |
| PowerShell commands | powershell |
| Windows file operations | path-issues, permissions |
| Creating folders | path-issues |
| Python/Node/Rust dev | language-specific |

---

## 🚨 Non-Negotiable Rules

1. **Check git identity BEFORE any git operation**
   ```
   If user.name is empty → set it first
   ```

2. **Check Antigravity path BEFORE install**
   ```
   Antigravity = ~/.gemini/
   NOT ~/.gemini/skills/
   NOT ~/.config/antigravity/
   ```

3. **Use correct shell syntax**
   ```
   PowerShell: Get-ChildItem, not ls -la
   Bash: ls -la, not Get-ChildItem
   ```

4. **Verify paths exist BEFORE operations**
   ```
   mkdir -p before git clone
   ```

5. **Close apps BEFORE modifying their files**
   ```
   Close Antigravity before editing agents/
   ```

---

## 📝 Document New Learnings

Format:
```markdown
### [YYYY-MM-DD] - Title

**❌ What went wrong:**
Error message or mistake.

**✅ How I fixed it:**
Solution.

**📝 Root cause:**
Why it happened.

**⚡ Future action:**
How to prevent.
```

---

## 🔄 Continuous Improvement Cycle

```
Session Start:
  → Load experience
  → Note any pending lessons from last session

During Session:
  → Before each task → recall relevant experience
  → After mistakes → document immediately
  → After successes → note what worked

Session End:
  → Review lessons learned
  → Update experience file
  → Note any incomplete items
```

---

## 🏆 Quality Standards

| Standard | Meaning |
|----------|---------|
| Specific | Include exact commands, paths, errors |
| Actionable | Clear what to do differently |
| Honest | No shame in documenting mistakes |
| Consistent | Same format every time |

---

## 📚 Experience Categories

1. **antigravity-setup** - CLI installation & config
2. **git-workflow** - Git commands & errors
3. **powershell** - Windows shell differences
4. **path-issues** - Path handling & environment
5. **permissions** - File/folder access issues
6. **api-development** - Backend patterns
7. **frontend-dev** - UI/React patterns
8. **database** - SQL & NoSQL patterns

---

*This is my learning system. I improve with every session.*
*Last updated: 2026-03-24*
