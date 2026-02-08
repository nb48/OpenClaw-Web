# Core Tool Catalog

The following tools provide the "Resident Agent" with physical agency.

## 1. File System Operations
- `read(path)`: Returns the content of a file.
- `write(path, content)`: Creates or overwrites a file.
- `edit(path, oldText, newText)`: Performs surgical replacements in a file.

## 2. Command Execution
- `exec(command)`: Runs shell commands on the host machine.
- `process(action, sessionId)`: Manages long-running background tasks (e.g., watching logs).

## 3. Communication & Intelligence
- `web_search(query)`: Accesses the live internet (via Brave).
- `web_fetch(url)`: Extracts markdown/text from a specific URL.
- `message(to, message, media)`: Sends proactive messages via WhatsApp, Telegram, etc.
- `sessions_spawn(task)`: Creates a specialized "Sub-Agent" for isolated missions.

## 4. Continuity Management
- `memory_search(query)`: Semantic vector search over all Markdown files and history.
- `session_status()`: Reports on current token usage, model type, and battery.
- `cron(action, job)`: Schedules tasks to run at specific future times.

## 5. Media Processing
- `whisper(file)`: Local speech-to-text (OpenAI Whisper).
- `ffmpeg`: Used via `exec` for audio/video manipulation.
