# CAMPAIGN MAP RULES
### [SERVER NAME] — The persistent war
*v1 runs on a spreadsheet. Prove the loop is fun before anyone writes code.*

---

## The idea

Operations aren't disposable. Every op is fought over a **named system**, the outcome persists, and what you hold changes what the ship can do next week.

**Losing should be felt in the base, not announced in Discord.** That's the whole design. A trooper who walks into a hangar with two fighters missing because we lost Sullust understands the campaign without reading a word.

---

## The map

**12 systems in an Outer Rim theater.** Original space — not canon planets fought over in canon battles, which keeps us free of lore arguments.

Each system has:

| Field | |
|---|---|
| **Name** | Original |
| **Control** | −5 (Separatist) to +5 (Republic), starts at 0 |
| **Adjacency** | 2–3 connected systems |
| **Trait** | One mechanical effect when held (see below) |

**Starting position:** Republic holds 3, Separatists hold 3, 6 contested at 0. We start with a foothold, not a victory — there has to be somewhere to go in both directions.

---

## Control

| Value | State |
|---|---|
| **+3 to +5** | Republic held — trait active |
| **+1 to +2** | Republic contested |
| **0** | Contested |
| **−1 to −2** | Separatist contested |
| **−3 to −5** | Separatist held — enemy trait active |

### How it moves

| Event | Change |
|---|---|
| Main operation won (Saturday) | +2 |
| Main operation lost | −2 |
| Minor operation won (Thursday) | +1 |
| Minor operation lost | −1 |
| Partial success | +1 or −1, planner's call |
| **Weekly drift** | ±1 toward whoever holds the majority of adjacent systems |

**Weekly drift is what makes the map feel alive between ops.** A system you took but can't support will slide back, and that's correct — it's how you teach that the map has a shape.

---

## Supply lines

A system is **supplied** if a chain of Republic-held systems connects it to our home station's system.

**Unsupplied systems:** trait inactive, drift doubles against us, and operations there start at a stated disadvantage in the brief.

**This is the strategic layer.** It means the map isn't a scoreboard — position matters, and High Command has an actual decision to make about where to fight next.

---

## System traits

Hold the system, get the effect. Lose it, lose the effect.

| Trait | Effect when held |
|---|---|
| **Shipyard** | Fighter losses replaced between ops |
| **Foundry** | Heavy weapons and explosives fully stocked in the armory |
| **Bacta source** | Medic supplies at full; faster revives |
| **Relay** | Long-range sensors extended; enemy ops telegraphed a week out |
| **Fuel depot** | Transport and armor available for ops |
| **Training world** | Sim deck scenario rotation expanded |
| **Listening post** | Reveals adjacent system control values |
| **Garrison** | Passive defense; drift resists one step |

**Enemy-held systems apply the inverse where it makes sense** — an enemy Foundry means tougher droid compositions in that theater.

---

## What loss actually looks like

The point of the whole system. When we lose ground, the base changes, visibly, without announcement:

- **Fighters missing from the hangar rack.** Physically absent.
- **Armory heavy weapons locker locked** with a supply notice.
- **Medbay supply shortage** — longer revive times.
- **Sensor board showing fewer systems.**
- **A system marked lost on the bridge map.**

**Conversely, winning opens things:** new battalions unlock at milestones, new maps enter the op rotation, new equipment reaches the armory.

---

## Battalion unlocks

Locked units don't exist yet in-fiction. They arrive as campaign events.

| Unit | Trigger |
|---|---|
| **41st Elite Corps** | Hold a jungle-theater system at +3 |
| **91st Recon** | Three consecutive successful recon ops |
| **327th Star Corps** | Hold 6 systems simultaneously |
| **Republic Commando** | Escalation trigger — 8 systems held |

**Opening a battalion is a server-wide event**, not a Discord announcement. Do a ceremony. It's free and people remember it for a year.

---

## Running it — v1

**A spreadsheet and a hand-updated map image. That's it.**

| Column | |
|---|---|
| System · Control · Adjacency · Trait · Supplied Y/N · Last op · Last changed |

**Weekly cycle, Sunday:**
1. Apply operation results
2. Apply drift
3. Recompute supply lines
4. Update the map image
5. Post the change summary to Discord
6. **Apply the base state** — lock the armory, pull the fighters, whatever changed

**Fifteen minutes a week.** Owned by Naval command or a designated campaign officer.

**Do not build this in Lua until it has run for two months on a spreadsheet.** If the loop isn't fun by hand, code won't fix it — and if it is fun, you'll know exactly what to build.

---

## Design rules

**Never let it snowball.** If we hold 10 of 12, escalate enemy strength hard. A campaign that's already won is a campaign nobody shows up for.

**Never let it collapse.** Below 2 systems held, enemy drift stops. Losing is a story; being unable to fight back is people leaving.

**The map serves the roleplay, not the reverse.** If a system change would produce a great story, the campaign officer may adjust it. Publish the reasoning.

**Publish every change.** Control values, drift, supply state — all visible. A hidden campaign is indistinguishable from no campaign.

**Give Naval a real job.** They run the map, brief High Command, and recommend where to fight. It's the only thing that makes bridge duty meaningful.

---

## The point

> *"We lost Sullust three weeks ago and tonight we're taking it back."*

That sentence fills a server, and no amount of standalone event content produces it.

---
*v1 spreadsheet-only. Revisit for in-game implementation after two months of live operation.*
