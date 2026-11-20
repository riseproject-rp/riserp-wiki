# ⚔️ Weapons & Fighting

![Fighting](https://img.shields.io/badge/Guide-Weapons%20%26%20Fighting-8f1d1d?style=for-the-badge)

How damage, armour, tiers and durability work in Rise RP Miami.

**Jump to:** [Damage](#-damage) · [Tiers](#-tiers) · [Body Armour](#%EF%B8%8F-body-armour) · [Reading a Hit](#-reading-a-hit) · [Durability](#-durability) · [Energy](#-energy)

---

## 💥 Damage

Your damage and your **health** both go up with your **combat level** (max **25**). Health goes from **100** at level 1 to **150** at level 25, so fights take about the same number of hits at every level.

| Weapon | Level 1 | Level 10 | Level 25 | Hits vs your own level |
|---|---|---|---|---|
| Sword | 12–13 | 14–15 | 18–19 | ~8–9 |
| Axe | 10–11 | 12–13 | 16–17 | ~10 |
| Bat | 8–9 | 10–11 | 13–14 | ~12 |
| Knife | 5–6 | 6–7 | 8–9 | ~18 (fastest swing) |
| Fists | 5–6 | 6–7 | 8–9 | ~18 |

> [!NOTE]
> These are **Gray** (as bought) weapons hitting someone with **no vest**. A level 25 beats a level 1 about **2 to 1**.

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

**Gold at level 25:** Sword **23–24** · Axe **20–21** · Bat **16–18**

---

## 🛡️ Body Armour

Body Armour takes a **%** off every hit you take. Better tiers can also **hit back** and **dodge stuns**.

| Tier | Blocks | Hits back | Stun dodge |
|---|---|---|---|
| ⬜ Gray | 4% | – | – |
| 🟩 Green | 7% | – | – |
| 🟦 Blue | 11% | 8% chance, 20% of the hit | 5% |
| 🟪 Purple | 15% | 12% chance, 25% of the hit | 10% |
| 🟨 Gold | 20% | 18% chance, 30% of the hit | 15% |

**Stun dodge** = chance to shrug off a stun gun or axe stun.

> [!IMPORTANT]
> Armour block + weapon block add up, but **total blocking is capped at 35%**.

---

## 📖 Reading a Hit

The hit message tells you what happened:

```
*slashes Cass with their sword, dealing 18 damage*
*slashes Cass with their sword, dealing 23 damage (+5 Gold)*
*slashes Cass with their sword, dealing 18 damage (-1 Armour)*
*slashes Cass with their sword, dealing 22 damage (+5 Gold, -1 Armour)*
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
