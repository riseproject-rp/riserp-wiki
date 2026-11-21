# Rise Fight Club

The boxing arena at the Lucky Devil (room `fightclub.room_id`, default **10**).
Players set up fights, bet on themselves, and climb the weekly and all-time boards.

---

## Starting a fight

1. Stand on one of the arena **action points**. The **Fight Club** menu opens.
2. On the **Fight** tab, pick:
   - **Mode**: 1 v 1, 2 v 2 or 3 v 3
   - **Rounds**: 1, 2 or 3
   - **Bet**: Friendly, a preset amount, or any amount you type
3. **Invite** players by name, or from the *Everyone in this room* list.
   VIPs in the club rooms (`fightclub.vip_invite_rooms`) can be invited too.
4. Invited players get a card with the mode, the rounds and the **bet**.
   They have 30 seconds to **Accept** or **Decline**.
5. Once both teams are full, the fight goes straight into the **queue**.

Roleplay lines:

| When | Money bet | Friendly |
|---|---|---|
| Asking | `*Asks Tracy to box for $200*` | `*Asks Tracy to a friendly boxing match*` |
| Accepting | `*Accepts Yan's request to box for $200*` | `*Accepts Yan's request to a friendly boxing match*` |

---

## Betting: fighters only

Only the fighters bet, on their own fight. Players watching cannot bet.

- The **host** picks the bet before anyone accepts. After that it is locked.
- Every fighter puts in the same amount.
- You can only invite or accept if you have the money.
- The money is taken when the fight **starts**, not when you accept.
  Anyone who can't cover it by then cancels the fight.
- **The winning side takes the losing side's money**, and gets its own back.
  - 1 v 1 at $200: the winner gets **$400**.
  - Team fights: the losers' money is split between the winners.
- **Draw, cancelled fight or server restart = full refund.**

| Setting | Default | What it does |
|---|---|---|
| `fightclub.stake_amounts` | `50,100,200,500,1000` | The quick-pick buttons |
| `fightclub.stake_max` | `100000` | The most anyone can bet |

---

## Fighting

- The fighters are teleported into the ring, the lights come on: **3, 2, 1, FIGHT!**
- Stand next to an opponent and use **`:hit`** (or the punch button).
- Each fighter has **100 HP** (`fightclub.hp`).
- A hit does **10 damage** (`fightclub.punch_min` / `punch_max`). A crit (10% chance) does about 18.
- The one who gets hit says how much it took: `*takes the hit* -10 HP`.
- **Misses**: 25% of swings miss (`fightclub.miss_chance`).
- **Knockout punch**: a small chance (`fightclub.ko_chance`, 3%) once someone is on their last bit of health.
- Empty the other side's bars = **KO** = round won. Health comes back for the next round.
- First to win the majority of rounds wins the match.

### The clock and overtime

- A match runs for **3 minutes** (`fightclub.match_seconds`).
- If the clock runs out **while they're still fighting**, the match goes to **OVERTIME**.
  Nobody is thrown out mid-fight.
- The match only stops when **nobody has moved or thrown a punch for 2 minutes**
  (`fightclub.idle_seconds`, 120). One fighter moving is enough to keep it going.
- In overtime, the clock on the board shows that 2-minute countdown. It starts over every time someone moves or swings.
- When it stops, whoever won more rounds wins. Equal rounds = **draw**, and bets go back.

### Ending early

| What happens | Result |
|---|---|
| A fighter walks out of the ring | They count as knocked out |
| A fighter disconnects or reloads | Fight cancelled, everyone refunded |
| The host cancels before it starts | Fight cancelled, everyone refunded |

---

## Boxer Customization

On the **Boxer Customization** tab, pick colours for your **top** (women), **shorts** and **gloves**.
You wear the outfit automatically in the ring, and your normal clothes come back after.

---

## Boards

- **Weekly**: wins, losses, KOs, damage and fights. Resets **Monday 12:00 AM Central**.
  Click a fighter to see who they fought this week.
  The **top 3** stand on the podium in the arena.
- **All Time**: every fight since the club opened, ranked by wins then KOs. It never resets.
- The arena board shows the fight that's on now, the HP bars, hits, damage and KOs, and the last 3 fights.

---

## Commands (the menu sends these)

| Command | What it does |
|---|---|
| `:fight mode <1-3>` | Fight size |
| `:fight rounds <1-3>` | Number of rounds |
| `:fight bet 0 stake <amount>` | Set the fighters' bet (0 = friendly) |
| `:fight invite <name>` | Invite someone |
| `:fight accept <id>` / `decline <id>` | Answer an invite |
| `:fight leave` | Leave or cancel before the fight starts |
| `:hit [name]` | Punch, in the ring |
