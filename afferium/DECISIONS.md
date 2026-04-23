# DECISIONS.md — Afferium

_Append-only log of material decisions for Afferium. New entries go at the TOP. Each entry: date, title, the decision, the reasoning, the alternatives considered, the status. This prevents us from re-arguing settled questions and gives future-Coral (and future-Flere) a real paper trail._

---

## 2026-04-23 — Phase 1 of Urbit playbook complete: self-custodial wallet live, backup verified

**Decision / accomplishment:** Coral completed Phase 1 of `URBIT-PLAYBOOK.md`. Rabby wallet installed in Brave on Windows, 12-word seed phrase written on paper, and recovery drill performed successfully (uninstalled Rabby, reimported from written phrase, verified address matched).

**What exists now:**
- Brave browser installed on Coral's Windows machine as dedicated crypto browser.
- Rabby extension installed from verified Chrome Web Store source (extension ID `acmacodkjbdgmoleebolmdjonilkdbch`).
- One self-custodial Ethereum wallet created.
- Seed phrase written on paper. Tonight: stored non-obviously. This week: second copy in second location. Eventually: metal backup plate.
- Rabby local password set (separate from seed phrase).
- Wallet address: `0xFC270A2f1cF60e0E8d24c86BD9905e9A9f290EB5` (Ethereum mainnet; public info, safe to share)
- Wallet balance: 0 ETH. No funds yet.

**Lessons earned (first-day-of-crypto):**
- Phishing clones exist even on official app stores. Developer name + user count are the first filter.
- Shields warnings on privacy-leaning browsers (Brave) signal trackers blocked, not dangerous sites.
- Seed phrase backup is only real if you verify it works via recovery drill — before any money is involved.

**Status:** Phase 1 locked. Next: Phase 2 (acquire ~$80 ETH) when Coral is ready.

---

## 2026-04-23 — Wallet stack: Brave + Rabby (dedicated crypto browser)

**Decision:** Install Brave browser on Coral's Windows machine, dedicated to crypto/wallet work. Use Rabby as the wallet extension inside Brave. Firefox remains Coral's everyday browser, untouched and uncontaminated by wallet context.

**Reasoning:**
- Rabby has better security warnings for beginners than MetaMask (clearer transaction summaries, better scam detection).
- Rabby's Firefox support is weak: a check of addons.mozilla.org returned a clear phishing clone ("🐇abby" by "Admin", 28 users) rather than a real Rabby build. Installing that would have been catastrophic.
- Dedicating a separate browser for crypto reduces tab-confusion risk and isolates extension surface area. This is a well-known best practice.
- Brave is free, Chromium-based, runs well on Windows, and takes ~2 minutes to install.

**Alternatives considered:**
- _MetaMask on Firefox_ — legitimate and works, but mixes everyday browsing with wallet context. Weaker safety warnings than Rabby.
- _Ambire on Firefox_ — legitimate, but less widely vetted than MetaMask or Rabby.
- _Use existing Firefox with Rabby_ — rejected because no real first-party Firefox Rabby build exists.

**Status:** Locked. First-day-of-crypto safety lesson already earned: every wallet extension must be installed from the official project site, not from app-store search results.

---

## 2026-04-23 — Brand name: Afferium

**Decision:** The company / holding brand for Coral's Sensorium project is **Afferium**.

**Reasoning:**
- Available across major TLDs (`.com`, `.io`, `.ai`, `.co`) and clear on USPTO trademark search at time of decision.
- Sits in the exact register as _Sensorium_ — Latin-scientific, -ium ending, three syllables, stress on the second.
- Meaning is load-bearing for the project: _afferent_ nerves carry signal inward to the brain; **Afferium** = the place that signal arrives. Matches the Sensorium thesis directly.
- It is itself a **proto-word** — sounds real, doesn't exist, enacts its own meaning. This is the decisive aesthetic win.
- Sister-approved. She rejected everything before this.

**Alternatives considered and declined:**
- _Proto Speech_ — USPTO clear but Jacob Ritchey has common-law rights via active studio at protospeech.com. Avoided conflict by pivoting.
- _Fremitus_ — squatter priced the .com at $2,500. Walked away.
- _Sensorium_ (as company name) — the book uses it as the conceptual frame; reserving it as a term-of-art inside the project rather than naming the company after it. Also the .com was $200,000.
- _Foretongue, Nervespeech, Thrumspeech, Ganglion.press, Glossa.press, etc._ — shortlisted but felt like linguistics-department energy, not sleek enough for sister's vibe check.

**Status:** Locked. `afferium.com` + `afferium.io` registered in Coral's name.

---

## 2026-04-23 — Domains: .com + .io purchased, .ai + .co deferred

**Decision:** Registered `afferium.com` and `afferium.io` only. Did not (yet) register `.ai` or `.co`.

