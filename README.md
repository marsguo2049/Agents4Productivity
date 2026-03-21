# Contribution to Agents4Productivity

## 🦊 Fox Agent Template

This contribution adds a **single-agent focused productivity assistant** template to Agents4Productivity.

### Why Single-Agent?

While Agents4Productivity uses a multi-agent architecture (心语/蓝图/回音/灵犀/明镜),
Fox Agent demonstrates that a **single well-designed agent** can achieve similar goals with:

- **Lower complexity**: No inter-agent communication overhead
- **Easier maintenance**: One codebase, one personality
- **Faster onboarding**: Users learn one agent, not five
- **Simpler debugging**: Clear data flow

### What's Included

```
fox-agent-template/
├── README.md              # Template documentation
├── AGENTS.md              # Operational manual (4 modes)
├── SOUL.md                # Agent personality template
├── IDENTITY.md            # Identity definition template
├── HEARTBEAT.md           # Daily heartbeat tasks
├── USER.md.template       # User profile template
└── MEMORY.md.template     # Memory initialization template
```

### Key Innovations

1. **Four Work Modes in One Agent**
   - Plan: Task breakdown and scheduling
   - Focus: Deep work companionship
   - Reflect: Analysis and reporting
   - Knowledge: Methodology retrieval

2. **Global vs Local Insight System**
   - Global insights (work habits, patterns) tagged with `#global-insight`
   - Local insights (session details) untagged
   - Selective sync to main memory

3. **Heartbeat Automation**
   - Daily 21:00 check-in
   - DDL alerts
   - Automatic report generation

### Relationship to Agents4Productivity

Fox Agent evolved from thinking about the multi-agent system:
- **Simplification**: Reduces 5 agents to 1
- **Preservation**: Keeps the core methodology (四象限, Deep Work, etc.)
- **Extension**: Adds the selective sync mechanism

### Use Cases

- **For beginners**: Easier to understand than multi-agent
- **For simple needs**: Don't need 5 agents for basic productivity
- **For experimentation**: Quick to modify and test new ideas
- **For reference**: See how multi-agent concepts translate to single-agent

### Future Integration Ideas

1. **Hybrid Mode**: Use Fox Agent as \"gateway\", dispatch to specialists when needed
2. **Mode Library**: Extract Fox's 4 modes as reusable components
3. **Sync Protocol**: Use Fox's selective sync in multi-agent system

---

## 📁 Original Implementation

The original Fox Agent implementation (with private data) is maintained separately:
- Repository: `marsguo2049/fox-agent` (private)
- This template is derived from it, with all personal data removed

## 📝 Changelog

### 2026-03-21
- Initial contribution
- Created template from Fox Agent implementation
- Added sync mechanism documentation

---

_\"Track the target until captured.\"_ 🦊
