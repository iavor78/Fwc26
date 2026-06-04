# 🏆 Special Team League — FIFA World Cup 2026

A real-time fantasy league tracker for 4 players following the FIFA World Cup 2026 (USA · Canada · Mexico).

**Live app:** [iavor78.github.io/Fwc26](https://iavor78.github.io/Fwc26)

---

## 🎲 The Draw

### Group Stage Draw
Each group (A–L) has 4 teams. Each player is assigned **one team per group**, giving every player **12 teams** across all 12 groups. The draw is done manually and entered in the **Draw** tab.

### Knockout Draw
After the group stage, a separate draw is held for each KO round:
- **Round of 32** — 8 teams per player
- **Round of 16** — 4 teams per player
- **Quarter-Finals** — 2 teams per player
- **Semi-Finals** — 1 team per player
- **3rd Place & Final** — 1 team per player each

Teams in the KO draw are drawn from those that actually qualified. The same team cannot be assigned to two different players in any round.

---

## ⚽ Scoring

### Group Stage
Points are awarded per match, per player who owns that team:

| Result | Points |
|--------|--------|
| Win | 3 |
| Draw | 1 |
| Loss | 0 |

**Goal Difference** and **Goals For** are tracked as tiebreakers.

### Knockout Rounds
KO matches that are decided at **Full Time**:

| Result | Points |
|--------|--------|
| Win (FT) | 3 |
| Loss (FT) | 0 |

KO matches decided on **Penalties** (FT score is a draw):

| Result | Points |
|--------|--------|
| Win (pens) | 3 |
| Loss (pens) | 0 |

> **Note:** When a KO match goes to penalties, the Full Time score is used for Goal Difference. The penalty shootout result determines who receives the 3 points — no draw points are awarded in KO rounds.

---

## 📊 League Table

The main **Table** tab shows the overall standings across all 4 players, accumulating points from every match across the group stage and all KO rounds. The player whose teams score the most points across the entire tournament wins.

Tiebreakers (in order):
1. Points
2. Goal Difference
3. Goals For

---

## 🏅 Qualification — Best 3rd-Placed Teams

In WC2026, the top 2 teams from each of the 12 groups qualify automatically for the Round of 32. Additionally, the **8 best 3rd-placed teams** across all 12 groups also qualify.

3rd-placed teams are ranked by:
1. Points
2. Goal Difference
3. Goals For

The **Groups** tab shows live 3rd-place standings and which teams are currently in the qualifying 8.

---

## 📱 App Features

| Tab | Description |
|-----|-------------|
| 🏆 Table | Overall league standings across all 4 players |
| 📊 Groups | Live group standings (A–L) + best 3rd-place ranking |
| 🔗 Bracket | Full KO bracket from R32 to Final |
| 🎲 Draw | Group and KO team assignments per player |
| ⚽ Matches | Enter match scores (group stage + all KO rounds) |
| 👤 Players | Edit player names, simulate, reset data |

### Real-Time Sync
All data syncs instantly across all devices via Firebase. Share the URL with all 4 players — everyone sees the same live state.

### Lock 🔒
The admin can lock the app from the footer to prevent others from editing scores while a review is in progress. Tap 🔒 to lock, 🔓 to unlock.

### Simulate
The Players tab includes a simulate function to test or demo the app:
1. Assign teams randomly to all players
2. Simulate group stage results
3. Simulate KO round results
4. Clear all sim data (keeps player names)

---

## 🗓️ Tournament

- **Kick-off:** 11 June 2026
- **Final:** 19 July 2026
- **Host nations:** 🇺🇸 USA · 🇨🇦 Canada · 🇲🇽 Mexico
- **Teams:** 48 nations across 12 groups
- **Matches:** 104 total

---

*Built with vanilla JS + Firebase Firestore · Deployed on GitHub Pages*
