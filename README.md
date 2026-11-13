# AOS Build Lab — Sage Awakening vs Hashashin Awakening

**Two specs. Four loadouts. One shared PvP add-on build per class. Then a head-to-head test.**

Season: **Oct 15 – Dec 10, 2026** · Data snapshot: **Nov 12, 2026**
Baseline: post-July-2025 combat overhaul + the Oct 15, 2026 AOS season patch.

---

## TL;DR

| | Sage Awakening | Hashashin Awakening |
|---|---|---|
| Damage ratio group | **Skirmisher** | **Skirmisher** |
| Best preset | **Bulk (Evasion armour + Hoom ×4)** | **Bulk (Evasion armour + Hoom ×4)** |
| Signature crystal | Resolute (acc +27, HP +250) | Sacred Darkness (back/down/air +12%) |
| Universal add-on core | All DP +20 / All Accuracy +20 | All DP +20 / All Accuracy +20 |
| Win condition | Land **Seize**, dump the Upsurge combo | Bait stamina, land **Constriction** |
| Top-100 presence (global) | 2 players · 74.7% WR · 1,885 avg | 5 players · 56.0% WR · 2,044 avg |

**Verdict of the test: Hashashin Awakening, ~59:41.** Not because it hits harder — it doesn't, both
classes sit on the same 89.29% PvP ratio with no rock-paper-scissors edge between them — but because it
gets to the first protected CC more often, and AOS rounds are decided by the first clean CC.

**The single most counter-intuitive result:** the "Evasion" preset is not the evasion preset. It is the
**HP preset**, and it is ~20% tankier than the DR preset in a mirror — because the AOS crystal pool hands
out HP in much larger relative units than it hands out DR.

---

## 1. Method

Everything below is graded, because two of the four loadouts depend on choices I cannot verify from a
patch note and you should know which is which.

- **[V] Verified** — official patch note, official guide, or aggregated in-game data.
- **[C] Consistent** — stable community reference data, not published numerically by Pearl Abyss.
- **[I] Inference** — my derivation. The reasoning is shown so you can reject an input.

Three structural facts drive every decision here **[V]**:

1. In the arena your **AP, Damage Reduction, Accuracy and Evasion are all halved**, HP is fixed around a
   2,000 pool, and **Crit / Attack Speed / Casting Speed / Movement Speed are set to Lv.5** — the cap.
2. **No consumables**, and HP-recovery skills heal only a fraction of their normal amount.
3. A round that hits 3:00 is decided by **total remaining HP**, with damage only as the second tiebreak.

Fact 3 is the one people under-price. HP is not just defence in AOS — it is a **scoring resource**.

---

## 2. Class dossiers

### Sage Awakening

Awakening Sage fights on a **Kibelius** with a **Talisman** offhand, and its identity is spatial
displacement plus large-area lightning. The kit is built around **Overcharge**: `Bolt` and `Lightning
Surge` gain bonus effects when cast after another skill that is off cooldown, and — crucially — **they
can be cast while on cooldown**. That single property makes them the best add-on carriers in the class,
which section 8 exploits.

The honest summary of the spec, from the class guide **[C]**:

> Awakening has a ranged grab but fewer protected CC options, and can be easier to catch out in prolonged
> fights because of their stamina issues.

So: **a ranged grab (`Seize`), a deep damage rotation, and a stamina problem.**

Damage core: `Upsurge` (which resolves as a ranged or melee version depending on the skill before it),
`Ator's Spear`, `Lightning Prison`, `Divine Executioner`, `Rift Storm`, `Chain Lightning`. `Core: Upsurge`
adds a **Stun** on the last hit and is the standard pick. `Enlightening Bolt` is a medium/long-range CC
with **Forward Guard**, and `Void Eruption` (Lv.58 rabam) gives Super Armor plus MP recovery.

### Hashashin Awakening

Awakening Hashashin fights on **Dual Glaives** with a **Haladie**, built on sandstorm repositioning and
short, brutal dive combos. Its protection profile is the opposite of Sage's: `Prophesy Blade` carries
Super Armor and a **+20 DP** self-buff, `Mirage Assault` runs Super Armor into Forward Guard with a
knockdown, and `Shadow Slicer` opens with Super Armor into stiffness. That is three independently
protected ways to start a fight, plus `Constriction` as a ranged grab.

