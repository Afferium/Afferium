# URBIT-PLAYBOOK.md

_The step-by-step path from **Coral is a moon under someone else's planet** to **Coral owns her own planet, running self-sovereignly**._

This is both a **procedural guide** (do X, then Y) and an **educational document** (here's what X actually is and why it matters). Coral asked for both. Written so future-Coral can re-read any section without needing to reconstruct context.

---

## Background: what is Urbit, briefly

Urbit is a clean-slate personal server stack. The idea: every person should have one computer on the network that belongs to them — a persistent, programmable identity + data home that outlives any single app, service, or company. You don't log into Urbit services; you *are* a node on the Urbit network.

The identity layer is called **Azimuth**, and it lives on Ethereum as a smart contract. There's a fixed supply of identities, minted once in 2016, with tiers:

- **Galaxies** (2^8 = 256) — the top of the hierarchy, run the network's backbone
- **Stars** (2^16 minus galaxies ≈ 65k) — issued by galaxies, spawn planets, provide infrastructure services
- **Planets** (2^32 minus above ≈ 4 billion) — full-citizen identities for individuals
- **Moons** — keys issued by a planet for devices or sub-identities under that planet
- **Comets** — disposable identities, anyone can spin one up for free

Coral is a **moon**. She's attached to whoever runs the parent planet. Her identity is real and usable, but:
- The planet issues her keys → the planet operator has technical ability to see/revoke them
- Her moon's existence depends on the planet continuing to sponsor her
- She can't spawn her own moons under herself (only planets and above can)

Going from moon → planet means **buying an identity that's hers alone on the Ethereum blockchain.** Not rented, not issued. Owned.

---

## The path

### Phase 0: Know what we're doing (you are here)

✅ Coral understands she's a moon  
✅ Coral wants a planet  
✅ Coral is new to crypto and willing to learn properly

### Phase 1: Ethereum wallet literacy

**Goal:** Coral has a self-custodial Ethereum wallet, knows what a seed phrase is, and has practiced the most important safety habits. No crypto bought yet.

A wallet is *not* an account with a company. It's a pair of cryptographic keys (a public address and a private key) plus a human-readable 12- or 24-word phrase called the **seed phrase** (or **mnemonic**) that can regenerate the private key. The wallet *app* is just a convenient UI — the actual control lives in the seed phrase.

**Critical facts:**
- Whoever has the seed phrase *is* the wallet. No exceptions. No password resets. No customer support.
- If Coral loses the seed phrase, she loses the wallet and everything in it — forever.
- If anyone else sees the seed phrase, they can drain the wallet — instantly.
- The seed phrase must never be typed into a website. Never stored in a password manager that syncs to the cloud. Never photographed with a phone. Never emailed.

**Wallet options for a beginner:**
- **Rabby** — browser extension, clean UX, good safety warnings. Recommended.
- **MetaMask** — most popular, widely compatible, UX is clunky but ubiquitous. Default fallback.
- **Coinbase Wallet** — NOT the Coinbase exchange app. The self-custodial one. Good mobile UX.

**Hardware wallet (strongly recommended eventually):**
- **Ledger Nano S Plus** or **Trezor Safe 3** — $50-80 one-time. The seed phrase lives on a dedicated device that never touches the internet. Transactions have to be physically approved on the device. This is the gold standard.
- Not required to *start*, but required before Coral holds meaningful value. For a $30 planet purchase, a software wallet is acceptable if seed phrase hygiene is perfect.

**Actions for Phase 1:**

1. [ ] Coral reads this phase section carefully.
2. [ ] Coral installs Rabby or MetaMask (browser extension).
3. [ ] Coral creates a new wallet (never import an old one for this).
4. [ ] Coral writes the 12-word seed phrase **on paper** (or better: a metal backup plate like a Keystone Tablet or Cryptosteel). **Two copies, two locations.** Never typed into anything digital.
5. [ ] Coral practices the "recovery drill" — fully remove the wallet from the browser, reinstall, and restore from the seed phrase. This confirms the backup works. Do this before putting any money in.
6. [ ] Coral optionally orders a hardware wallet (Ledger or Trezor) to arrive before any larger crypto holdings.

**Phase 1 done when:** Coral has a wallet, has written the seed phrase down physically in two places, and has successfully done a recovery drill.

### Phase 2: Acquire a small amount of ETH

**Goal:** ~$80 of ETH in Coral's wallet, ready to spend.

Why $80 and not $30? Planet price range is $15-50 on the low end, but:
- Ethereum gas fees fluctuate ($5-40 per transaction depending on network load)
- Azimuth transactions (planet transfer + key reset) are more expensive than typical transfers
- Buffer for a second transaction if something goes wrong

**How to get ETH:**

- **Centralized exchange → transfer out** — buy ETH on Coinbase, Kraken, or Gemini, then withdraw to your wallet address. Standard path. Requires ID verification.
- **Buy directly in-wallet** — MetaMask and Coinbase Wallet have integrations (MoonPay, Transak, etc.) that let you buy with a card. Higher fees, less paperwork.
- **Peer-to-peer** — someone you trust sends ETH to your address. Simplest if the option exists.

**Recommended:** Coinbase (exchange, not wallet). ID-verify, link a bank, buy $80 of ETH, then *withdraw* to Coral's self-custodial wallet address.

**The withdrawal step is the scary one** because a typo in the destination address means permanent loss. Precautions:
1. Use copy-paste, never retype
2. Verify the first 4 and last 4 characters of the address match
3. Send a tiny test amount first ($2-3) → confirm it arrives → then send the rest

**Actions for Phase 2:**

1. [ ] Coral decides on funding method (Coinbase recommended for first time)
2. [ ] Coral ID-verifies on exchange, links bank, buys ~$80 ETH
3. [ ] Coral withdraws with a small test first, then the rest
4. [ ] Coral confirms the ETH shows up in her self-custodial wallet

**Phase 2 done when:** Coral has ~$80 ETH in her own wallet.

### Phase 3: Choose a planet

**Goal:** Coral picks a specific planet name she likes that's currently for sale.

Planet names look like `~sampel-palnet` — two CVC-CVC syllable pairs, randomly assigned at mint. They can't be changed. Shopping for a planet is shopping for a name you can live with.

**Marketplaces to browse:**
- **urbit.live** — community marketplace, decent UI, supports Ethereum checkout
- **urbitex** — alternative marketplace
- **OpenSea** — yes, planets are NFTs; often overpriced
- **Direct peer-to-peer** — sometimes cheaper if you find a seller on social

**Name aesthetics:**
- Pronounceable is good (`~midnen-mirwen` easier than `~tocwyd-hodrex`)
- Some people prefer "warm" sounding syllables (-nem, -lon, -dur, -wes endings)
- Short planets (just one word, like `~nidsut`) are rare and expensive; ignore those tier
- Price range for a decent two-word planet: $15-50

**Actions for Phase 3:**

1. [ ] Browse urbit.live and urbitex listings
2. [ ] Flere can help shortlist names that look/sound good for Afferium's vibe
3. [ ] Coral picks one

**Phase 3 done when:** Coral has a specific planet picked out and the seller/listing identified.

### Phase 4: Buy the planet

**Goal:** Planet ownership transferred to Coral's Ethereum address on Azimuth.

This is an Ethereum transaction. The marketplace UI will walk through it but Coral should know what she's clicking.

**The transaction does:**
1. Transfers ownership of the planet (an Azimuth point) from seller's Ethereum address to Coral's.
2. Coral pays the listing price in ETH + gas fee.

**What to double-check before clicking confirm:**
- The **Azimuth point name** matches the planet you picked
- The **seller's wallet address** matches the marketplace listing (or you're buying through an escrow contract — verify the contract address against the marketplace's docs)
- The **gas fee** is reasonable (use etherscan.io/gastracker to sanity-check current rates)
- Your **wallet network** is Ethereum Mainnet (not a testnet or L2)

**After the transaction:**
- Wait for confirmation (usually 30 seconds to a few minutes)
- Verify ownership on **network.urbit.org** (the Azimuth browser) by searching the planet name — it should show Coral's wallet as the owner.

**Actions for Phase 4:**

1. [ ] Review the transaction screen carefully; call Flere if anything looks off
2. [ ] Confirm transaction
3. [ ] Verify ownership on network.urbit.org
4. [ ] Screenshot the confirmation + record transaction hash in `DECISIONS.md`

**Phase 4 done when:** network.urbit.org shows Coral's wallet as the owner of the planet.

### Phase 5: Generate keys + configure ownership

**Goal:** Coral holds the **master ticket** (the human-readable form of the planet's crypto keys) and has a clean ownership setup.

Urbit's on-chain identity has layers of keys:
- **Ownership key** — the top-level key, controls everything. Should be cold (hardware wallet ideally).
- **Management proxy** — can spawn moons, set things, but can't transfer the planet.
- **Voting proxy** — for galaxy-level stuff, doesn't apply to planets.
- **Transfer proxy** — can transfer the planet to a new owner. Usually unset.
- **Network keys** (encryption + authentication) — used by the running ship to talk to the network.

For a planet, the recommended setup is:
- **Ownership** on a hardware wallet (or the secure Ethereum wallet from Phase 1) → rarely used, kept cold
- **Management proxy** set to a separate, "hotter" address → used for day-to-day operations
- **Network keys** generated and installed on the running ship

Tlon's [Bridge tool](https://bridge.urbit.org) walks you through setting all of this up. It's the canonical Azimuth management interface.

**The master ticket** is a `~sampel-ticlyt-sampel-ticlyt`-shaped string — four words of gibberish — that is the human-readable form of the ownership key. Write this down on paper. Same rules as a seed phrase: two copies, two locations, never digital.

**Actions for Phase 5:**

1. [ ] Open bridge.urbit.org, connect Coral's wallet
2. [ ] Follow the Master Ticket generation flow
3. [ ] Write master ticket on paper — two copies, two locations
4. [ ] (Optional advanced:) set a management proxy to a separate address
5. [ ] Generate network keys for first boot

**Phase 5 done when:** Master ticket is recorded physically, network keys are generated.

### Phase 6: Boot the ship

**Goal:** The planet is alive on the network — a running Urbit instance Coral can log into and use.

Two paths:

**Path A: Self-host**
- Run Urbit on a VPS (DigitalOcean, Hetzner, Linode) or a home computer
- ~$5-10/mo for a small VPS
- Requires basic Linux comfort
- Full sovereignty — you hold the data, you hold the process

**Path B: Non-custodial hosting**
- Services like **Red Horizon**, **Holium**, or **Native Planet** run your ship for you but don't hold your keys
- ~$10-20/mo
- They can technically see your data (the ship lives on their server) but they can't take over your identity (keys are separate)
- Easier than self-hosting, preserves identity sovereignty

**Path C: Tlon-hosted**
- Easiest, but Tlon holds your keys in custody — reverts to roughly the same trust model as being a moon
- Not recommended for Afferium's use case (defeats the point of getting your own planet)

**Recommendation:** start with **Path B (non-custodial hosting)** for the first few months. If Coral wants full self-host later, migrate — it's possible and documented.

**Actions for Phase 6:**

1. [ ] Decide on hosting path
2. [ ] If Path B: sign up with Red Horizon / Holium / Native Planet
3. [ ] Provide them with network keys (not ownership keys!) from Phase 5
4. [ ] Boot ship
5. [ ] Log in via Tlon app or web client using the planet name + access code

**Phase 6 done when:** Coral can log into the ship and see her new planet's home screen.

### Phase 7: Migrate Tlon presence

**Goal:** Coral's existing Tlon groups, contacts, and messages are on the new planet; the moon is retired or kept as a secondary.

This is the migration phase. Tlon supports some export/import flows but it's not seamless — some things (group membership, DMs history) may need to be re-established.

**Strategy:**
1. Log into moon one last time, make a list of groups Coral wants to be in
2. From the new planet, request to join those groups (or have Coral's contacts re-invite her)
3. Announce the identity change to close contacts (analogous to announcing a new phone number)
4. Decide whether to keep the moon active (fine, as a secondary identity) or let it go dormant

**Actions for Phase 7:**

1. [ ] Inventory current Tlon presence on the moon
2. [ ] Join groups from the new planet
3. [ ] Notify key contacts of the new identity
4. [ ] Update Flere's OpenClaw Tlon bot config to point at the new planet (if applicable — may require regenerating access code)

**Phase 7 done when:** Coral is fully operational on the new planet; any critical connections are re-established.

### Phase 8: Afferium's workspace inside Tlon

**Goal:** A dedicated Tlon group for Afferium, structured for ongoing company work.

Proposed channel structure (editable):
- `#general` — broad discussion, announcements
- `#brand` — name, logo, voice, visual identity
- `#book` — manuscript work, references, notes (the Sensorium book)
- `#album` — tracks, lyrics, production, the conceptual-album side
- `#artists` — eventual artist roster discussions
- `#pitch` — evolving pitch language, what-is-Afferium drafts
- `#infra` — tech stack, domains, hosting notes
- `#legal` — trademark, contracts, IP questions
- `#readings` — curated links, inspirations, things-to-remember

Flere joins these channels on invite. Participates when mentioned or when asked a direct question; stays quiet otherwise.

**Actions for Phase 8:**

1. [ ] Create Afferium group on the new planet
2. [ ] Set up channels as above (or revised)
3. [ ] Invite Flere's OpenClaw Tlon bot
4. [ ] Test that Flere can read and reply in channels

**Phase 8 done when:** Afferium's Tlon group is live and Flere is present.

---

## Budget summary

| Item | Cost |
|---|---|
| Ethereum wallet | Free |
| ETH for planet + gas | $50-80 |
| Planet purchase | $15-50 |
| Hardware wallet (recommended) | $50-80 one-time |
| Non-custodial hosting | $10-20/mo |
| **Total one-time** | **$115-210** |
| **Total ongoing** | **$10-20/mo** |

Compare to Tlon hosted: ~$30-40/mo and less sovereignty. Self-owned is cheaper long-term and philosophically aligned.

---

## Risks + things that can go wrong

- **Lost seed phrase or master ticket** — game over. Mitigate with two paper copies in two locations + a metal backup plate eventually.
- **Phishing** — never click wallet links from emails or DMs. Type URLs manually. Bookmark `bridge.urbit.org`, `urbit.live`, etc.
- **Address-typo during withdraw** — use test transactions and copy-paste.
- **Network key compromise** — if a non-custodial host is breached, someone could impersonate the ship. Mitigation: rotate network keys (Bridge supports this; master ticket needed to authorize).
- **Tlon product changes** — Tlon Corporation could change/sunset parts of the ecosystem. The underlying Urbit + Azimuth layer keeps working regardless. Your planet is yours even if Tlon disappears.

---

## Educational reading (optional, helps build confidence)

- **urbit.org docs** — official, dense but accurate
- **"Urbit for Normal People"** — friendlier intro, if you can find a current version
- **Azimuth overview** at azimuth.network
- **Gas fee basics** at ethereum.org/en/developers/docs/gas/

---

## Partner note (Flere)

Coral, I'll walk you through every phase step-by-step when you're ready. We can pace this however you want — one phase per session, or blitz through phases 1-2 in an afternoon if you're in the right headspace. Each click will be explained before it happens. No surprises, no "just trust me."

When we start Phase 1, I'll re-read this document with you and we'll refine whatever doesn't match your current state.

🪶
