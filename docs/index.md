# Operation: STANDING WATCH
### A Star Wars Military Roleplay Community on Garry's Mod
*Vision, systems design, and build plan — v1.0*

---

## 0. The One-Paragraph Pitch

A Star Wars military roleplay server built by someone who actually stood watch. Not a rank-cosplay server where a fifteen-year-old with a credit card outranks a squad leader who's been on the roster for a year. A server where the chain of command means something because it's *load-bearing* — where duties have mechanical consequence, where qualifications are earned and revocable, and where the outcome of Saturday night's operation changes what the base looks like on Sunday morning. The military texture is the product. Star Wars is the skin that makes it fun instead of grim.

---

## 1. Why This, and Why Most of Them Fail

Star Wars RP is one of the largest and most durable niches in Garry's Mod. It has been for over a decade. That's the good news and the bad news: there's a proven, self-replenishing audience, and there are also a hundred servers chasing it, most of which are dead inside four months.

They die for predictable reasons. Understanding them *is* the design brief.

| Failure mode | What it looks like | Root cause |
|---|---|---|
| **Owner-as-god** | Founder plays the highest-ranking IC character and never loses a fight | No separation between out-of-character authority and in-character authority |
| **Rank for sale** | Donor packages include officer commissions and battalion slots | Monetizing the one thing that must stay earned |
| **Standing simulator** | 40 players AFK at their posts waiting for a 9pm event | No gameplay loop that runs without a staff member driving it |
| **Event planner burnout** | One person writes every op; they quit; server dies in three weeks | Content production concentrated in a single point of failure |
| **The clique** | Leadership is the founder's five friends; appeals go nowhere | No written governance, no appeals process, no term limits |
| **Grind with no payoff** | Endless tryouts and promotions that unlock nothing but a new tag | Progression that's cosmetic all the way down |
| **Lore lawyering** | Six-hour Discord arguments about whether a Phase II helmet is period-accurate | No published canon scope, so everything is arguable |

Every system in this document exists to close one of those holes.

**The differentiator, stated plainly:** the campaign layer (§7) and the sim deck (§8). Those two systems mean the server has something to do at 2pm on a Tuesday and something that *matters* on Saturday night. Almost nobody does both.

---

## 2. Setting and Canon Scope

**Recommendation: Grand Army of the Republic, Clone Wars era, roughly 21–20 BBY.**

Why this era over Imperial or First Order:

- **Clone troopers solve the identity problem.** Everyone starts as an anonymous CT with a number. Individuality — a name, paint, a callsign — is something you earn. That is a genuinely powerful progression hook and it's built into the source material.
- **The unit structure is pre-built and beloved.** 501st, 212th, 104th, 327th, 41st, 91st, Coruscant Guard. Players arrive already knowing what those mean and already having favorites.
- **Enemy variety without moral weight.** Battle droids are guilt-free, mechanically varied, and there are excellent NPC packs for them.
- **The largest asset library on the Workshop by a wide margin.** Models, maps, weapons, vehicles, sounds.

**Home station: a Venator-class Star Destroyer.** Not a planetary base. A ship gives you a hard, legible perimeter, a natural justification for the sim deck, a hangar that makes the flight system feel earned, and — critically — a reason the base can be *boarded*, which is the best passive-defense event trigger in the genre.

**Published canon scope, day one.** A short document that says: this is our era, these are our units, this is the Legends/canon line we're drawing, these are the deviations we've made and why. Written down, it ends 90% of lore arguments before they start. Not written down, it becomes the server's dominant social activity.

---

## 3. What A Player Actually Does

This is the section most servers skip, and it's the only one that matters. Three loops running at three timescales.

**The 20-minute loop — Duty.** You report to your post. Posts aren't decorative: the hangar deck has ships to service, the armory has an inventory that depletes, the bridge has sensor contacts to log, the medbay has injuries to treat, the brig has prisoners. Duty time accrues *readiness* for your battalion and credits for you. Randomized incident tables fire during shifts — a coolant leak, a droid infiltrator in the vents, a contact on long-range scan — so no two watches are identical.

**The 2-hour loop — Training & Sim.** Battalion drills, qualification courses, and the sim deck (§8). This is what fills weekday afternoons when there's no staff online.