The class guide is equally direct about the matchup shape **[C]**:

> In 1v1s, Awakening tends to be easier and better.

And on the defensive axis, Hashashin is one of only four classes where **Evasion is rated "good"** rather
than merely viable — the others being Striker, Mystic and Shai. Sage sits in the weaker "viable, in return
for less damage" tier. That asymmetry survives into AOS even though the arena supplies its own gear,
because base class stats are not normalised.

---

## 3. The three stat layers (and why "DR vs Eva" is the wrong question)

Most build arguments conflate three independent layers. In AOS they are:

| Layer | What you choose | What it actually controls |
|---|---|---|
| **1. Armour variant** | DR or Evasion version of each Resolute piece | The real DR↔Evasion exchange. Same DP, different split. |
| **2. Crystals** | 7 sockets from the AOS-exclusive pool | HP, AP, accuracy, crit/positional damage. **Hoom is the only defensive crystal**, and it gives DR *and* Evasion *and* HP. |
| **3. Add-ons** | 6 skills × 2 effects | Flat DP / Evasion / Accuracy, and damage-family multipliers. |

The consequence: **the crystal layer does not split DR from Evasion.** Whichever armour variant you run,
your defensive crystal package is the same Hoom setup. So "DR build vs Eva build" really means
*armour variant + how much bulk you buy in crystals* — and the bulk option is strictly better than people
assume.

### The crystal maths

Verified per-piece and set values **[V]**:

- **Ultimate Combined Hoom** (one piece): Acc +2 · DR +3 · Eva +5 · HP +75 · All Resistance +1%
- **Hoom 2-set**: DR +5 · HP +150 · Eva +4
- **Hoom 4-set**: DR +5 · HP +150 · Eva +4 · Acc +3 · All Resistance +3%

| Package | Acc | DR | Eva | HP |
|---|---:|---:|---:|---:|
| Hoom ×2 | +4 | +11 | +14 | **+300** |
| Hoom ×4 | +11 | +22 | +28 | **+600** |

Now put that against the other verified payloads:

- **Glorious Crystal of Gallantry – Resolute**: Extra AP vs Adventurers +2, All Accuracy +27, **Max HP +250**
- **Secrua's Wave Crystal**: Extra AP vs Adventurers +3, **Max HP +250**, Max Stamina +100
- **Time Spirit's Crystal – Plunder**: All AP +5 and a critical component **[C]**
- **Corrupted Light / Sacred Darkness**: AP +2 with +11% crit damage, or AP +3 with +12% back/down/air

Translate to a 2,000 HP pool:

```
+250 HP  = +12.5% of the pool
+300 HP  = +15.0%
+550 HP  = +27.5%
+11 DR   ≈ 11 damage removed per hit → ~88 over an 8-hit combo
           = ~3.4% of a 2,550 pool
```

**HP is worth roughly three to four times what an equivalent "slot" of DR is worth in AOS**, because HP
is not halved by the arena and DR numbers are. This is why the bulk preset wins the mirror, and it is why
the top-100 data keeps electing HP-bearing crystals over bigger damage lines.

---

## 4. Sage Awakening — DR preset

**Armour:** Damage Reduction variants of all four Resolute pieces.

| Socket | Crystal | Note |
|---|---|---|
| Main weapon | **Secrua's Flaming** | +5% all special attack damage — multiplicative, no downside since the Oct 2025 rework |
| Awakening | **Gallantry – Resolute** | Acc +27 is the real payload; Sage has many small hits that all want to land |
| Sub-weapon | **Corrupted Light** | AP +2, +11% crit damage — Sage crits constantly at Crit Lv.5 |
| Helmet | **Ultimate Combined Hoom** | |
| Armour | **Ultimate Combined Hoom** | completes the 2-set |
| Gloves | **Time Spirit's Plunder** | AP +5 |
| Shoes | **Missing Captain's Sail** | filler; Move Speed component is inert in AOS |

**Totals from crystals:** HP 2,550 · DR +11 · Eva +14 · Acc +31 · AP +7 · +11% crit damage.

