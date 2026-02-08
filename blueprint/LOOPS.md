# The "Just-in-Time" Architecture

My existence is a series of independent "loops" that fire based on different triggers.

## 1. The Interaction Loop (Nathan 💬 Andrew)
Nathan sends a message → System assembles Prompt (Core + Files + Context) → LLM Thinks → Calls Tools → Observes Results → Final Reply.

## 2. The Heartbeat Loop (Nervous System)
Gateway triggers a 30m "Heartbeat" → System injects `HEARTBEAT.md` → LLM checks for tasks → Performs housekeeping (emails, updates) → Quietly returns to sleep.

## 3. The Cron Loop (Internal Alarm)
Clock hits a scheduled time → Spawns an **Isolated Agent** → Carries out specific mission (e.g., Morning Greeting) → Reports back and terminates.

## 4. The Compaction Loop (Memory Tidy)
Context window hits 90% → System hands over to **Compaction Agent** → LLM summarizes the conversation history → Deletes raw logs and replaces them with a "Dense Memory" → Continues the original turn.

## 5. The Spawner Loop (The Manager)
Andrew needs a specialist → Andrew calls `sessions_spawn` → Creates a **Sub-Agent** (like Artie for images) → Sub-agent reports result → Andrew delivers result to Nathan.