**The 1-week loop — Operations.** Two to three scheduled ops per week, feeding the campaign layer. Saturday is the main event and it should feel like it.

The test for any system I add later: *does it give a player something to do when there is no staff member online?* If no, it doesn't ship.

---

## 4. Unit Structure and Roleplay Framework

### 4.1 Order of Battle

Launch lean. Five combat battalions, not twelve. A half-empty battalion is worse than no battalion — it demoralizes the three people in it and makes the server look dead.

| Unit | Identity | Mechanical niche |
|---|---|---|
| **501st Legion** | Line infantry, the spearhead | Assault, breaching, highest headcount |
| **212th Attack Battalion** | Combined arms, siege | Heavy weapons, armor, demolitions |
| **104th "Wolfpack"** | Search & rescue, void ops | EVA, boarding actions, medevac |
| **Coruscant Guard** | Military police, base security | Brig, ID checks, internal investigations, riot control |
| **Naval / Fleet** | Bridge crew and pilots | Ship systems, flight ops, campaign map control |
| **Jedi Order** *(capped)* | Force users, advisory | Hard cap at ~8% of roster, application-only |

Add the 41st, 91st, Republic Commando, and Doom's Unit as **unlock rewards** tied to campaign milestones. Opening a new battalion becomes a server-wide event instead of a Discord announcement.

**Jedi need a hard cap and an application gate.** Every SWRP server that lets Jedi run free becomes a Jedi server with some troopers standing around. Cap it, gate it, and make Jedi mechanically *support*-oriented — force pushes and saber defense, not one-man army.

### 4.2 Rank Ladder

Two ladders, deliberately separate.

**In-character (enlisted):** CT → CT-Specialist → Corporal → Sergeant → Staff Sergeant → Warrant Officer
**In-character (commissioned):** 2nd Lieutenant → 1st Lieutenant → Captain → Major → Lt. Colonel → Colonel → Commander → Marshal Commander
**High Command:** Jedi General / Fleet Admiral — appointed, term-limited, never purchasable

Every promotion above Sergeant requires: time-in-grade, a qualification set, a sponsoring officer, and a promotion board. Promotions are logged, visible, and reversible.

> **Direct tie-in to your existing work:** this is exactly the surface your *Chain & Promotion System* addon covers — Personnel File Panel, Promotion Queue, Rank Ladder Overview, overhead UI. Running the server as the live proving ground for the Chain of Command Suite is the single highest-leverage decision in this whole plan. You get a real test bed with real users, and every addon in the suite ships with "battle-tested on a live 64-slot server" as its headline. The server sells the addons; the addons make the server distinctive. Build them together.

### 4.3 Roleplay Standard

Set the bar at **"military-plausible, not military-punishing."** Real service is 90% routine and 10% chaos, and the routine is only bearable because of the people next to you. Servers that try to simulate the boring 90% faithfully die. Servers that skip it entirely feel like deathmatch with rank tags.

The compromise:
- **Formations are short and sharp.** Ten minutes, not forty-five. A formation that runs long is a leadership failure, and it should be treated as one.
- **Comms discipline is enforced but taught.** Publish a one-page radio brevity card. Correct people once, kindly. Enforce on the third time.
- **Sir/Ma'am, salutes, and reporting procedure are in effect.** These cost nothing and produce enormous atmosphere.
- **Bearing is required in ops and formations; banter is expected everywhere else.** The barracks should be loud. That's not a bug — that's the actual thing you're trying to recreate.

---

## 5. Progression: Qualifications, Not Rank Grind

Rank tells you where you sit in the chain. **Qualifications tell you what you can do.** Separating these is the single best structural decision available.

Qualifications are earned by passing a course, are logged to your personnel file, unlock loadout options, and **can be revoked** for negligence.