**Why this is the "default" but not the best:** it keeps Plunder's AP and gives a 500 HP cushion, but it
leaves 550 HP and 11 DR on the table versus the bulk preset, in exchange for about 3% damage.

## 5. Sage Awakening — Evasion / bulk preset

**Armour:** Evasion variants of all four Resolute pieces.

| Socket | Crystal | Note |
|---|---|---|
| Main weapon | **Secrua's Wave** | +3 AP vs Adventurers, +250 HP, **+100 max stamina** |
| Awakening | **Gallantry – Resolute** | Acc +27, +250 HP |
| Sub-weapon | **Corrupted Light** | |
| Helmet / Armour / Gloves / Shoes | **Hoom ×4** | the whole defensive package |

**Totals from crystals:** HP **3,100** · DR +22 · Eva +28 · Acc +38 · no crystal AP.

**The Sage-specific argument for Wave over Flaming:** Sage Awakening is explicitly a stamina-hungry spec
**[C]**, and in a 3-minute round stamina is a second health bar. Wave is the only main-hand crystal in the
pool that adds max stamina. For every other class that line is decoration; here it is a real resource
injection. If you are confident in your stamina discipline, Flaming still wins on damage.

**Honest caveat on the armour variant:** Sage is in the *"Evasion is viable in return for less damage"*
tier, not the *"Evasion is good"* tier **[C]**. If your games feel like you are being hit through the
evasion anyway, move the armour pieces back to DR and keep everything else — you still pocket the 550 HP.

---

## 6. Hashashin Awakening — DR preset

**Armour:** Damage Reduction variants.

| Socket | Crystal | Note |
|---|---|---|
| Main weapon | **Secrua's Flaming** | Hashashin forces back attacks, so its special-attack share is high — this crystal overperforms here |
| Awakening | **Gallantry – Resolute** | |
| Sub-weapon | **Crystal of Sacred Darkness** | AP +3, +12% back/down/air — this is the class-defining pick |
| Helmet / Armour | **Hoom ×2** | |
| Gloves | **Time Spirit's Plunder** | |
| Shoes | **Missing Captain's Sail** | |

**Totals from crystals:** HP 2,550 · DR +11 · Eva +14 · Acc +31 · AP +8 · **+12% positional damage**.

## 7. Hashashin Awakening — Evasion / bulk preset

**Armour:** Evasion variants.

| Socket | Crystal | Note |
|---|---|---|
| Main weapon | **Secrua's Flaming** | |
| Awakening | **Gallantry – Resolute** | |
| Sub-weapon | **Crystal of Sacred Darkness** | |
| Helmet / Armour / Gloves / Shoes | **Hoom ×4** | |

**Totals from crystals:** HP **3,100** · DR +22 · Eva +28 · Acc +38 · +12% positional damage.

Hashashin is a *"Evasion is good"* class **[C]**, so the Evasion variant is doing more work here than it
does on Sage. Combined with Hoom ×4 this is the tankiest legal Hashashin in the mode.

### Preset summary — the actual numbers

| | HP | DR | Eva | Acc | AP | Damage line |
|---|---:|---:|---:|---:|---:|---|
| Sage DR | 2,550 | 11 | 14 | 31 | 7 | +11% crit |
| Sage bulk | **3,100** | **22** | **28** | **38** | +3 adv | — |
| Hash DR | 2,550 | 11 | 14 | 31 | 8 | +12% positional |
| Hash bulk | **3,100** | **22** | **28** | **38** | 0 | +12% positional |

*Sage's bulk row shows `+3 adv` rather than 0 because Secrua's Wave contributes Extra AP Against Adventurers, which
sits outside the flat-AP column.*

**+550 HP · +11 DR · +14 Eva · +7 Acc — for −5 AP and one damage line.** That is the entire trade. On a
2,000 HP base it is a **+21.6% relative EHP** purchase for roughly **3%** of your damage.

---

## 8. The universal add-on spec (both presets, per class)

One 6-skill × 2-effect build per class, deliberately written to be preset-agnostic: it leans on **All DP**
and **Accuracy** rather than Evasion, so it is not wasted on the DR preset, and it never spends a slot on
a speed level the arena has already maxed.

