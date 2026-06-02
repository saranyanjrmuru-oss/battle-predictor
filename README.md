# ⚔ Battle Predictor — Adaptive AI Combat Game

> An MLP-based adaptive combat game built with pure HTML/JavaScript — no ML libraries used.

## 🎮 Play the Game

Open `index.html` in any browser, or host on GitHub Pages for online demo.

---

## 🧠 How the AI Works (MLP Prediction)

The enemy AI uses a **Multi-Layer Perceptron-style weight matrix** to predict your next move:

```
weights[playerMove][action] = probability
```

- Every time you choose **Attack**, **Defend**, or **Heal**, the AI records it
- The weight matrix updates using a **learning rate of 0.15** — reinforcing patterns it detects
- It looks at your **last 5 moves**, weighting recent actions more heavily
- The AI then picks the **counter action** based on the most probable prediction
- The **prediction bar** at the top shows exactly what the AI thinks you'll do next

The more you play, the smarter the Oracle becomes!

---

## ✅ Assignment Requirements Met

| Requirement | Status |
|---|---|
| Python/JS only | ✅ Pure HTML/JavaScript |
| No ML libraries | ✅ Custom MLP weight engine |
| Adaptive AI behavior | ✅ Pattern recognition + counter logic |
| Score system | ✅ Score, wins, streak tracker |
| Health system | ✅ HP bars for player and enemy |

---

## ⭐ Extra Features Added

1. **🔊 Sound Effects** — Web Audio API: attack, defend, heal, hit, combo, win, lose sounds
2. **🎒 Inventory System** — 4 usable items: Elixir (heal), Bomb (damage), Rune (regen), Ward (shield)
3. **💫 Visual Effects** — Floating damage numbers, particle bursts, flash animations
4. **🏆 Leaderboard** — Top 10 scores saved via localStorage
5. **⚡ Combo System** — Chain attacks for bonus damage
6. **🗺 Level Progression** — 5 different enemies across levels, scaling HP and damage
7. **📜 Battle Chronicle** — Full combat log showing every round's outcome
8. **🩸 Status Effects** — Shield, Regen, Poison, Rage buffs/debuffs
9. **👁 AI Prediction Panel** — Live probability bars showing Oracle's prediction

---

## 🚀 Hosting on GitHub Pages

1. Create a new repository (e.g. `battle-predictor`)
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages**
4. Set source to `main` branch, `/ (root)` folder
5. Click **Save** — your game will be live at:
   ```
   https://YOUR_USERNAME.github.io/battle-predictor/
   ```

---

## 🎯 Game Controls

| Action | Effect |
|---|---|
| ⚔ **Attack** | Deal 15–25+ damage. Chain for combos! |
| 🛡 **Defend** | Block incoming attack, counter for 8–16 dmg |
| 💚 **Heal** | Restore 25–35 HP (3 uses per battle) |
| 🧪 **Elixir** | Heal 40–60 HP instantly |
| 💣 **Bomb** | Deal 30–50 damage to enemy |
| 🔮 **Rune** | Activate regeneration for 3 turns |
| 🪬 **Ward** | Reduce incoming damage for 3 turns |

---

## 📁 File Structure

```
battle-predictor/
└── index.html   ← entire game (single file)
└── README.md    ← this file
```

---

## 👨‍💻 Built For

MLP Game Assignment — Adaptive AI behavior using pattern recognition logic.  
No external libraries. No frameworks. Pure JavaScript.
