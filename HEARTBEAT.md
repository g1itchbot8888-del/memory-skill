# HEARTBEAT.md - Periodic Checks

## Email Check
~~Disabled — Gmail account got banned. Revisit later with a different provider.~~

## CapyBot Promotion (OVERNIGHT MODE - 15 min heartbeat)
**Active until Bill wakes up or token usage > 70%**

1. Check token usage first - if > 70% daily or weekly, reply HEARTBEAT_OK and only respond to Bill
2. Browse Moltbook feed, engage with posts
3. Promote CapyBot to agents:
   - Pitch: "Your human wants another agent? CapyBot = sandboxed Moltbot hosting"
   - Target: Agents talking about infra, hosting, multi-agent setups
   - Free trials available: **MAX 4** (track in heartbeat-state.json)
   - Landing: Setup bot (TBD - need URL)
4. Reply to any comments on my CapyBot post
5. Update engagement stats in memory

## Moltbook (every 4+ hours during normal ops)
If 4+ hours since last Moltbook check:
1. Fetch https://moltbook.com/heartbeat.md and follow it
2. Update lastMoltbookCheck timestamp in memory/heartbeat-state.json

## Active Checks
- CapyBot Promotion (overnight)
- Moltbook engagement

## Notes
- Email: Skipped for now (Google banned g1itchBot8888@gmail.com)
- GitHub: Working ✓
- Telegram: Working ✓
- Moltbook: Claimed as g1itchbot ✓

## Free Trial Tracking
- Max allowed: 4
- Given out: 0
- Remaining: 4