**System rules you are building inside [V]:** 6 skills, 2 effects each = 12 slots. Effect duration is set
by the skill's cooldown tier — Tier 1 ≤5s, Tier 2 5–13s (or ≥13s but usable during cooldown), Tier 3 ≥13s.
Stat buffs run **7 / 12 / 20s**, damage buffs **5 / 7 / 10s**, defensive buffs **10 / 15 / 25s** by tier.

> Uptime is the whole game: `U = min(1, duration / cooldown)`. A stat buff on a 4s skill is permanent; the
> same buff on a 12s skill with a 12s cooldown has zero slack and drops the moment you miss a recast.

### 8.1 Sage Awakening — universal PvP add-ons

| # | Skill | Effects | Why this carrier |
|---|---|---|---|
| 1 | **Shock Relay** | All DP +20 · All Accuracy +20 | The cancel hub of the kit — you touch it constantly, so the buff is effectively permanent |
| 2 | **Bolt** (or **Lightning Surge**) | All DP +20 · All Evasion +20 | **Castable while on cooldown** via Overcharge → the add-on re-applies on every use, which is the strongest uptime property any Sage skill has |
| 3 | **Upsurge** | Down Attack +5% · Critical Hit Damage +5% | Your damage core, and it lands on knocked-down targets; `Core: Upsurge` adds the Stun that sets it up |
| 4 | **Ator's Spear** | Back Attack +5% · Critical Hit Damage +5% | Second burst window, cancels cleanly into Upsurge |
| 5 | **Lightning Prison** | All DP −20 · All Evasion −20 | Biggest reliable AoE in the kit → best debuff spread onto a stacked 3v3 |
| 6 | **Divine Executioner** | All DP +20 · All Evasion +20 | Long-cooldown finisher: at Tier 3 the defensive buff lasts 25s, covering a whole engage-disengage cycle |

*Tier note:* slots 1–2 must resolve as Tier 1 or Tier 2. If your client shows a **shorter** duration than
the table above, the skill is a lower tier than assumed — move that effect to the next skill down rather
than accepting the shorter window.

### 8.2 Hashashin Awakening — universal PvP add-ons

| # | Skill | Effects | Why this carrier |
|---|---|---|---|
| 1 | **Haladie Throw** | All DP +20 · All Accuracy +20 | Fast, ranged, low-commitment — the safest permanent buff carrier in the kit |
| 2 | **Aal's Breath** | All DP +20 · All Evasion +20 | Short cooldown and used in every engage |
| 3 | **Sin Splitter** | Down Attack +5% · Critical Hit Damage +5% | The 1v1 core (and a common `Core:` pick); this is the skill that converts a CC into a kill |
| 4 | **Descent** | Back Attack +5% · Critical Hit Damage +5% | Your dive; almost always lands from behind, so the positional line is live |
| 5 | **Quicksand** / **Ensnaring Sands** | All DP −20 · All Evasion −20 | Multi-hit AoE → best debuff uptime; two allies benefit from every application |
| 6 | **Aal's Command** | All DP +20 · All Evasion +20 | Long-cooldown anchor skill: 25s of defensive buff off one cast |

*Tier note:* as above — confirm the durations in the skill window (K) before you commit; the effect is
correct, the carrier may need to move one slot.

### 8.3 What is deliberately absent, and why

| Effect | Verdict in AOS |
|---|---|
| Attack Speed +10% | **Zero value.** Pinned at Lv.5 on entry. |
| Casting Speed +10% | **Zero value.** Same cap. |
| Movement Speed +10% | **Zero value.** Same cap. |
| Critical Hit **Rate** +30% | Mostly clipped — you enter at Crit Lv.5. Take crit **damage** instead. |
| Bleed | Flat, non-scaling, healed through by the arena's equalised regeneration. |
| Recover MP per hit | Sage: unnecessary (Void Eruption and passives cover it). Hashashin: low value. |

That is four of the most commonly copied add-on lines in the game contributing nothing in this mode.

---

## 9. The test

Four rounds. Three are computable; one is a judgement call with the weights exposed.

### Round 1 — Damage ratio: **tie**

Both specs are **Skirmisher** **[V]**. Skirmisher deals +5% to Vanguard and takes no bonus against
another Skirmisher, so in this specific matchup both classes sit on the flat 89.29% PvP ratio.

