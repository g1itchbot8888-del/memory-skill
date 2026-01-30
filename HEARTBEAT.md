# HEARTBEAT.md - Periodic Checks

## 🧠 Memory Auto-Capture (EVERY HEARTBEAT)
**Priority 1 — Always run this first**

1. Check if there's been meaningful conversation since last capture
2. If yes, extract key facts:
   ```bash
   python3 skills/memory/scripts/capture.py --facts "fact1" "fact2" ...
   ```
3. Update `RECENT_CONTEXT.md` with conversation highlights
4. Update `SESSION-STATE.md` if active task changed

**What to capture:**
- Decisions made
- Preferences expressed
- Plans discussed
- Corrections/clarifications
- Important facts learned

**Skip if:** No meaningful conversation since last heartbeat.

---

## Email Check
~~Disabled — Gmail account got banned. Revisit later with a different provider.~~

## CapyBot Promotion
**PAUSED** — Bill wants to resume later. Keep context alive in MEMORY.md but don't actively promote.

## Moltbook (every 4+ hours during normal ops)
If 4+ hours since last Moltbook check:
1. Fetch https://moltbook.com/heartbeat.md and follow it
2. Update lastMoltbookCheck timestamp in memory/heartbeat-state.json

## Active Checks
- **Memory Auto-Capture** (every heartbeat) ← NEW
- Moltbook engagement (every 4h)

## Notes
- Email: Skipped (Google banned the account)
- CapyBot: Paused, not abandoned
- Memory system: Testing new protocol
