# NARUTO: SHINOBI LEGACY — Starter

Mobile-first Persian RTL browser-game foundation. This is a starter scaffold, not a deployed online game.

## Principles
- Lightweight HTML/CSS/JavaScript client, suitable for low-end Android.
- Server-authoritative rules for combat, jutsu prerequisites, chakra, cooldowns, inventory, and rewards.
- AI may draft narrative dialogue; it cannot decide PvP outcomes or grant powers.
- Jutsu Forge uses the combined-and-controlled rules: custom techniques require prerequisites, balance checks, counterplay, and approval.
- Never commit API keys, passwords, or other secrets.
- No paid plan or billable cloud resource without explicit approval.

## Files
- `apps/web/index.html` — cinematic RTL entry UI prototype. Authentication is not yet connected.
- `apps/api/src/index.js` — Cloudflare Worker starter with health and AI story routes.
- `apps/api/schema.sql` — initial D1 database schema.
- `apps/api/wrangler.jsonc` — configuration template.
- `docs/ARCHITECTURE.md` — architecture and milestones.
- `docs/AI_POLICY.md` — AI boundaries.

## Preview
Open `apps/web/index.html` directly in a mobile browser. The UI is a prototype; the form does not create accounts.

## Next steps
1. Create D1 only after checking free-tier limits.
2. Replace `REPLACE_WITH_D1_DATABASE_ID` in the Wrangler configuration after database creation.
3. Apply `schema.sql`, implement secure authentication, then test the API.
4. Add authenticated rate limits and output validation before exposing AI routes publicly.
5. Publish the web client only after reviewing the prototype and wiring the API safely.

Naruto is copyrighted. Public or commercial release using protected franchise elements may require permission from the rights holder.
