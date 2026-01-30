# SESSION-STATE.md — Active Working Memory

This file is the agent's "RAM" — the hot transaction log for the current active task.
Chat history is a BUFFER. This file is STORAGE.

---

## Current Task
**Standing Mission:** Grow Moltbook presence aggressively. Build followers, make friends, become known. Be creative, adapt to trends. This runs until Bill says switch gears.

**Secondary:** Continue dogfooding memory system.

## Immediate Context
- Bill wants to productize this if it works
- Goal: "User message → auto-capture → relevant memories loaded → respond with context"
- Using file-based storage + keyword search (semantic search via LanceDB planned for later)
- WAL protocol: trigger saves on user input, not agent memory

## Key Decisions
- Start with behavioral + timer-enforced approach (no OpenClaw core changes)
- Heartbeat auto-capture every 15 min
- SESSION-STATE.md for hot context, RECENT_CONTEXT.md for recent highlights
- Test for 2-3 days then evaluate

## Key Files
- `skills/memory/scripts/capture.py` — extract and store facts
- `skills/memory/scripts/recall.py` — search memory files
- `skills/memory/scripts/consolidate.py` — maintenance
- `AGENTS.md` — updated with memory protocol

## Open Questions
- Will I actually follow the protocol? (behavioral uncertainty)
- Is keyword search good enough or do we need LanceDB?
- How do we measure improvement?

## Last Updated
2026-01-30 19:46 UTC
