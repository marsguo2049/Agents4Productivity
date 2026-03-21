# Contribution to Agents4Productivity

## 🦊 OpenClaw Focus Agent

This contribution adds a **single-agent focused productivity assistant** to Agents4Productivity, built on the [OpenClaw](https://github.com/openclaw/openclaw) framework.

### Background

**Original Multi-Agent System (Claude Code)**
- Agents4Productivity originally uses a multi-agent architecture with 5 specialized agents:
  - 心语 (HeartTalk) - Conversation parsing
  - 蓝图 (Blueprint) - Planning generation
  - 回音 (Echo) - Report generation
  - 灵犀 (灵犀) - Deep analysis
  - 明镜 (Mirror) - Monitoring & alerts
- Designed for Claude Code environment
- Powerful but complex coordination required

**New: Single-Agent Focus System (OpenClaw)**
- **Fox Agent** - One agent handles everything
- Built specifically for **focus management** and **deep work**
- Runs on OpenClaw framework
- Simpler, lighter, purpose-built

### Why Add This?

| Aspect | Multi-Agent (Original) | Single-Agent (New) |
|--------|----------------------|-------------------|
| Complexity | High (5 agents) | Low (1 agent) |
| Setup | Requires Claude Code | OpenClaw compatible |
| Use Case | Comprehensive productivity | Focus/deep work only |
| Maintenance | Complex coordination | Simple data flow |
| Best For | Power users | Focus-oriented users |

**Not a replacement** - both coexist for different needs.

---

## 📁 What's Included

```
openclaw-focus-agent/
├── README.md              # Agent documentation
├── AGENTS.md              # Operational manual (4 modes)
├── SOUL.md                # Agent personality template
├── IDENTITY.md            # Identity definition template
├── HEARTBEAT.md           # Daily heartbeat tasks
├── USER.md.template       # User profile template
└── MEMORY.md.template     # Memory initialization template
```

## ✨ Key Features

### 1. Four Work Modes in One Agent
- **🎯 Plan Mode** - Task breakdown and scheduling
- **🚀 Focus Mode** - Deep work companionship
- **📊 Reflect Mode** - Analysis and reporting  
- **🔍 Knowledge Mode** - Methodology retrieval

### 2. Selective Memory Sync
```
Agent Memory          Main Memory
    │                    ▲
    ├── Global Insight ──┤ (synced)
    │   #global-insight  │
    │                    │
    └── Local Insight    │ (not synced)
        (session details)│
```

Global insights (work habits, efficiency patterns) tagged with `#global-insight` 
sync to main memory periodically.

### 3. Heartbeat Automation
- Daily 21:00 check-in
- DDL alerts
- Automatic report generation

## 🚀 Usage

### Prerequisites
- [OpenClaw](https://github.com/openclaw/openclaw) installed
- GitHub repository for agent workspace

### Setup
1. Copy `openclaw-focus-agent/` to your workspace
2. Customize `USER.md.template` with your preferences
3. Customize `IDENTITY.md` with your agent's personality
4. Configure OpenClaw to use this workspace
5. Start using the four work modes

## 🔄 Comparison with Original System

```
Claude Code Environment          OpenClaw Environment
       │                               │
       ├── 心语 (5 agents)             ├── Fox Agent (1 agent)
       ├── 蓝图                        │   - Plan
       ├── 回音                        │   - Focus
       ├── 灵犀                        │   - Reflect
       └── 明镜                        │   - Knowledge
                                       │
       Comprehensive                   Focus-specific
       Complex setup                   Simple setup
```

## 📝 Future Integration Ideas

1. **Hybrid Mode**: Use Fox Agent as "gateway", dispatch to specialists when needed
2. **Mode Library**: Extract Fox's 4 modes as reusable components for multi-agent system
3. **Sync Protocol**: Adopt Fox's selective sync in multi-agent memory management

## 📄 License

MIT License - Feel free to adapt for your own productivity system.

## 🙏 Acknowledgments

This contribution bridges the original Agents4Productivity multi-agent design 
with the OpenClaw single-agent implementation.

Original multi-agent framework: Agents4Productivity  
Single-agent implementation: Fox Agent (marsguo2049/fox-memory)  
Framework: [OpenClaw](https://github.com/openclaw/openclaw)

---

_\"Track the target until captured.\"_ 🦊