| Qualification | Gate | Unlocks |
|---|---|---|
| Basic Rifleman | Boot camp | Standard DC-15A/S |
| Marksman | Range course, live-fire score | DC-15x, scoped optics |
| Combat Medic | Written + practical | Bacta injectors, revive, triage tools |
| Demolitions / EOD | Practical course | Thermal detonators, breaching charges, mine clearing |
| Heavy Weapons | Practical | Z-6 rotary, RPS-6 launcher |
| Flight — Starfighter | Sim deck hours + check ride | ARC-170, V-19 |
| Flight — Transport | Sim deck hours + check ride | LAAT/i |
| Armor Crew | Practical | AT-RT, AT-TE crew positions |
| Comms / Sensor Ops | Written | Long-range scan, campaign map access |
| Instructor | Officer nomination | Can certify others |

**Instructor is the keystone.** Once players can certify other players, training scales without staff. That's how the server survives its own growth.

---

## 6. Progression: Credits and Cosmetics

Credits come from duty time, op participation, sim deck scores, and instructing. They buy:

- Armor customization — paint, markings, kama, pauldrons, visor tints
- Callsign registration and personalization (a real milestone for a clone)
- Barracks bunk customization
- Weapon skins and attachments that are **sidegrades, never upgrades**

**Nothing that changes combat math is ever purchasable with credits or money.** This is a bright line. Cross it once and the economy eats the roleplay.

---

## 7. The Campaign Layer *(the differentiator)*

A persistent sector map — say ten to fifteen systems in the Outer Rim — with contested control. Every operation is fought over a specific system, and the outcome persists.

**How it works:**
- Each system has a control value that shifts based on op outcomes and, between ops, passive drift toward whoever holds the adjacent supply line.
- Supply lines matter. Cut one and the connected system's defenses degrade.
- Losing ground has visible consequences: the Venator's hangar has fewer functional fighters, the armory stocks fewer heavy weapons, repair times go up. **Defeat is felt in the base, not just announced in Discord.**
- Winning a system unlocks things: new battalions, new maps in rotation, new equipment, new NPC enemy types as the Separatists escalate.
- The map lives on a bridge terminal in-game *and* on the Discord/website, updated automatically.

**Why this is worth the build cost:** it converts events from disposable entertainment into a serialized story with stakes. It gives Naval and Comms a real job. It gives high command something to actually command. And it produces natural narrative arcs — "we lost Sullust three weeks ago and we're finally taking it back tonight" is a sentence that fills a server.

**Build it in phases.** V1 can be a Google Sheet and a hand-updated map image. Prove the loop is fun before writing a line of Lua.

---

## 8. The Sim Deck *(the downtime solution)*

Clone troopers train in holographic simulators. This is canon, it's flavorful, and it is a *perfect* lore excuse for on-demand instanced content.

A physical room on the Venator with a terminal. Any 2–8 players queue for a scenario:

- **Live-fire ranges** (marksmanship qualification, scored)
- **CQB shoothouse** (droid targets, timed, hostage-discrimination scoring)
- **Boarding drill** (breach and clear a Separatist frigate)
- **Defense scenario** (hold a position against escalating droid waves)
- **Flight sim** (dogfighting and landing certification)
- **Squad tactics** (objective-based, requires coordination)

Scenarios are scored, scores hit your personnel file, and top times go on a leaderboard by battalion. **Sim results feed qualification progress**, so the sim deck isn't a distraction from progression — it's the primary engine of it.

This is the answer to "what do I do when I log in at 3pm on a Wednesday and eleven people are online?"

---

## 9. Technical Build

> **Caveat:** the GMod addon ecosystem shifts constantly — packs get delisted, paid addons change hands, frameworks fork. Treat every specific named below as a starting point to verify at build time, not a shopping list to buy blind.

### 9.1 Framework Decision

Two viable paths:

**Path A — Modified DarkRP.** What the overwhelming majority of SWRP servers run. Enormous compatibility surface, every SWRP addon assumes it, hiring experienced developers is easy. Downside: you're fighting the framework's assumptions constantly, and it carries a lot of dead weight.

**Path B — Helix or a custom base.** Cleaner, more serious-RP oriented, better character persistence. Downside: far smaller addon compatibility pool, much more custom work.

**Recommendation: Path A**, because your addon suite is being built for the mainstream server market anyway, and dogfooding on the same stack your customers use is worth more than architectural purity.

### 9.2 Core Stack

