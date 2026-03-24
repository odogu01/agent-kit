# 🧰 Agent Kit - Universal Agent Skills Collection

> A comprehensive collection of **38 specialized skills** for AI coding agents. Now with ** Antigravity Agent Format** - 35 agents + 36 commands ready to use!

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Total Skills](https://img.shields.io/badge/agents-35-green.svg)](#-antigravity-agents)
[![Total Commands](https://img.shields.io/badge/commands-36-blue.svg)](#-antigravity-commands)

---

## 🎯 Quick Install (Choose Your CLI)

### One-Line Commands by CLI Tool

| CLI Tool | Quick Install |
|----------|---------------|
| **OpenCode** | `git clone https://github.com/odogu01/agent-kit.git ~/.config/opencode/skills` |
| **Claude Desktop** | `git clone https://github.com/odogu01/agent-kit.git ~/.claude/skills` |
| **Gemini CLI** | `git clone https://github.com/odogu01/agent-kit.git ~/.gemini/skills` |
| **Antigravity** | `git clone https://github.com/odogu01/agent-kit.git ~/.gemini` |
| **VS Code (Cline)** | See [VS Code / Cline](#vs-code--cline) section |
| **Cursor** | `git clone https://github.com/odogu01/agent-kit.git ~/.cursor/skills` |
| **Windsurf** | `git clone https://github.com/odogu01/agent-kit.git ~/.windsurf/skills` |

---

## ⚡ Antigravity Quick Start (Recommended!)

Antigravity uses **agents** (`.md` files) and **commands** (`.toml` files).

### Install for Antigravity

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.gemini

# Windows (PowerShell)
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.gemini"
```

This will install:
- **35 agent files** → `~/.gemini/agents/`
- **36 command files** → `~/.gemini/commands/`

### Use in Antigravity

After installation, **restart Antigravity** and type `/` to see all available commands:

```
/react-expert          # React/Next.js optimization
/nodejs-expert        # Node.js development
/python-expert        # Python development
/rust-expert          # Advanced Rust
/api-designer         # API design
/database-architect   # Database design
/game-developer       # Game development
/clean-coder          # Clean code principles
/frontend-designer    # UI design
/mobile-designer      # Mobile design
/architect            # Software architecture
/project-planner      # Project planning
/brainstormer         # Requirements clarification
/debugger             # Debugging methodology
/tdd-expert          # Test-driven development
/cloud-architect      # Cloud architecture
/system-designer      # Distributed systems
/mcp-builder          # MCP server building
/web-designer         # Web accessibility
/security-auditor     # Security review
/penetration-tester  # Security testing
/test-engineer        # Testing strategies
/performance-optimizer # Performance optimization
/seo-specialist       # SEO optimization
/devops-engineer      # DevOps & deployment
/orchestrate          # Multi-agent coordination
/plan                 # Create project plans
/create               # Build projects
/test                 # Testing workflows
/debug                # Debug workflows
/deploy               # Deployment workflows
/enhance              # Code enhancement
/preview              # Preview workflows
/status               # Project status
```

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

---

### 2. Claude Desktop (claude-code)

**Location:** `~/.claude/skills/`

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.claude/skills

# Windows
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.claude\skills"
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

---

### 4. Antigravity ⚡ (RECOMMENDED)

**Location:** `~/.gemini/` (agents & commands folders)

```bash
# Linux / macOS
git clone https://github.com/odogu01/agent-kit.git ~/.gemini

# Windows (PowerShell)
git clone https://github.com/odogu01/agent-kit.git "$env:USERPROFILE\.gemini"
```

**What gets installed:**
```
~/.gemini/
├── agents/           # 35 agent files (.md)
│   ├── react-expert.md
│   ├── nodejs-expert.md
│   ├── python-expert.md
│   ├── architect.md
│   ├── debugger.md
│   └── ... (30 more)
└── commands/         # 36 command files (.toml)
    ├── react-expert.toml
    ├── nodejs-expert.toml
    ├── brainstormer.toml
    └── ... (33 more)
```

**Then restart Antigravity and use `/` commands!**

---

### 5. VS Code (Cline / Continue / Roo Code)

#### Cline
**Location:** `~/.cline/skills/`

```bash
git clone https://github.com/odogu01/agent-kit.git ~/.cline/skills
```

#### Continue
**Location:** `~/.continue/skills/`

```bash
git clone https://github.com/odogu01/agent-kit.git ~/.continue/skills
```

#### Roo Code
**Location:** `~/.roo/skills/`

```bash
git clone https://github.com/odogu01/agent-kit.git ~/.roo/skills
```

---

### 6. Cursor

**Location:** `~/.cursor/skills/`

```bash
git clone https://github.com/odogu01/agent-kit.git ~/.cursor/skills
```

---

### 7. Windsurf (Codeium)

**Location:** `~/.windsurf/skills/`

```bash
git clone https://github.com/odogu01/agent-kit.git ~/.windsurf/skills
```

---

## 🤖 Antigravity Agents (35)

| Agent | Description |
|-------|-------------|
| `react-expert` | React/Next.js performance optimization |
| `nodejs-expert` | Node.js development principles |
| `python-expert` | Python development patterns |
| `rust-expert` | Advanced Rust 1.75+ with async |
| `api-designer` | REST/GraphQL/tRPC design |
| `database-architect` | Schema, indexing, ORM selection |
| `game-developer` | Game dev orchestrator |
| `clean-coder` | Pragmatic coding standards |
| `frontend-designer` | UI design thinking |
| `mobile-designer` | Mobile-first design |
| `architect` | Software architecture decisions |
| `cloud-architect` | AWS/GCP/Azure services |
| `system-designer` | Distributed systems design |
| `project-planner` | Task breakdowns, milestones |
| `brainstormer` | Socratic questioning |
| `debugger` | Root cause analysis |
| `tdd-expert` | Test-driven development |
| `test-engineer` | Unit, integration, E2E |
| `security-auditor` | OWASP Top 10 |
| `penetration-tester` | Red team tactics |
| `performance-optimizer` | Profiling, optimization |
| `seo-specialist` | Core Web Vitals |
| `devops-engineer` | CI/CD, deployment |
| `web-designer` | WCAG accessibility |
| `mcp-builder` | MCP server building |
| `orchestrator` | Multi-agent coordination |
| `frontend-specialist` | Full frontend guidance |
| `backend-specialist` | Full backend guidance |
| `mobile-developer` | React Native, Flutter |
| `explorer-agent` | Codebase exploration |
| `product-manager` | Product strategy |
| `product-owner` | Agile practices |
| `code-archaeologist` | Legacy code analysis |
| `documentation-writer` | Tech writing |
| `qa-automation-engineer` | Test automation |

---

## 📋 Antigravity Commands (36)

| Command | Trigger | Description |
|---------|---------|-------------|
| `/react-expert` | React optimization | React/Next.js advice |
| `/nodejs-expert` | Node.js help | Node.js best practices |
| `/python-expert` | Python help | Python patterns |
| `/rust-expert` | Rust help | Advanced Rust |
| `/api-designer` | API design | REST/GraphQL/tRPC |
| `/database-architect` | DB design | Schema, indexing |
| `/game-developer` | Game dev | Any platform |
| `/clean-coder` | Code quality | Clean code |
| `/frontend-designer` | UI design | Components |
| `/mobile-designer` | Mobile design | iOS/Android |
| `/architect` | Architecture | System design |
| `/cloud-architect` | Cloud setup | AWS/GCP/Azure |
| `/system-designer` | Systems | Distributed |
| `/project-planner` | Planning | Task breakdown |
| `/brainstormer` | Clarify | Requirements |
| `/debugger` | Debug | Root cause |
| `/tdd-expert` | TDD | Test-first |
| `/test-engineer` | Testing | Test strategy |
| `/security-auditor` | Security | Vulnerability scan |
| `/penetration-tester` | Pentest | Attack simulation |
| `/performance-optimizer` | Speed | Optimization |
| `/seo-specialist` | SEO | Search ranking |
| `/devops-engineer` | DevOps | CI/CD |
| `/web-designer` | Accessibility | WCAG |
| `/mcp-builder` | MCP | Server building |
| `/orchestrate` | Multi-agent | Coordination |
| `/plan` | Planning | Create plans |
| `/create` | Build | Generate code |
| `/test` | Testing | Test workflows |
| `/debug` | Debug | Debug workflows |
| `/deploy` | Deploy | Deployment |
| `/enhance` | Improve | Code enhancement |
| `/preview` | Preview | Preview mode |
| `/status` | Status | Project status |
| `/ui-ux-pro-max` | UI/UX | Full design |
| `/ brainstorm` | Brainstorm | Ideation |

---

## 🌐 Automated Setup Scripts

### Linux / macOS (Bash/Zsh)

```bash
#!/bin/bash
CLI_TOOL=${1:-antigravity}

case $CLI_TOOL in
  antigravity)
    DEST=~/.gemini;;
  opencode)
    DEST=~/.config/opencode/skills;;
  claude)
    DEST=~/.claude/skills;;
  cursor)
    DEST=~/.cursor/skills;;
  windsurf)
    DEST=~/.windsurf/skills;;
  *)
    echo "Unknown CLI: $CLI_TOOL"
    exit 1;;
