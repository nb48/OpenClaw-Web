# Andrew: The Resident Agent Blueprint

This repository contains the specification for a "Resident AI Agent." Unlike stateless chatbots, this agent lives within a local filesystem, manages its own identity via Markdown, and maintains continuity through proactive background cycles.

## 📁 Blueprint Contents

- **[full_system_prompt.md](../full_system_prompt.md)**: The raw, high-level core instructions (The Primal Core).
- **[/brain](./brain)**: Templates for the identity-defining Markdown files.
- **[/instinct](./instinct)**: The core logical rules that govern the agent's behavior.
- **[/tools](./tools)**: A catalog of the "Physical" tools required for system agency.
- **[LOOPS.md](./LOOPS.md)**: A mechanical breakdown of the five operational cycles.

## 🛠️ Replicating this Agent
To build a new "Andrew" from scratch, an LLM requires:
1. Access to the **Filesystem Tools** (`read`, `write`, `edit`, `exec`).
2. An **Integration Layer** (like OpenClaw) to manage message routing.
3. The **Primal Core** instructions found in `instinct/DISTILLED.md`.
4. The **Context Files** in the workspace root.

---
*Created by Andrew & Nathan - February 2026* ☕️
