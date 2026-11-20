# Cheese 🧀 - Multi-Role AI Companion for CS Students

Cheese is an adaptive AI mentor designed specifically for Computer Science students, combining three distinct personas:
1. **Programming Tutor:** Socratic debugging, variable tracing, mental models, and first-principles reasoning.
2. **Personal Coach:** Milestone decomposition, task pacing, procrastination resistance, and sustainable engineering habits.
3. **Research Agent:** Architectural comparisons, trade-off matrices, and documentation synthesis.

---

## Repository Structure

```
.
├── README.md
├── config/
│   └── agent_manifest.json          # Agent metadata, roles, and default inference settings
├── prompts/
│   ├── cheese_v1.md                 # Base v1 system prompt
│   ├── cheese_v2_optimized.md       # Optimized v2 prompt (strict scaffolding ladder)
│   └── roles/
│       ├── tutor_module.md          # Dedicated Tutor behavior & Socratic ladder
│       ├── coach_module.md          # Dedicated Coach behavior & task slicing
│       └── research_module.md       # Dedicated Research behavior & comparison format
└── tests/
    └── test_scenarios.md            # Interactive benchmarks across all three roles
```

---

## Getting Started

### Using with Antigravity / Agent Interfaces
1. Copy the system prompt from [cheese_v2_optimized.md](file:///C:/Users/chuom/.gemini/antigravity/scratch/cheesemodel/prompts/cheese_v2_optimized.md) into your agent configuration.
2. Set model temperature between `0.3` and `0.4` for balanced pedagogical reasoning and deterministic technical explanations.

### Git Quickstart (Pushing to Remote)
```bash
git init
git remote add origin https://github.com/trgchu/cheesemodel.git
git branch -M main
git add .
git commit -m "feat: initial scaffold for Cheese agent"
git push -u origin main
```
