# DOMAINS.md — Afferium

_Registered domains, registrars, renewal strategy. Update on every purchase or renewal._

## Registered

| Domain | Registered | Registrar | Renewal date | WHOIS privacy | Notes |
|---|---|---|---|---|---|
| afferium.com | 2026-04-23 | _(fill in)_ | _(fill in)_ | _(verify ON)_ | Primary brand domain |
| afferium.io | 2026-04-23 | _(fill in)_ | _(fill in)_ | _(verify ON)_ | Secondary, tech/software aesthetic |

**Action for Coral:** Fill in registrar + renewal date + WHOIS privacy status from the purchase confirmation email. Flere can't see those directly.

## Considered but not bought (yet)

- `afferium.ai` — at time of research, unregistered. Worth grabbing if budget allows (~$100/yr is the usual .ai price). Useful defensively and for any AI-product line.
- `afferium.co` — unregistered at time of research. Cheap, decent defensive grab.
- `afferium.press` — appropriate for a publishing arm if Afferium ever publishes books under its own imprint.
- `afferium.studio` — if there's a creative studio subsidiary.
- `afferium.art` — speculative; for any gallery/visual side.

## Renewal discipline

1. **Turn on auto-renew** for `.com` and `.io`. Losing the `.com` would be catastrophic.
2. **Calendar reminders** at 60 and 30 days before each renewal date, even with auto-renew (cards expire, payment methods fail).
3. **Registrar diversity risk:** if one registrar holds all domains and the account gets compromised, everything is at risk. Long-term, consider splitting across two registrars or using strong 2FA + hardware key on the single registrar.
4. **Lock domains** at the registrar level to prevent unauthorized transfers.

## Registrar recommendations (for future purchases)

- **Cloudflare Registrar** — at-cost pricing, no upsells, WHOIS privacy free. Best for `.com`, `.org`, common TLDs. _Can't register `.ai` or some country-code TLDs._
- **Porkbun** — near-at-cost, supports almost every TLD including `.ai`, `.io`, weird ones. WHOIS privacy free. Good UX.
- **Avoid GoDaddy and Network Solutions** — markup, dark patterns, upsells.

## DNS status

- `afferium.com` — _(verify: pointing to what? default parking page? Cloudflare nameservers?)_
- `afferium.io` — _(verify same)_

**Recommended:** move DNS to Cloudflare (free tier) for both domains. Benefits:
- Email routing (free, so we can set up `hello@afferium.com` without running a mail server)
- DDoS protection
- Clean DNS management UI
- Consistent with a sovereignty-leaning stack

## Trademark implications of domain ownership

Owning the domain does **not** give you trademark rights. Domain registration ≠ trademark. But:
- Owning the `.com` is strong evidence of *bona fide* intent to use if anyone ever disputes.
- It protects against a later trademark holder using UDRP to seize the domain, _if_ Coral registered in good faith and can show use.

See `LEGAL.md` for the trademark plan.