esac

git clone https://github.com/odogu01/agent-kit.git "$DEST"
echo "✅ Agent Kit installed to $DEST"
```

**Usage:**
```bash
chmod +x install-agent-kit.sh
./install-agent-kit.sh antigravity   # Recommended!
./install-agent-kit.sh opencode
```

---

### Windows (PowerShell)

```powershell
param([string]$CLI = "antigravity")

$dest = switch ($CLI) {
    "antigravity" { "$env:USERPROFILE\.gemini" }
    "opencode"    { "$env:USERPROFILE\.config\opencode\skills" }
    "claude"      { "$env:USERPROFILE\.claude\skills" }
    "cursor"      { "$env:USERPROFILE\.cursor\skills" }
    "windsurf"    { "$env:USERPROFILE\.windsurf\skills" }
}

git clone https://github.com/odogu01/agent-kit.git "$dest"
Write-Host "✅ Agent Kit installed to $dest"
```

**Usage:**
```powershell
.\Install-AgentKit.ps1 -CLI antigravity   # Recommended!
.\Install-AgentKit.ps1 -CLI opencode
```

---

## 🔄 Updating Your Kit

```bash
# Navigate to your folder
cd ~/.gemini          # Antigravity
cd ~/.config/opencode/skills  # OpenCode

# Pull latest changes
git pull origin main
```

---

## ❓ Troubleshooting

### Antigravity commands not showing?
1. Make sure you cloned to `~/.gemini/` (not `~/.gemini/skills/`)
2. Restart Antigravity completely
3. Type `/` to see available commands

### "Path not found"
```bash
mkdir -p ~/.gemini
git clone https://github.com/odogu01/agent-kit.git ~/.gemini
```

### Permission denied
```bash
chmod +x install-agent-kit.sh
```

---

## 📄 License

MIT License - Use, modify, and share freely!

---

## 🙏 Credits

Built with ❤️ by [odogu01](https://github.com/odogu01)

[![GitHub Stars](https://img.shields.io/github/stars/odogu01/agent-kit?style=social)](https://github.com/odogu01/agent-kit)

---

**⭐ Star this repo if it helped you!**
