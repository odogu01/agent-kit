# 🧰 Agent Kit - Universal Agent Skills Collection

> A comprehensive collection of **38 specialized skills** for AI coding agents. Compatible with **OpenCode**, **Claude**, **Gemini**, **Antigravity**, **VS Code**, and more.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Total Skills](https://img.shields.io/badge/skills-38-green.svg)](#-skills-overview)
[![Contributors](https://img.shields.io/badge/contributors-welcome-orange.svg)](CONTRIBUTING.md)

---

## 🎯 Quick Install (Choose Your CLI)

### One-Line Commands by CLI Tool

| CLI Tool | Quick Install |
|----------|---------------|
| **OpenCode** | `git clone https://github.com/odogu01/agent-kit.git ~/.config/opencode/skills` |
| **Claude Desktop** | `git clone https://github.com/odogu01/agent-kit.git ~/.claude/skills` |
| **Gemini CLI** | `git clone https://github.com/odogu01/agent-kit.git ~/.gemini/skills` |
| **Antigravity** | `git clone https://github.com/odogu01/agent-kit.git ~/.config/antigravity/skills` |
| **VS Code (Cline)** | See [VS Code / Cline](#vs-code--cline) section |
| **Cursor** | `git clone https://github.com/odogu01/agent-kit.git ~/.cursor/skills` |
| **Windsurf** | `git clone https://github.com/odogu01/agent-kit.git ~/.windsurf/skills` |
| **Jan** | `git clone https://github.com/odogu01/agent-kit.git ~/.jan/skills` |

---

## 📦 Detailed Installation by CLI Tool

### 1. OpenCode

**Location:** `~/.config/opencode/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.config/opencode/skills

# Windows (PowerShell)
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.config\opencode\skills"
```

**Config:** `~/.config/opencode/config.json`
```json
{
  "skills": {
    "path": "~/.config/opencode/skills",
    "enabled": true,
    "autoLoad": true
  }
}
```

---

### 2. Claude Desktop (claude-code)

**Location:** `~/.claude/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.claude/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.claude\skills"
```

**Config:** `~/.claude/settings.json`
```json
{
  "skills": {
    "directory": "~/.claude/skills",
    "enabled": true
  }
}
```

---

### 3. Gemini CLI (Google)

**Location:** `~/.gemini/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.gemini/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.gemini\skills"
```

**Config:** `~/.gemini/config.json`
```json
{
  "skills": {
    "path": "~/.gemini/skills"
  }
}
```

---

### 4. Antigravity

**Location:** `~/.config/antigravity/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.config/antigravity/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.config\antigravity\skills"
```

**Config:** `~/.config/antigravity/config.json`
```json
{
  "skills": {
    "directory": "~/.config/antigravity/skills"
  }
}
```

---

### 5. VS Code (Cline / Continue / Roo Code)

For VS Code extensions, skills are usually stored in the extension's config directory.

#### Cline
**Location:** `~/.cline/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.cline/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.cline\skills"
```

#### Continue
**Location:** `~/.continue/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.continue/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.continue\skills"
```

#### Roo Code
**Location:** `~/.roo/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.roo/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.roo\skills"
```

#### VS Code Settings (settings.json)
```json
{
  "cline.skillsDirectory": "~/.cline/skills",
  "continue.skillsDirectory": "~/.continue/skills"
}
```

---

### 6. Cursor

**Location:** `~/.cursor/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.cursor/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.cursor\skills"
```

**Config:** `~/.cursor/settings.json`
```json
{
  "cursor": {
    "skillsDirectory": "~/.cursor/skills"
  }
}
```

---

### 7. Windsurf (Codeium)

**Location:** `~/.windsurf/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.windsurf/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.windsurf\skills"
```

---

### 8. Jan (Local AI)

**Location:** `~/.jan/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.jan/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.jan\skills"
```

---

### 9. LM Studio

**Location:** `~/.lm-studio/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.lm-studio/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.lm-studio\skills"
```

---

### 10. Ollama (with GUI)

**Location:** `~/.ollama/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.ollama/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.ollama\skills"
```

---

### 11. Other AI CLI Tools

#### Shell AI / Aider
```bash
git clone https://github.com/odogu01/agent-kit.git ~/.aider.skills
```

#### Devin
```bash
git clone https://github.com/odogu01/agent-kit.git ~/.devin/skills
```

#### CodeRabbit
```bash
git clone https://github.com/odogu01/agent-kit.git ~/.coderabbit/skills
```

#### Figote / Goose
```bash
git clone https://github.com/odogu01/agent-kit.git ~/.goose/skills
```

---

## 🌐 Automated Setup Scripts

### Linux / macOS (Bash/Zsh)

Create `install-agent-kit.sh`:

```bash
#!/bin/bash

# Choose your CLI tool
CLI_TOOL=${1:-opencode}

case $CLI_TOOL in
  opencode)
    DEST=~/.config/opencode/skills;;
  claude)
    DEST=~/.claude/skills;;
  gemini)
    DEST=~/.gemini/skills;;
  antigravity)
    DEST=~/.config/antigravity/skills;;
  cursor)
    DEST=~/.cursor/skills;;
  windsurf)
    DEST=~/.windsurf/skills;;
  *)
    echo "Unknown CLI: $CLI_TOOL"
    exit 1;;
esac

# Clone
git clone https://github.com/odogu01/agent-kit.git "$DEST"
echo "✅ Agent Kit installed to $DEST"
```

**Usage:**
```bash
chmod +x install-agent-kit.sh
./install-agent-kit.sh opencode
./install-agent-kit.sh claude
./install-agent-kit.sh antigravity
```

---

### Windows (PowerShell)

Create `Install-AgentKit.ps1`:

```powershell
param(
    [string]$CLI = "opencode"
)

$dest = switch ($CLI) {
    "opencode" { "$env:USERPROFILE\.config\opencode\skills" }
    "claude" { "$env:USERPROFILE\.claude\skills" }
    "gemini" { "$env:USERPROFILE\.gemini\skills" }
    "antigravity" { "$env:USERPROFILE\.config\antigravity\skills" }
    "cursor" { "$env:USERPROFILE\.cursor\skills" }
    "windsurf" { "$env:USERPROFILE\.windsurf\skills" }
    default { throw "Unknown CLI: $CLI" }
}

git clone https://github.com/odogu01/agent-kit.git "$dest"
Write-Host "✅ Agent Kit installed to $dest"
```

**Usage:**
```powershell
.\Install-AgentKit.ps1 -CLI opencode
.\Install-AgentKit.ps1 -CLI antigravity
```

---

## 🔧 Verification

After installation, verify your skills are loaded:

```bash
# Check if skills directory exists and has files
ls -la ~/.config/opencode/skills/  # (adjust for your CLI)

# Should show: api-patterns, app-builder, game-development, etc.
```

---

## 🔄 Updating Your Kit

```bash
# Navigate to your skills folder
cd ~/.config/opencode/skills  # (adjust for your CLI)

# Pull latest changes
git pull origin main
```

Or re-install fresh:
```bash
rm -rf ~/.config/opencode/skills
git clone https://github.com/odogu01/agent-kit.git ~/.config/opencode/skills
```

---

## 📚 Skills Overview (38 Skills)

### 🏗️ Core Development
| Skill | Description |
|-------|-------------|
| `app-builder` | Full-stack app orchestration |
| `plan-writing` | Structured task planning |
| `brainstorming` | Socratic questioning for requirements |
| `clean-code` | Pragmatic coding standards |
| `templates` | 12 project scaffolding templates |

### 🎨 Frontend & Design
| Skill | Description |
|-------|-------------|
| `react-best-practices` | React/Next.js optimization |
| `tailwind-patterns` | Tailwind CSS v4 |
| `frontend-design` | Design thinking for web UI |
| `mobile-design` | Mobile-first design |
| `web-design-guidelines` | Accessibility compliance |

### ⚙️ Backend & Architecture
| Skill | Description |
|-------|-------------|
| `nodejs-best-practices` | Node.js development |
| `python-patterns` | Python patterns |
| `rust-pro` | Advanced Rust 1.75+ |
| `api-patterns` | REST/GraphQL/tRPC design |
| `architecture` | Architectural decisions |

### 🗄️ Database
| Skill | Description |
|-------|-------------|
| `database-design` | Schema, indexing, ORM |

### 🎮 Game Development
| Skill | Description |
|-------|-------------|
| `game-development` | Main orchestrator |
| `game-design` | GDD, balancing |
| `game-art` | Visual style, assets |
| `2d-games` | Sprites, tilemaps |
| `3d-games` | Rendering, shaders |
| `web-games` | WebGPU, PWA |
| `mobile-games` | Touch input, performance |
| `multiplayer` | Networking, sync |
| `vr-ar` | VR/AR development |

### 🔒 Security
| Skill | Description |
|-------|-------------|
| `vulnerability-scanner` | OWASP 2025 |
| `red-team-tactics` | MITRE ATT&CK |

### ✅ Testing & Quality
| Skill | Description |
|-------|-------------|
| `testing-patterns` | Unit, integration, mocking |
| `tdd-workflow` | Test-Driven Development |
| `lint-and-validate` | Static analysis |
| `webapp-testing` | E2E, Playwright |

### 🚀 DevOps & Performance
| Skill | Description |
|-------|-------------|
| `deployment-procedures` | Safe deployment, rollback |
| `server-management` | Process, scaling |
| `performance-profiling` | Measurement, optimization |

### 🌍 Other
| Skill | Description |
|-------|-------------|
| `seo-fundamentals` | Core Web Vitals |
| `i18n-localization` | Translations, RTL |
| `mcp-builder` | MCP server design |
| `parallel-agents` | Multi-agent orchestration |

---

## 🤝 Contributing

Found a new CLI tool or want to add a skill? Contributions welcome!

1. **Fork** the repository
2. **Clone** your fork
3. **Add** your skill or CLI setup guide
4. **Commit** (`git commit -m "Add [CLI] setup"`)
5. **Push** and open a **Pull Request**

---

## ❓ Troubleshooting

### "Permission denied"
```bash
chmod +x install-agent-kit.sh
```

### "Path not found"
Make sure the parent directory exists:
```bash
mkdir -p ~/.config/opencode
git clone https://github.com/odogu01/agent-kit.git ~/.config/opencode/skills
```

### "Skills not loading"
Check your CLI's config file and ensure the skills path is correct.

---

## 📄 License

MIT License - Use, modify, and share freely!

---

## 🙏 Credits

Built with ❤️ by [odogu01](https://github.com/odogu01)

[![GitHub Stars](https://img.shields.io/github/stars/odogu01/agent-kit?style=social)](https://github.com/odogu01/agent-kit)

---

**⭐ Star this repo if it helped you!**