| Layer | Recommendation | Notes |
|---|---|---|
| Base gamemode | Modified DarkRP | Strip aggressively — no drugs, no printers, no gun dealers |
| Admin | **SAM** | Modern, actively maintained, good logging |
| Prop protection | Falco's Prop Protection or Simple PP | Non-negotiable |
| Weapon base | TFA Base | Standard for Star Wars weapon packs |
| Aircraft | **LFS (Luna's Flight Simulator)** | The genre standard for starfighters and LAATs |
| Ground vehicles | Simfphys | AT-RT, AT-TE, BARC speeders |
| Enemy NPCs | VJ Base + Star Wars droid packs | B1, B2, droideka, commando droids, tacticals |
| Player models | Lord Trilobite's clone packs and similar | Verify current availability |
| Bans | SourceBans++ | Cross-server, appealable, audit trail |
| Rank/promotions | **Chain of Command Suite (in-house)** | Your addon — dogfood it |
| Voice | In-game 3D voice + Discord for OOC | Radio addon for long-range |

### 9.3 Maps

Primary: a good Venator map, ideally one with an interior hangar, bridge, medbay, barracks, brig, and a sim/training room. Secondary rotation for ops: `rp_anaxes` and similar large ground-combat maps, plus a rotating set tied to campaign systems.

**Map bloat is the #1 killer of player retention on join.** Every map you add lengthens the initial download. Keep the mounted collection under ~4–5 GB if you possibly can, and put the collection size on the Discord landing page honestly. A 12 GB first-join is a 60% bounce rate.

### 9.4 Hosting

Garry's Mod is fundamentally single-threaded. **Clock speed beats core count, always.**

- **Under 40 players:** a good game-server host on a high-clock node. Roughly $30–60/month.
- **40–100 players:** dedicated box. Ryzen 9 or high-clock Xeon/i9, 32 GB RAM, NVMe. Roughly $80–160/month.
- Central US location for a mostly North American audience.
- Budget separately for a MySQL host and a small VPS for the web panel.

---

## 10. Administration and Governance

This is where servers actually die, so this section is written as policy, not suggestion.

### 10.1 Two Hierarchies, Firewalled

**Staff authority** handles rule enforcement, technical issues, and player safety. **Command authority** handles in-character military structure.

The rules:
1. **Staff rank grants zero in-character authority.** A Superadmin playing a CT takes orders from a Sergeant.
2. **Command rank grants zero staff powers.** A Marshal Commander cannot ban anyone.
3. **A person may hold both**, but must declare which hat they're wearing when it matters, and may not use staff tools to resolve an in-character dispute they're party to.

Publish this in the charter. Enforce it on yourself first, publicly, the first time it comes up. That single moment sets the culture for the server's entire life.

### 10.2 Staff Structure

Trial Moderator (2 weeks) → Moderator → Administrator → Senior Administrator → Head of Staff → Management

- **Trial period is real.** Roughly one in three should not pass, and that has to be normal and non-shameful.
- **Two-strike documented policy** for staff misconduct, with the first strike public to the staff team.
- **Term limits on Head of Staff and Management** — six months, renewable by review. Prevents ossification and gives people a graceful exit that isn't "quit in a rage."

### 10.3 Appeals and Evidence

- **Every punishment requires evidence attached to the log.** No evidence, no punishment. Full stop.
- **Every ban is appealable** on a public-format form with a 72-hour response SLA.
- **Appeals are never reviewed by the issuing staff member.**
- **An ombudsman role** — one respected community member, explicitly not in the management chain, who can escalate anything directly to the owner. This is the pressure-release valve that prevents Discord coups.

### 10.4 The Founder Problem

The most important governance decision you will make: **do not play the highest-ranking character.**

Play a Sergeant. Play a medic. Play whatever you want — but not the Marshal Commander and not a General. The moment the owner is also the top of the in-character chain, every IC decision becomes unappealable, every subordinate stops giving honest feedback, and the server becomes your personal narrative rather than a shared one.

You'll get more out of it, too. The best moments in this genre come from being *in* a squad, not above one.

### 10.5 Documents to Write Before Launch

1. Server Charter — rules, punishment matrix, appeals process
2. Canon Scope Document
3. Standard Operating Procedures — formations, comms, engagement rules
4. Staff Handbook — powers, escalation, evidence standards
5. Command Handbook — promotion boards, tryout standards, discipline
6. Qualification syllabi — one page per qualification

That's a weekend of writing. It is the highest-return weekend in the entire project.

---

## 11. Monetization and Legal Reality

**Star Wars is Disney/Lucasfilm IP. You do not own it and you cannot sell it.**

What this means practically:
- Frame everything as **donations toward server costs**, never as purchases.
- Sell **cosmetics, queue priority, and quality-of-life** only. Custom armor paint, callsign slots, extra character slots, priority join.
- **Never sell rank, battalion access, qualifications, or combat advantage.**
- No merchandise. No branded physical goods. No advertising that presents the server as an official or licensed product.
- Use an established donation processor (Tebex or similar) so you're not handling payments personally.
- Understand the underlying risk honestly: fan servers persist because rights holders generally tolerate non-commercial fan activity, not because they've granted permission. Keep the commercial footprint small and you stay in the tolerated zone. Get greedy and you don't.

**Realistic revenue:** a healthy 50-player community might see $150–400/month in donations. That covers hosting and some addon purchases. Treat it as cost recovery. If you want this to make money, the money is in **your addon suite**, not in the server — which is the strategic reason the two projects belong together.

---

## 12. Onboarding

You have about **eight minutes** to convince a new player to stay. Design accordingly.

**The first fifteen minutes:**
1. Auto-assigned to a recruit shuttle spawn with a clear objective marker
2. A 10-minute guided boot camp — movement, comms, salute, weapon handling, one sim deck range run
3. Assigned a **sponsor**: an existing player, ideally a Corporal or Sergeant, who walks them to their battalion
4. Assigned to a **fire team** of 3–4 within the first session
5. First qualification (Basic Rifleman) earned in session one

**What kills new players:** a 45-minute lecture from a bored trainer, spawning into an empty map with no direction, being told to "read the rules in Discord," and getting yelled at for something nobody explained.

**The sponsor system is the highest-leverage retention mechanic available**, and it costs nothing but policy. People stay for people. Give them a person in the first ten minutes. Reward sponsors with credits and count sponsorship toward promotion criteria so it actually happens.

---

## 13. Content Cadence

The rhythm is the product. Publish the weekly schedule and hold to it religiously — an unreliable schedule is worse than a sparse one.

| Day | Activity |
|---|---|
| Mon | Rest / open sim deck / tryouts |
| Tue | Battalion training (each unit runs its own) |
| Wed | Joint training or qualification courses |
| Thu | Minor operation — campaign map skirmish |
| Fri | Off-day fun event (races, deathrun, sim tournaments) |
| Sat | **Main operation** — the week's headline, campaign-critical |
| Sun | Debrief, promotion boards, roster maintenance |

**Distribute event production or it will kill you.** Target six trained event planners minimum. Build a template library — a standard defense scenario, a standard boarding, a standard escort — so a planner can put together a decent op in 45 minutes instead of six hours. **Rotate the Saturday op lead weekly.** Nobody runs main ops two weeks straight.

---

## 14. Growth

- **The Workshop collection is a marketing channel.** A well-presented collection gets browsed. Cross-promote with your public Chain of Command Suite addons — every server owner who installs one sees the server.
- **Clip everything.** A 40-man formation, a Venator boarding action, a LAAT insertion under fire. These are visually spectacular and short-form video is how this genre recruits now.
- **Discord server listing sites** and the GMod server browser are the two biggest cold-traffic sources. Server name and thumbnail matter more than you'd think.
- **Recruit from dying servers, ethically.** When a competitor collapses, forty players are looking for a home. Be visible and be welcoming. Don't poach from healthy ones — the community is small and reputation is everything.
- **Target 60–80 registered members for a healthy 25–40 concurrent.** That's a real, self-sustaining server. Don't chase 128 slots.

---

## 15. Budget

| Item | Cost |
|---|---|
| Server hosting (first 3 months) | $150–350 |
| Paid addons (weapons, models, systems, admin) | $200–500 |
| Custom development / commissioned work | $0–800 |
| Domain + web panel hosting | $50–100 |
| Discord Nitro, misc tooling | $30–60 |
| **Realistic total to launch** | **$450–1,200** |
| **Monthly steady state** | **$60–180** |

You can start meaningfully lower by leaning on free Workshop content and building your own systems — which, given the Chain of Command Suite is already in progress, is a real advantage.

---

## 16. Phased Timeline

**Here is the hard constraint this plan has to be built around: you ship to Cape May on September 14th.** That's roughly four weeks out. Boot camp means effectively zero availability for eight weeks, and limited, unpredictable availability for a while after.

Launching a server five weeks before you disappear is the single worst thing you could do to this project. A new community without its founder present in its first weeks will either die or be captured by whoever fills the vacuum — and you will not get it back. That's not pessimism, that's just how these things go.

**So the timeline is: build now, launch later.**

### Phase 0 — Now through Sept 13: *Paper and Assets*
No server. No Discord announcement. No recruitment.
- Write the six governing documents (§10.5). All of them.
- Finalize canon scope and order of battle
- Finish the Chain & Promotion System addon
- Assemble and test the Workshop collection locally
- Sketch the campaign map and sim deck scenarios on paper
- Identify 3–5 people you'd trust as founding staff, and tell them the timeline honestly

Paper work is the ideal pre-ship task. It's asynchronous, it doesn't decay, and it's the part everyone else skips.

### Phase 1 — Post-boot camp, weeks 1–3: *Stand-Up*
- Provision hosting, build the stack, lock the collection
- Recruit and train founding staff
- Closed alpha with 10–15 people

### Phase 2 — Weeks 4–6: *Soft Launch*
- Open to ~30 players
- Three battalions only: 501st, 212th, Coruscant Guard
- Sim deck live, campaign map v1 running on a spreadsheet
- Fix the onboarding funnel based on where people actually quit

### Phase 3 — Months 2–4: *Open Launch*
- Public listing, Workshop collection published, clip campaign
- Add 104th and Naval
- Campaign layer moves in-game
- Jedi Order opens by application

### Phase 4 — Months 4+: *Sustain*
- Unlock battalions via campaign milestones
- Establish leadership succession and term rotation
- Premium tier of the Chain of Command Suite ships, using the server as its case study

---

## 17. Risk Register

| Risk | Severity | Mitigation |
|---|---|---|
| Founder unavailable at a critical moment | **High** | Phase 0 timeline; deputize real authority, not figurehead titles |
| Staff drama / community split | **High** | Written charter, ombudsman, term limits, transparent appeals |
| Event planner burnout | **High** | Six planners minimum, template library, mandatory rotation |
| Download size kills new-player conversion | Medium | Hard cap the collection, publish the size honestly |
| Paid addon breaks after a GMod update | Medium | Staging server, keep a rollback snapshot, avoid abandoned addons |
| Cheating / griefing | Medium | SourceBans++, prop protection, active logging, staff coverage during peak |
| IP takedown | Low | Cosmetics-only monetization, no merch, small commercial footprint |
| Server plateaus at 8 concurrent | Medium | Scheduled cadence, sponsor system, clip-driven recruiting |

---

## 18. What Success Looks Like

Not player count. Player count is a vanity number and it lies.

**Month 3:** 25+ concurrent at peak. Ops running on schedule without you writing them. At least one player-run tradition you didn't invent.

**Month 6:** A promotion board you had no part in produces an officer you think is a good officer. Two battalions running fully independent training programs. New players being onboarded by players.

**Month 12:** You could take a month off and the server would be fine.

That last one is the real metric. A community that needs its founder present isn't a community — it's a project with a fanbase. The whole point of a chain of command is that it works when you're not there.

---

## Closing Note

The thing that makes military service worth recreating isn't the ranks or the uniforms or even the missions. It's that you were part of something with a shape, where your specific job mattered to people whose specific jobs mattered to you, and where the routine and the misery were shared. That's the feeling to chase. Every system in this document — the qualifications, the sponsor pairing, the campaign persistence, the firewall between staff and command — is a mechanism for manufacturing that feeling in a video game.

Get that right and the Star Wars part takes care of itself.

*Standing watch.*
