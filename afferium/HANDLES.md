# HANDLES.md — Afferium Social Handle Claim Sweep

_Goal: claim `@afferium` (or the closest clean variant) on every platform that matters before anyone else notices the word exists._

## Strategy

- **Claim first, post later.** Empty accounts are fine. We just want the name held.
- **Use a consistent email alias** for all registrations — recommend `handles@afferium.com` (set up via Cloudflare Email Routing forwarding to Coral's real inbox). This keeps the brand inbox separate from personal, and makes recovery easier if any single account is compromised.
- **Bio placeholder** for the initial claim: just the name and the feather 🪶 emoji. More coming.
- **Profile photo placeholder:** black square on cream, or a simple glyph. We'll design real brand visuals later.

## Platforms to sweep

### Priority 1 (do today)

| Platform | Handle target | Status | Notes |
|---|---|---|---|
| X / Twitter | @afferium | ⏳ | High trademark/squatting risk; do first |
| Instagram | @afferium | ⏳ | Same. Meta is slow to help with recovery. |
| GitHub | afferium | ⏳ | For any code the company touches. Also, GH orgs are common reference points. |
| Bluesky | @afferium.bsky.social _(or use afferium.com as handle via DNS)_ | ⏳ | Bluesky supports custom-domain handles — point `_atproto` TXT record at afferium.com, then the handle becomes `@afferium.com`. On-brand. |
| YouTube | @afferium | ⏳ | Claim the channel handle even if no video yet. |

### Priority 2 (this week)

| Platform | Handle target | Status | Notes |
|---|---|---|---|
| Substack | afferium.substack.com | ⏳ | If we ever do a written newsletter |
| Bandcamp | afferium.bandcamp.com | ⏳ | Critical for the album side |
| SoundCloud | @afferium | ⏳ | Same |
| TikTok | @afferium | ⏳ | Don't sleep on this; squatting is rampant |
| Threads | @afferium | ⏳ | Linked to the Instagram claim |
| Mastodon | @afferium@mastodon.social _or self-host_ | ⏳ | Philosophically aligned with the brand's sovereignty story |
| LinkedIn | Afferium (company page) | ⏳ | Lower priority but free to lock |

### Priority 3 (nice to have, only if time)

- Reddit (`u/afferium` — user, and eventually a subreddit)
- Pinterest (brand aesthetic moodboards)
- Vimeo (if we ever publish video work at higher quality than YouTube)
- Patreon (if we ever do paid subscriber tier)
- Ko-fi (same)
- Discord (a public Afferium server, eventually)

## The Bluesky move specifically

Bluesky lets you use any domain you control as your handle, by setting a DNS TXT record. Instead of `@afferium.bsky.social`, Coral can be **@afferium.com** directly. This is:
- On-brand (sovereignty, your own domain is your identity)
- Free
- Easy to set up (one DNS record)
- Transferable (you keep your handle as long as you keep the domain)

**Process:**
1. Register on Bluesky with any temporary handle
2. In Bluesky settings → Advanced → Change handle → I have my own domain
3. Add the TXT record they give you to your DNS (`_atproto.afferium.com`)
4. Verify in Bluesky

This should be one of the first claims.

## Anti-pattern: don't link everything to one recovery email/phone

Spread recovery methods across at least two independent emails and a phone number. If the `handles@afferium.com` inbox is the single point of failure and someone compromises it, every account falls at once.

## Documentation discipline

For each handle claim, record in the status column:
- ✅ = claimed and verified
- ⚠️ = claimed but needs follow-up (e.g., bio not set, photo not uploaded)
- ❌ = taken by someone else (note who, and whether worth contesting)

When Coral finishes a sweep session, edit this file with the results.
