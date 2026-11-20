# ⚔️ Weapons & Fighting

![Fighting](https://img.shields.io/badge/Guide-Weapons%20%26%20Fighting-8f1d1d?style=for-the-badge)

How damage, armour, tiers and durability work in Rise RP Miami.

**Jump to:** [Damage](#-damage) · [Tiers](#-tiers) · [Body Armour](#%EF%B8%8F-body-armour) · [Reading a Hit](#-reading-a-hit) · [Durability](#-durability) · [Energy](#-energy)

---

## 💥 Damage

Your damage goes up with your **combat level** (max **25**). Each hit rolls inside the range.

| Level | Sword | Axe | Bat | Fists |
|---|---|---|---|---|
| 1 | 6–7 | 5–6 | 4–5 | 2–3 |
| 5 | 8–9 | 7–8 | 6–7 | 4–5 |
| 10 | 10–11 | 9–10 | 7–8 | 5–6 |
| 15 | 12–13 | 11–12 | 9–10 | 7–8 |
| 20 | 14–15 | 13–14 | 11–12 | 9–10 |
| 25 | 16–17 | 15–16 | 13–14 | 11–12 |

> [!NOTE]
> These are **Gray** (as bought) weapons hitting someone with **no vest**.

- 🪓 **Axe:** some hits **stun** the target for a moment.
- 🔪 **Knife:** light and fast, low damage.

---

## 🌈 Tiers

Upgrade weapons and armour at the **Bass Pro Workbench** (see the Crafting wiki).

| Tier | Weapon extra damage | Weapon blocks | Glow |
|---|---|---|---|
| ⬜ Gray | – | – | No |
| 🟩 Green | – | 3% | No |
| 🟦 Blue | +5% | 6% | No |
| 🟪 Purple | +12% | 10% | ✨ Yes |
| 🟨 Gold | +25% | 15% | ✨ Yes |

**Gold at level 25:** Sword **20–21** · Axe **19–20** · Bat **16–18**

---

## 🛡️ Body Armour

Body Armour takes a **%** off every hit you take. Better tiers can also **hit back**.

| Tier | Blocks | Hits back |
|---|---|---|
| ⬜ Gray | 4% | – |
| 🟩 Green | 7% | – |
| 🟦 Blue | 11% | 8% chance, 20% of the hit |
| 🟪 Purple | 15% | 12% chance, 25% of the hit |
| 🟨 Gold | 20% | 18% chance, 30% of the hit |

> [!IMPORTANT]
> Armour block + weapon block add up, but **total blocking is capped at 35%**.

---

## 📖 Reading a Hit

The hit message tells you what happened:

```
*slashes Cass with their sword, dealing 12 damage*
*slashes Cass with their sword, dealing 17 damage (+4 Gold)*
*slashes Cass with their sword, dealing 13 damage (-1 Armour)*
*slashes Cass with their sword, dealing 16 damage (+4 Gold, -1 Armour)*
```

- **+X Gold** = extra damage from the weapon's tier.
- **-X Armour** = damage the target's vest took off.
- **-X Blocked** = damage their weapon's tier blocked (no vest).
- When armour **hits back**: `*armour reflects 5 damage on to X*`

---

## 🔧 Durability

Every **landed hit** wears down the weapon **and** the vest it hits. **Misses cost nothing.**

| Hit with | Weapon loses | Vest it hits loses |
|---|---|---|
| 🔪 Knife | 2 | 2 |
| 🏏 Bat | 2–3 | 2–3 |
| 🪓 Axe | 3–4 | 3–4 |
| ⚔️ Sword | 3–5 | 3–5 |
| ✊ Fists | – | 1 |
| ⚡ Stun gun | 2 per stun | – |

**Better tiers wear slower:**

| Tier | Lasts |
|---|---|
| ⬜ Gray | 1x |
| 🟩 Green | ~1.3x |
| 🟦 Blue | ~1.8x |
| 🟪 Purple | ~2.5x |
| 🟨 Gold | ~3.6x |

> [!WARNING]
> At **0** it **breaks and is gone**: `*Their Sword breaks and falls apart*`. Get it repaired at **Bass Pro** before that happens.

---

## ⚡ Energy

Fighting and actions use **energy**. Store chips refill it.

| Action | Energy |
|---|---|
| Sword · Axe · Bat · Stun | -2 |
| Landing or missing a hit | -2 |
| Stun gun | -4 |
| Push · Pull | -5 |
| Stolen pepper spray · Stolen flashbang | -5 |
| Throwing knife | -10 |
| Drugs | -10 |
| Thrown bomb · TNT | -15 |
| Suicide vest | -20 |
| Cop loadout (flashbang, pepper spray, cuffs) | 0 |
