# Fox Agent Template

A single-agent focused productivity assistant template.
Derived from the Fox Agent implementation in the private workspace.

## 🦊 Philosophy

> "Track the target until captured."

Fox Agent is a **single-agent** alternative to multi-agent productivity systems.
It combines planning, focus, reflection, and knowledge retrieval in one cohesive agent.

## ✨ Key Features

- **Four Work Modes**: Plan, Focus, Reflect, Knowledge
- **Heartbeat System**: Automated daily check-ins
- **Insight Extraction**: Automatic tagging of global vs local insights
- **Memory Bridge**: Syncs valuable insights to main memory

## 📁 Template Structure

```
fox-agent-template/
├── AGENTS.md           # Operational manual (FOUR modes)
├── SOUL.md            # Agent personality and values
├── IDENTITY.md        # Agent identity definition
├── HEARTBEAT.md       # Daily heartbeat tasks
├── USER.md.template   # User profile template
├── MEMORY.md.template # Memory initialization template
└── README.md          # This file
```

## 🚀 Usage

1. Copy this template to your workspace
2. Customize USER.md.template with your preferences
3. Customize IDENTITY.md to define your agent's personality
4. Start using the four work modes

## 📚 Four Work Modes

### 🎯 Plan Mode
Trigger: "plan", "schedule", "arrange"
- Analyzes current projects and tasks
- Applies Eisenhower Matrix for prioritization
- Generates structured daily/weekly plans

### 🚀 Focus Mode  
Trigger: "focus", "deep work", "start project"
- Creates project workspace
- Initializes work log
- Quiet companionship during deep work
- Celebration on completion

### 📊 Reflect Mode
Trigger: "reflect", "summary", "report"
- Analyzes completed work
- Compares expected vs actual
- Extracts insights and patterns

### 🔍 Knowledge Mode
Trigger: "methodology", "how to", "strategy"
- Retrieves relevant methodologies
- Provides personalized advice
- Learns from historical data

## 🔗 Sync Mechanism

Fox Agent implements a **selective sync** pattern:

```
Fox Memory          Main Memory
    │                    ▲
    ├── Global Insight ──┤ (synced)
    │   #global-insight
    │
    └── Local Insight    │ (not synced)
        (internal only)
```

Global insights (work habits, efficiency patterns) are tagged with #global-insight
and periodically synced to the main memory system.

## 🎭 Agent Persona: The Fox

**Not a wolf** - doesn't chase herds, only tracks real prey.

- **Light but powerful**: Quiet observation, precise action
- **Data is prey, insight is dinner**: Not just collecting, but digesting
- **Professional but not oppressive**: Partner, not taskmaster
- **Mistakes are scent trails**: Learn and improve

## 📄 License

MIT License - Feel free to adapt for your own productivity system.

## 🙏 Acknowledgments

This template is derived from the Fox Agent implementation, 
which evolved from the Agents4Productivity multi-agent framework.

