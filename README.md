# 🧰 Agent Kit - Universal Agent Skills Collection

A comprehensive collection of **38 specialized skills** for AI coding agents. Shareable across multiple CLI tools including **OpenCode**, **Claude**, **Gemini**, and more.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Total Skills](https://img.shields.io/badge/skills-38-green.svg)](#skills-overview)

---

## 🎯 Quick Install

### One-Command Setup

```bash
# Clone the repository
git clone https://github.com/odogu01/agent-kit.git

# Navigate to it
cd agent-kit

# Run the setup script for your CLI tool (see below)
```

---

## 📦 Install for Your CLI Tool

### OpenCode

```bash
# Clone to your opencode skills folder
git clone https://github.com/odogu01/agent-kit.git ~/agent-kit-temp
cp -r ~/agent-kit-temp/* ~/.config/opencode/skills/
rm -rf ~/agent-kit-temp
```

**Windows (PowerShell):**
```powershell
git clone https://github.com/odogu01/agent-kit.git $env:USERPROFILE\agent-kit-temp
Copy-Item "$env:USERPROFILE\agent-kit-temp\*" -Destination "$env:USERPROFILE\.config\opencode\skills" -Recurse -Force
Remove-Item -Path "$env:USERPROFILE\agent-kit-temp" -Recurse -Force
```

---

### Claude (claude-code / Claude Desktop)

```bash
# Clone to claude skills folder
git clone https://github.com/odogu01/agent-kit.git ~/agent-kit-temp
cp -r ~/agent-kit-temp/* ~/.claude/skills/
rm -rf ~/agent-kit-temp
```

**Windows:**
```powershell
git clone https://github.com/odogu01/agent-kit.git $env:USERPROFILE\agent-kit-temp
Copy-Item "$env:USERPROFILE\agent-kit-temp\*" -Destination "$env:USERPROFILE\.claude\skills" -Recurse -Force
Remove-Item -Path "$env:USERPROFILE\agent-kit-temp" -Recurse -Force
```

---

### Gemini CLI (Google)

```bash
# Clone to gemini skills folder
git clone https://github.com/odogu01/agent-kit.git ~/agent-kit-temp
cp -r ~/agent-kit-temp/* ~/.gemini/skills/
rm -rf ~/agent-kit-temp
```

---

### Cursor

```bash
# Clone to cursor config folder
git clone https://github.com/odogu01/agent-kit.git ~/agent-kit-temp
cp -r ~/agent-kit-temp/* ~/.cursor/skills/
rm -rf ~/agent-kit-temp
```

---

### Windsurf (Codeium)

```bash
# Clone to windsurf config folder
git clone https://github.com/odogu01/agent-kit.git ~/agent-kit-temp
cp -r ~/agent-kit-temp/* ~/.windsurf/skills/
rm -rf ~/agent-kit-temp
```

---

### Generic / Custom Setup

```bash
# Clone anywhere
git clone https://github.com/odogu01/agent-kit.git

# Set environment variable (adjust path for your CLI)
export AGENT_SKILLS_PATH=~/agent-kit

# Or copy to custom location
cp -r agent-kit/* /your/custom/skills/path/
```

---

## 🔧 CLI-Specific Configuration

### OpenCode Config

Edit `~/.config/opencode/config.json`:

```json
{
  "skills": {
    "path": "~/.config/opencode/skills",
    "enabled": true
  }
}
```

### Claude Desktop Config

Edit `~/.claude/settings.json`:

```json
{
  "skills": {
    "directory": "~/.claude/skills"
  }
}
```

---

## 📚 Skills Overview

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

---

## 🔄 Update Your Kit

```bash
# Navigate to your skills folder
cd ~/.config/opencode/skills  # (adjust for your CLI)

# Pull latest changes
git pull origin main
```

Or re-clone:

```bash
# Remove old version
rm -rf ~/.config/opencode/skills

# Re-clone
git clone https://github.com/odogu01/agent-kit.git ~/.config/opencode/skills
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-skill`)
3. Add your skill following the `SKILL.md` format
4. Commit changes (`git commit -m "Add amazing-skill"`)
5. Push to your fork (`git push origin feature/amazing-skill`)
6. Open a Pull Request

---

## 📄 License

MIT License - Feel free to use, modify, and share!

---

## 🙏 Credits

Created with ❤️ by [odogu01](https://github.com/odogu01)

---

**Star ⭐ if this kit helped you!**