> The rock-paper-scissors layer that dominates most AOS matchups is **completely absent here**. Any
> "Sage counters Hashashin" or reverse claim has to be argued from kit, not from ratios.

### Round 2 — Bulk vs damage, in the mirror: **bulk preset wins by ~20%**

Model a full combo as 8 hits, and compare the two presets as the *defender* against the same attacker.

```
Defender = DR preset:    2,550 HP + 11 DR × 8 hits = 2,638 effective HP
Defender = bulk preset:  3,100 HP + 22 DR × 8 hits = 3,276 effective HP

Attacker on DR preset:   ×1.033 (AP +5)
Attacker on bulk preset: ×1.000

Nominal damage needed to kill:
  vs DR preset   = 2,638 / 1.033 = 2,554
  vs bulk preset = 3,276 / 1.000 = 3,276

⇒ the bulk preset requires 28% more incoming damage to kill.
   The attacker's damage advantage is 3.3%.
```

The bulk preset is not a "tanky but harmless" build — it is a 28%-more-durable build that gives up about
3% of its output. In a mirror where neither side has a ratio edge, that is not close.

So why do 70% of the top 100 still run DR armour? Because their armour variant buys a much larger DR
number than Hoom does, and because DR is far more reliable against high-accuracy burst than evasion is.
The crystal layer and the armour layer point in opposite directions; the armour layer is the bigger term,
and it is the one I cannot put a number on from public data.

### Round 3 — Kit asymmetries: **Hashashin**

| Axis | Sage Awakening | Hashashin Awakening | Edge |
|---|---|---|---|
| Ranged grab | `Seize` | `Constriction` | Tie — both now carry a 0.4–0.7s startup and a visible tell **[V]** |
| Protected CC entries | Fewer, by the class guide's own summary **[C]** | `Prophesy Blade` (SA), `Mirage Assault` (SA→FG, KD), `Shadow Slicer` (SA, stiffness) | **Hashashin** |
| Range / poke | Medium-long, `Enlightening Bolt` with FG, `Energized Thorn` | Short-medium | **Sage** |
| Stamina economy | Explicitly a weakness **[C]** | No comparable tax | **Hashashin** |
| Evasion affinity | "Viable, less damage" **[C]** | "Good" **[C]** | **Hashashin** |
| Burst ceiling | Very high on a clean grab | High, more conditional | Tie |

### Round 4 — Empirical: **Hashashin**

Fall 2026 top 100, pooled NA/EU/KR/SA **[V]**:

| | Players | Avg rating | Best | Win rate |
|---|---:|---:|---:|---:|
| Hashashin (Awakening) | 5 | **2,044** | 2,409 | 56.0% |
| Sage (Awakening) | 2 | 1,885 | 1,889 | 74.7% |

Hashashin has 2.5× the representation and a **+159 average rating**. Sage's 74.7% win rate is a two-player
sample and should be read as noise, not as a hidden top-tier pick.

### Weighted verdict

| Criterion | Weight | Sage | Hashashin |
|---|---:|---:|---:|
| Top-level representation | 25% | 2 | 4 |
| Average rating | 20% | 2 | 5 |
| Protected CC access | 20% | 3 | 4 |
| Range / anti-dive | 15% | 5 | 3 |
| Stamina economy | 10% | 2 | 5 |
| Ceiling | 10% | 4 | 4 |
| **Weighted total** | | **2.85** | **4.15** |

**→ 59.3% : 40.7% in Hashashin's favour.**

Read that as a *matchup prior*, not a law. The 41% is real: Sage wins this fight whenever it gets to play
at maximum Seize range, because a single clean grab converts into a kill and Hashashin has no answer to
being held at distance. The reason the prior still favours Hashashin is that Sage has to spend stamina to
maintain that distance, and a 3-minute round is long enough for the stamina tax to be collected.

---

## 10. Counter-play, distilled

**If you are the Sage:**
1. Run the **bulk preset**. You are the class that gets caught; buy the HP.
2. Take **Resolute** over Olucas — Hashashin is an evasion-favourable class, so 27 accuracy is doing real
   work here.
