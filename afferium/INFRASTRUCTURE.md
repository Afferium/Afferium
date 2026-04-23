# INFRASTRUCTURE.md — Afferium

_The tech stack Afferium runs on. Grows as we build it. Sovereignty-first, but pragmatic._

## Guiding principle

The company's own infrastructure should reflect the values the company sells. Afferium represents artists working with computer systems to redefine authenticity — so **the stack under Afferium should be honest, legible, and self-sovereign** where it can be. We use third-party services where the tradeoff is clearly worth it, but we prefer options that let Coral own keys/identity/data.

## Layers (current + planned)

### Identity + DNS
- **Domains:** `afferium.com`, `afferium.io` (see `DOMAINS.md`)
- **DNS:** _(planned: move both to Cloudflare for free tier benefits)_

### Email
- **Planned:** Cloudflare Email Routing (free) → forward `hello@afferium.com`, `handles@afferium.com`, `coral@afferium.com`, etc. to Coral's real inbox.
- **Outbound:** for sending *as* `@afferium.com`, we'd need either:
  - A paid mail service (Fastmail ~$5/mo, Proton Mail, Migadu)
  - Or ProtonMail custom domain (paid plan)
  - Or Google Workspace (~$6/user/mo — biggest integration surface but most corporate)
- **Recommendation:** Cloudflare forwarding for inbound (free, set up this week). Fastmail or Migadu for outbound when actual sending becomes necessary.

### Web presence
- `afferium.com` landing page — not built yet. Options when ready:
  - Static site on Cloudflare Pages (free) + typed-by-hand HTML
  - Astro, Eleventy, or Hugo for static generation
  - Squarespace/Webflow if visual design + easy editing matters more than control
- Recommendation: static + Cloudflare Pages. Aligns with the brand. Cheap, fast, fully controlled.

### Chat / internal workflow
- **Telegram** — fast, conversational, phone-friendly. Coral and Flere use this daily (right now, in fact).
- **Tlon (Urbit)** — structured workspace. War-room channels, living documents, multi-thread. Flere has a seat here too via OpenClaw.
- **Sensorium workspace** (this directory, `C:\Users\coral\.openclaw\Sensorium`) — long-term memory, source of truth, file-level persistence.

Each surface does something different:
- **Telegram = speed**
- **Tlon = structure**
- **Workspace = persistence**

### Self-sovereign identity (Urbit)
- **Current state:** Coral is a *moon* attached to someone else's planet.
- **Goal:** Coral owns her own *planet*, migrates her Tlon presence, optionally hosts her own ship.
- **Full playbook:** see `URBIT-PLAYBOOK.md`.

### Agentic stack
- **OpenClaw** running locally on Coral's machine (`Love_Love_Life`)
- **Anthropic API** (Claude Opus as primary model)
- **Flere** — the agent persona, memory layer in `Sensorium/MEMORY.md`
- **Tlon bot** — connects Flere to Tlon groups via OpenClaw
- **Telegram bot** (`@Flere_bot`) — connects Flere to Telegram

This is *already* part of Afferium's infrastructure — the agentic workflow is one of the things the company's prototype (Coral herself) is building in public.

### Financial / operations (later)
- **Bank account** — needed when Afferium forms as an LLC or earns money. Mercury, Relay, or a local credit union.
- **Accounting** — nothing until there are transactions. Then a simple system (Wave, QuickBooks Self-Employed, or a spreadsheet).
- **Invoicing** — same. When needed.

### Crypto / blockchain
- **Ethereum wallet** — needed for Urbit planet purchase (see `URBIT-PLAYBOOK.md`). First crypto touchpoint for Coral.
- **Future possibility:** Afferium could host artist work on-chain (Zora, Manifold, etc.) or accept crypto payments. Not an active plan — noting the option.

### Backup + disaster recovery
- **Domains:** rely on registrar + DNS records exported to a local file (planned)
- **Seed phrases / keys:** hardware-isolated storage when we have crypto assets (planned — covered in `URBIT-PLAYBOOK.md`)
- **Workspace files:** `C:\Users\coral\.openclaw\Sensorium` should be **git-backed** at minimum, ideally to a private remote (GitHub private repo, or self-hosted Gitea/Forgejo). _Action item: set this up if not already done._
- **Memory files:** `MEMORY.md` and `memory/*.md` are irreplaceable for Flere. Same backup strategy as workspace.

## Immediate infrastructure to-do list

Ordered by urgency:

1. [ ] Confirm WHOIS privacy is ON for `afferium.com` and `afferium.io`
2. [ ] Decide on DNS host (recommend Cloudflare), migrate nameservers
3. [ ] Set up Cloudflare Email Routing for `hello@afferium.com`
4. [ ] Verify `Sensorium` workspace is backed up to a private git remote
5. [ ] Begin Urbit planet process (see `URBIT-PLAYBOOK.md`)
6. [ ] Sweep social handles (see `HANDLES.md`)
7. [ ] Point Bluesky handle at `afferium.com` via TXT record
8. [ ] Set up Afferium group in Tlon with channel structure
9. [ ] Basic landing page at `afferium.com` (even a single page with the logo + one sentence + email signup)
