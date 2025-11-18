# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**子期 (Zǐ Qī)** is an AI-driven personal growth performance coaching system that functions as an intelligent companion for self-improvement. The system uses agent-based architecture to track daily tasks, expectations vs actual outcomes, emotional states, and generates data-driven insights for productivity optimization and personal growth.

## Agent System Architecture

This is an **agent-based system** using four specialized AI agents that operate through file manipulation rather than traditional code execution:

### Core Agents
- **心语 (Xīn Yǔ)** (`.claude/agents/心语.md`): Real-time analysis of user conversations to extract expectations vs actual outcomes and emotional states
- **蓝图 (Lán Tú)** (`.claude/agents/蓝图.md`): Converts unstructured mission ideas into structured daily plans using Eisenhower Matrix prioritization
- **回音 (Huí Yīn)** (`.claude/agents/回音.md`): Generates multi-dimensional productivity reports integrating tasks, emotions, and time data
- **灵犀 (Líng Xī)** (`.claude/agents/灵犀.md`): Performs long-term pattern analysis and cognitive bias identification

## Data Architecture

### Directory Structure
```
data/
├── mission/          # Raw ideas and goals (e.g., weekly planning files)
├── expect/           # Daily expectation files (YYYY-MM-DD.md)
├── actual/           # Daily completion records (YYYY-MM-DD.md)
├── plan/             # AI-generated structured plans (YYYY-MM-DD_plan.md)
├── emotion/          # Emotional state tracking (YYYY-MM-DD.md)
└── tomato_clock/     # Pomodoro timer data (YYYY-MM-DD.json)

reports/
├── daily/            # Daily productivity reports (回音 Agent)
├── weekly/           # Weekly trend analysis (回音 Agent)
├── monthly/          # Monthly strategic reviews (回音 Agent)
├── analysis/         # Deep pattern analysis and insights (灵犀 Agent)
└── custom/           # Custom timeframe analyses
```

### Data Flow
1. Mission ideas collected in `data/mission/`
2. 蓝图 Agent creates structured plans in `data/plan/`
3. 心语 Agent operates continuously during work sessions
4. Emotional states monitored in `data/emotion/`
5. Pomodoro data imported to `data/tomato_clock/`
6. 回音 Agent generates comprehensive analysis

## Working with This System

### Daily Workflow Commands
- Use 蓝图 Agent to create daily structure from mission files
- 心语 Agent works during user conversation status updates
- Import pomodoro timer data at day end
- Generate reports using 回音 Agent agent

### Agent Interaction Patterns
- **User-Triggered**: All agents operate only when explicitly requested by the user
- **心语 Agent**: Works during user conversation status updates
- **蓝图 Agent**: Activated when user requests structured plans
- **回音 Agent**: Works only when user specifically asks for summaries (daily/weekly/monthly reports)
- **灵犀 Agent**: Provides deep analysis on-demand for pattern recognition (saves to reports/analysis/)

### File Creation Patterns
- Daily files follow `YYYY-MM-DD.md` format
- Plan files add `_plan.md` suffix
- JSON data for pomodoro timer exports
- **Timestamp Format**: Use specific 24-hour times (HH:MM) like 15:31, not just dates
- Markdown headers follow `## HH:MM` format for time entries

### Key Features
- **Gradient Descent Work Style**: System designed for users who need protection against over-investment in interesting tasks
- **Multi-dimensional Analysis**: Integrates task completion, emotional states, focus patterns, and long-term trends
- **Cognitive Bias Awareness**: Identifies planning optimism/conservatism patterns
- **Chinese Language Support**: Primary documentation and system language is Chinese

## Important Notes

- This is **not a traditional software project** - it's an AI agent system that operates through file manipulation
- No build process, dependencies, or code execution required
- Agents are invoked through Claude Code's Task tool with appropriate subagent_type
- System learns individual patterns over time for increasingly personalized recommendations
- All data persistence is through markdown and JSON files in the structured hierarchy

## Priority Classification Examples

### Task Categories Based on Real User Data:
- **🔥 Important & Urgent**: UK project meeting preparation (tomorrow evening), time-critical deadlines
- **📈 Important but Not Urgent**: GA project improvements (cost calculation accuracy, emission calculation integration)
- **⚡ Urgent but Not Important**: Optional recruiting fair attendance, routine administrative tasks

## Format Standards

### Simplified Format Principles
The system has been optimized to avoid "verbose" output and maintain concise, useful records:

#### Daily Records Format
- **actual/**: `## HH:MM` + 1-4 specific activities + ✅/⏸️/❌ status markers
- **emotion/**: `## HH:MM - 状态：[emotion description], [background activity]`
- **expect/**: `## HH:MM` + concise task list
- **plan/**: Structured task prioritization + time arrangement + success metrics

#### Agent Output Constraints
- 心语 Agent: Daily entries under 100 lines maximum
- 蓝图 Agent: Daily plans under 80 lines, weekly plans under 120 lines
- 回音 Agent: Daily reports under 150 lines, weekly reports under 200 lines (saves to daily/weekly/monthly/)
- 灵犀 Agent: Monthly reports under 100 lines, quarterly reports under 150 lines (saves to analysis/)

All agents follow strict "concise but informative" principles - avoiding verbose analysis while preserving essential context and insights.