**Reasoning:**
- `.com` is non-negotiable for a real brand.
- `.io` covers the tech/software side of the brand story and fits the sovereignty-leaning aesthetic better than `.ai`.
- `.ai` is ~$100/yr — higher ongoing cost. Deferred until we know if Afferium will ever ship an AI-flavored product line.
- `.co` is cheap and defensive but not urgent.

**Status:** `.com` + `.io` registered. `.ai` + `.co` deferred. Revisit if someone else registers them, or in 3-6 months regardless.

---

## 2026-04-23 — Social handle strategy: `@afferium` for brand, `@protospeech` for personal

**Decision:** Coral will sweep `@afferium` on social platforms as the brand account. `@protospeech` stays as Coral's personal handle.

**Reasoning:**
- Different roles: Afferium is the company, Protospeech is Coral's personal identity.
- Cleaner story if collaborators, press, or artists ever need to find either separately.
- The `@protospeech` handle predates awareness of Jacob Ritchey's studio; using it authentically as personal identity is defensible. Squatting empty would be risky.

**Status:** Strategy locked. Sweep in progress. See `HANDLES.md`.

---

## 2026-04-23 — Trademark filing: deferred, 1(b) planned

**Decision:** Do not file a USPTO trademark yet. Plan to file a **1(b) intent-to-use** application within 3-6 months if Coral is still committed to Afferium at that point.

**Reasoning:**
- Common-law rights attach from use; federal registration is additive protection.
- Filing now locks in priority but costs ~$1,050 for three classes (9, 16, 41) before there's revenue.
- Filing in 3-6 months gives time to validate direction without losing priority to a hypothetical later filer.
- Revisit if another party appears to be exploring the name.

**Status:** Timer running, decision point ≈ 2026-07 to 2026-10.

---

## 2026-04-23 — Entity formation: deferred until income or liability requires it

**Decision:** Do not form an LLC (or any legal entity) for Afferium yet.

**Reasoning:**
- No revenue. No contracts with third parties. No liability exposure. No collaborator or investor is requiring it.
- Forming early costs money (filing + annual fees + registered agent) and creates administrative overhead without benefit.
- When the time comes, likely choice is Wyoming LLC (cheap, private) or home-state NY LLC (operational simplicity) — decision deferred to that future moment.

**Status:** Deferred. Revisit when any triggering condition (income, contract, liability, collaborator) appears.

---

## 2026-04-23 — Urbit: pursue sovereignty, move from moon to planet

**Decision:** Coral will buy her own Urbit planet rather than remain as a moon under someone else's planet.

**Reasoning:**
- Afferium's thesis requires self-sovereign infrastructure where plausible.
- Moons are technically subordinate to the parent planet — keys are issued by and visible to the planet operator in principle.
- A planet is a one-time purchase (~$15-50 on secondary market, plus ~$30 ETH for gas), not a subscription.
- The learning investment required (Ethereum wallet stack) pays off beyond just Urbit — it's general crypto literacy.
- Philosophically on-brand: a company about authenticity in computer-mediated expression should run on infrastructure it actually owns.

**Alternatives considered:**
- _Stay on the moon._ Works, but subordinate identity mid-brand-build is awkward.
- _Tlon-hosted planet._ Easy but Tlon Corp holds the keys — trust model is almost identical to being a moon. Missed the point.
- _Buy hosted but non-custodial._ This is the actual path: buy the planet on-chain (sovereign ownership), pay Red Horizon / Holium / Native Planet to host the ship (sovereignty preserved, operational complexity handed off).

**Status:** Full playbook written in `URBIT-PLAYBOOK.md`. Execution begins at Phase 1 (wallet setup) when Coral is ready.

---

## 2026-04-23 — Documentation directive: "DOCUMENT EVERYTHING"

**Decision:** Flere will document every step of Afferium's construction — decisions, setup procedures, learning paths, dead ends, reasoning — as the work happens, in the `afferium/` folder in this workspace.

**Reasoning:**
- Coral is new to crypto/Urbit/brand formation and is deliberately learning rather than paying-and-praying.
- Documentation doubles as Coral's personal knowledge base and future reference.
- Most of the playbook becomes a reusable template for Coral's sister's eventual mustard business.
- A company built on honesty-in-computer-mediated-expression should itself be legible on paper.

**Status:** Active, ongoing.

---

## How to use this file

- **New decisions go at the top**, so reading top-to-bottom shows the most recent thinking first.
- **Never rewrite or delete old entries.** If a decision is reversed, add a new entry that says so and cross-references the old one.
- **Keep entries specific.** "Decided to do X because Y. Considered Z but declined because W." Future-us will thank present-us.
- **When in doubt, over-document.** Terseness can be fixed by reading; missing context cannot be reconstructed.
