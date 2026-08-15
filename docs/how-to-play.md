# Throne of Kings — How to Play

Welcome to Throne of Kings. Two kingdoms clash on the battlefield. Summon your forces, advance your lines, and crush your opponent's Morale before they crush yours.

---

## The Goal

**Break your opponent's army before they break yours.**

You win by achieving one of two things:
- **Morale Collapse** — reduce the opponent's Morale to zero
- **Complete Exhaustion** — force a state where their deck is empty and they have no units left on the field (not counting a lone King)

---

## Your Resources

You have three things to track each turn:

### 👑 Glory
- Starts at **10** and gains **+1 every turn**
- Also gained by **killing enemy units** (+1 per kill)
- Only spent on **Legendary units** — they cost Glory to summon instead of Authority

### ⚔ Authority
- Starts at **20** and is generated each turn by your **King**
- Spent to **summon units** and **move units** (1 Authority per non-Legendary unit)
- Legendary units are free to move
- If you crown a new King while one is already alive, your Authority resets to 0

### ❤️ Morale
- Starts at **20** — this is your life total
- Every time one of your units dies, you lose **1 Morale**
- If a unit that has **consumed allies** dies, you lose extra Morale (see Civil War)
- If your Morale hits **0**, you lose immediately
- Morale cannot be recovered

---

## Your Cards

Cards come in several types:

| Type | What it does |
|------|-------------|
| **Human / Div / Beast / Hybrid** | Units — summon them to fight |
| **King** | Special unit — generates Authority each turn, powers your army |
| **Equipment** | Attach to a unit to boost its stats |
| **Trap** | Place face-down — activates automatically when the opponent does something |
| **Event** | Play immediately for a one-time effect |

### Unit Ranks

Every unit has a rank that determines how you pay for it:

| Rank | Paid with | Move cost |
|------|-----------|-----------|
| Troop | Authority | 1 |
| Elite | Authority | 1 |
| Legendary | Glory | Free to move |
| King | Authority | 1 |

### Unit Stats
- **⚔ Attack** — how much damage it deals
- **❤️ Vitality** — its hit points
- **🛡 Armor** — reduces incoming physical damage
- **Ranged Protection** — reduces incoming ranged damage

---

## The Battlefield

The battlefield is split into two halves — yours and your opponent's. Each half has **4 rows** and **3 columns**.

```
Your side:
[ Capital ] [ Reserve ] [ Support ] [ Frontline ] | [ Frontline ] [ Support ] [ Reserve ] [ Capital ]
  ← back                                                                               front →
```

- Your **Frontline** is closest to the enemy
- Your **Capital** is furthest back
- Columns represent left, center, and right lanes
- Multiple units can stack on one tile

---

## A Turn, Step by Step

Every turn follows the same order:

```
Dawn → Command → Battle → Civil War → (next player's turn)
```

---

### 🌅 Dawn (automatic)
At the start of your turn:
- Your King generates **Authority** for you
- You gain **+1 Glory**
- You draw **1 card**
- Status effects tick (poison damages, regen heals, stun/debuffs count down)
- Any opponent traps set to trigger at turn start fire

---

### ⚙️ Command Phase
This is your main action window. You can do as many actions as your resources allow:

**Summon a unit**
1. Click a card in your hand — it highlights
2. Click a friendly tile on the board — the unit appears there
3. Authority (or Glory for Legendaries) is deducted

**Move a unit**
1. Click one of your units — it highlights
2. Click a destination tile — the unit moves
3. Costs 1 Authority per non-Legendary unit
4. Moving into an **enemy-occupied tile** triggers immediate combat
5. Shift-click multiple units to move them as a group

**Play an Event card**
- Click an Event card in your hand — it resolves immediately

**Place a Trap**
- Click a Trap card — it goes face-down and waits to trigger

When you're ready, press **Begin Battle**.

---

### ⚔️ Battle Phase
Time to fight. Your units can no longer move — only attack.

**Attack**
1. Click one of your units — it highlights
2. Click an enemy unit to attack it

**Group attack**
1. Shift-click multiple friendly units to select them all
2. Click an enemy unit — all selected units attack that target

**Combat resolution:**
- Your unit deals its Attack as damage to the target
- If the target survives and the attack was physical (not ranged), **it retaliates**
- Ranged units attack without triggering retaliation
- Curse attacks bypass armor and retaliation
- Armor reduces physical damage. Ranged Protection reduces ranged damage
- When a unit reaches 0 Vitality, it dies — its owner loses 1 Morale

**Guard rule:** If an enemy has a unit with the **Guard** keyword within range, you must attack it before attacking anything else.

