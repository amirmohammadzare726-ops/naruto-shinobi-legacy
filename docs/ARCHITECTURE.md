# Architecture

## Initial stack
- Client: plain HTML/CSS/JavaScript, Persian RTL, mobile-first.
- API: Cloudflare Workers.
- Database: Cloudflare D1 (SQLite).
- Real-time rooms: consider Durable Objects later, after the first server-authoritative combat prototype.
- AI: Cloudflare Workers AI server-side binding, subject to free quota and model availability.
- Source control: a separate GitHub repository.

## Trust boundaries
The browser is untrusted. It must not decide hit detection, damage, cooldowns, chakra costs, rank, inventory, jutsu ownership, progression, rewards, or PvP results. The server validates requests and derives state from trusted data.

## Milestones
1. Commit the starter files.
2. Create D1 only after confirming free limits and no paid upgrade is required.
3. Apply schema and test `/api/health`.
4. Implement account authentication and secure sessions.
5. Build one playable combat room with server-authoritative movement and jutsu.
6. Add AI story dialogue behind authentication, rate limits, and safe fallback text.
7. Add Jutsu Forge validation and test-only mode.
8. Expand into persistent world, clans, groups, and seasonal story.

## Cost guardrails
Do not create paid resources or change the Cloudflare plan without explicit approval. Keep AI calls out of real-time combat. Use bounded output tokens and static story fallback.