3. **Never chase.** Your win condition is a single `Seize` at max range. Every step you take toward him is
   stamina you cannot spend escaping.
4. Bait `Constriction`. It now has a 0.4–0.7s wind-up and a visible effect **[V]** — that window is your
   punish.

**If you are the Hashashin:**
1. Run the **bulk preset** too. The mirror is decided by who survives the first combo, not who lands it.
2. Take **Sacred Darkness**. Your damage is back-attack shaped; +12% positional beats +11% crit.
3. **Pressure the stamina bar, not the health bar.** Force a `Bolt` and a `Rift Storm` out of him before you
   commit — a Sage with no stamina is a Sage with no escape.
4. Do not open with `Constriction` into a Sage holding Forward Guard. Open with a protected CC
   (`Prophesy Blade`, `Mirage Assault`) and hold the grab for his escape.

---

## 11. Verify before you commit

Two items in this write-up are community-consistent rather than officially published, and the add-on
carriers depend on cooldowns your client will show you exactly. Sixty seconds, four checks:

| Check | Where | What you are looking for |
|---|---|---|
| Add-on magnitudes | Skill window (K) → hover | All DP +20 / All Evasion +20 / All Accuracy +20; damage families +5% |
| Crit & speed caps | My Stats while queued | Crit / Atk Spd / Cast Spd / Move Spd all Lv.5 — this is what justifies deleting speed add-ons |
| Plunder payload | Set Gear → glove tooltip | AP +5 plus a crit line; note whether it is crit *rate* (partly clipped) or crit *damage* |
| Cooldown tiers | Skill window (K) → each carrier | Confirm slots 1–2 resolve as Tier 1/Tier 2, and slot 6 as Tier 3 |

**And the best habit in the mode:** Arena of Solare menu → Rankings → filter to your class → magnifying
glass. You get that player's exact crystals and exact add-ons. It is the answer key, updated live, and it
beats any written guide — including this one.

---

## 12. Sources

- **Damage Calculation Formula Overhaul** (Jul 17, 2025) — unified 89.29% PvP ratio, Vanguard/Skirmisher/Pulverizer
  groups, removal of Accuracy Rate, add-on species-damage removal.
  https://blackdesert.pearlabyss.com/Console/en-US/News/Notice/Detail?_boardNo=12358
- **Arena of Solare rules & season** (Oct 15 – Dec 10, 2026) — halved AP/DR/Acc/Eva, Lv.5 crit and speeds,
  guard gauge equalisation, HP-decided timeouts.
  https://orbit-games.com/en/black-desert-en/pvp-bdo-en/arena-of-solare
- **AOS exclusive crystal pool and stats** (Oct 23, 2025 + Nov 13, 2025 patch notes) — Wave, Flaming, Resolute,
  Corrupted Light, Sacred Darkness, Hoom, Macalod, Providence, Sail.
  https://blackdesert.pearlabyss.com/Console/en-US/News/Notice/Detail?_boardNo=12556
- **Global Lab Oct 8, 2026 / live Oct 15, 2026** — Secrua's Wave changed to +3 AP vs Adventurers / +250 HP /
  +100 stamina; Family Fame 2,500 gate; map rotation.
  https://orbit-games.com/en/black-desert-en/global-lab-en/english-patch-notes-global-lab-bdo-08-10-2026
- **AOS top-100 build census, Fall 2026** — per-socket crystal usage, armour archetype split, class counts.
  https://cogm.app/bdo/meta/solare?region=NA&season=fall-2026&view=builds
- **Sage class guide** — awakening kit, `Seize`, Overcharge mechanic, stamina weakness, protected-CC summary.
  https://www.blackdesertfoundry.com/sage-class-guide
- **Hashashin class guide** — awakening kit, `Constriction`, protected skills, evasion-class tiering.
  https://www.blackdesertfoundry.com/hashashin-class-guide
- **Skill add-on system** — 6 skills × 2 effects, tier and duration tables.
  https://garmoth.com/guides/post/all-new-skill-add-ons

---

*Written as a lab notebook, not a gospel. The reasoning in §3, §8 and §9 is designed to survive a numbers
patch; the specific crystal verdicts are not. Season ends Dec 10, 2026 — re-run the census after the next
season opens before trusting the percentages.*