When you're done attacking, press **End Turn**.

---

### ⚔️ Group Combat (Collision)
When you move **multiple units** into an enemy-occupied tile, a collision happens:
- All your attacking units strike the enemy group together (damage is pooled)
- Armor still applies
- Surviving defenders then strike back at your group
- Dead units are removed, surviving units occupy the tile

---

### 🔥 Civil War Phase (optional)
After battle, before your turn ends, you can take optional actions.

Press **End Civil War** to skip this phase entirely.

**Retire a unit**
- Click a friendly unit, then click it again to confirm
- The unit is permanently removed
- You lose **1 Morale** for retiring a fresh unit
- If the unit previously consumed allies (see below), you lose more Morale

**Consume (Div and Beast units only)**
- Click a Div or Beast unit to select it
- Click an **adjacent** friendly unit to consume it
- The consumed unit is permanently removed — **no Morale cost right now**
- The consumer gains bonus stats (half of the consumed unit's attack and vitality, minimum 1 each)
- The consumer now carries a **💀 debt** — shown as 💀N on the board
- When the consumer eventually dies (in battle, retirement, or any other way), you pay **1 + N Morale** instead of just 1
- Consuming a consumer absorbs their full debt chain

**Key rule:** Consuming is a trade — you grow a powerful unit now, but you'll pay more Morale if it dies later.

---

## Keywords

Keywords are special abilities printed on cards. Here are the ones you'll encounter:

| Keyword | What it does |
|---------|-------------|
| **Charge** | Gains bonus attack when it moved this turn before attacking |
| **Ranged** | Attacks from any distance, no retaliation |
| **Swift N** | Can move N extra tiles |
| **Flying** | Can move anywhere on the board in one move |
| **Guard** | Enemies must attack this unit first if it is in range |
| **Regenerate N** | Heals N Vitality at the start of each turn |
| **Fear N** | Enemies attacking this unit deal N less damage. Fearless units ignore this. |
| **Fearless** | Immune to Fear |
| **Heroic** | Permanently gains +1 Attack each time it survives combat damage |
| **Brave** | Gains bonus attack when your army is outnumbered |
| **Aggressive N** | Always deals +N extra attack damage |
| **Burn N** | Deals +N bonus damage after armor mitigation |
| **Massive** | Reduces incoming attack damage |
| **Predator** | Gains bonus attack when attacking a wounded enemy (below half HP) |
| **Brutal N** | Gains bonus attack when attacking any damaged enemy |
| **Commander N** | Adjacent allies gain +N attack |
| **Support N** | Adjacent allies gain +N attack (similar to Commander) |
| **Leader N** | All allies gain +N armor at the start of each turn |

---

## Traps

Traps are placed face-down during the Command phase and activate automatically.

| Trigger | When it fires |
|---------|--------------|
| Enemy Move | When the opponent moves any unit |
| Enemy Summon | When the opponent summons a unit |
| Enemy Attack | When the opponent declares an attack |
| Turn Start | At the start of the opponent's turn |

**Trap effects:**
- **Damage** — deals physical damage to a target unit (armor applies)
- **Stun** — the target cannot move or attack for one turn
- **Attack Debuff** — reduces the target's attack for one turn

---

## The King

Your King is your most important unit.

- Generates **Authority** for you every turn
- When a King is on the field, your army fights at full strength
- You can only have **one King** at a time — crowning a new King resets your Authority to 0
- The King's death does not end the game, but it weakens your army

---

## Winning and Losing

### You lose by Morale Collapse
Your Morale hits 0. This happens faster than you think — every unit death costs 1 Morale, and consumers can cost even more when they die.

### You lose by Complete Exhaustion
Your deck is empty **and** you have no units on the battlefield (a lone King doesn't count).

### Tips for staying alive
- Don't overextend — a dead unit is lost Morale
- Think twice before consuming with a Div or Beast — that debt follows the unit forever
- Keep your Frontline defended so your Capital isn't exposed
- Ranged units can attack safely. Use them to chip away without taking retaliation
- Guard units protect the rest of your army — place them in front

---

## Quick Reference

| Action | Phase | Cost |
|--------|-------|------|
| Summon unit | Command | Authority (or Glory for Legendaries) |
| Move unit | Command | 1 Authority per unit |
| Attack | Battle | Free |
| Retire unit | Civil War | 1+ Morale |
| Consume ally | Civil War | 0 Morale now (debt paid on consumer death) |
| End Battle → Civil War | — | Press "End Turn" |
| End Civil War | — | Press "End Civil War" |

---

*Good luck, Commander.*