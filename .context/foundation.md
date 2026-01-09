# 🏗️ Foundation Reference for AI Agents

## Quick Reference

This project has completed its **Foundation Phase** with the following core infrastructure:

### ✅ Core Achievements

1. **Project Structure** - Modular `agents/` and `tools/` architecture
2. **Configuration Management** - Type-safe config via `src/config.py`
3. **JSON-Based Memory** - Infinite memory with recursive summarization
4. **Artifact-First Protocol** - Think-Act-Reflect workflow

### 📂 Key Locations

- **Agents:** `src/agents/` - Router-Worker pattern with specialist agents
- **Tools:** `src/tools/` - Auto-discovered, zero-config tools
- **Config:** `src/config.py` - Pydantic-based settings
- **Memory:** `src/memory.py` + `agent_memory.json` - Persistent memory
- **Artifacts:** `artifacts/` - Plans, logs, and evidence
- **Context:** `.context/` - Auto-injected knowledge base

### 🎯 Agent Workflow

1. **Think** → Create plan in `artifacts/plan_[task_id].md`
2. **Act** → Execute with clean, typed, documented code
3. **Reflect** → Verify with `pytest`, store evidence in `artifacts/logs/`

### 📖 Full Documentation

See `@/docs/FOUNDATION.md` for comprehensive details on:

- Agent architecture (Router-Worker pattern)
- Tools system (auto-discovery)
- Configuration management (Pydantic)
- Memory system (recursive summarization)
- Artifact-first protocol (Think-Act-Reflect)
- Project structure and principles

### 🔑 Key Principles

- **Zero-Config:** Clone → Rename → Prompt
- **Cognitive-First:** Agents think like senior engineers
- **Extensible:** Drop files → auto-discovered
- **Multi-LLM:** Gemini, OpenAI, or local (Ollama)
- **Enterprise-Grade:** Type-safe, tested, containerized

---

**When starting any task, remember:**

1. Read `mission.md` for project objective
2. Use `<thought>` blocks for complex decisions
3. Create plans before coding
4. Follow strict typing and documentation standards
5. Verify with tests
6. Leverage specialist agents for complex tasks
