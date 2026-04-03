# 🏫 School Mischief!

> A browser game set inside an SMS Gurugram classroom. Bhawana Ma'am sleeps at her desk — when she does, it's chaos time. Do pranks, earn points, survive her wake cycles, and WIN. Play solo or with friends via multiplayer!

**[▶ Play Now](https://OjiTheChamp.github.io/school-mischief/)** ← replace with your username after deploying

---

## 🎮 Controls

| Input | Action |
|-------|--------|
| `WASD` / Arrow Keys | Move |
| `Space` | Instantly teleport to seat |
| `Escape` | Close any open panel |
| 🚪 Leave button | Return to main menu |

---

## 🕹️ Game Modes

| Mode | Lives | Sleep | Awake | Wins on Win |
|------|-------|-------|-------|-------------|
| 😎 Easy | 4 | 18s | 6s | +1 |
| 😤 Medium | 3 | 12s | 10s | +5 |
| 😰 Hard | 2 | 7s | 15s | +50 |
| 💀 Nightmare | 1 | 3.5s | 20s | +2000 |
| ♾️ Easy Endless | 4 | 18s | 6s | survive forever |
| ♾️ Medium Endless | 3 | 12s | 10s | survive forever |
| ♾️ Hard Endless | 2 | 7s | 15s | survive forever |
| ♾️ Nightmare Endless | 1 | 3.5s | 20s | survive forever |

---

## ✨ Features

### Gameplay
- 😈 **94 Pranks** — 5 tiers from harmless (10 pts) to legendary (80+ pts), searchable menu
- 💃 **4 Powerups** — Dance, Talk, Score Run, Hide
- 💤 **Bhawana Ma'am** — sleeps at desk, wakes on timer, sees the ENTIRE classroom
- 🏆 **Win condition** — survive enough wake cycles with lives remaining

### Shops & Upgrades
- 🛒 **Class Store** — Extra lives (150 pts), Shield 3× (450 pts), 2×–6× multipliers
- 🛍️ **Power Shop** — spend Wins on mid-game boosts: Extra Time, Speed Burst, Disguise, Distraction, Second Chance, Mega Prank, Star Magnet, Teacher Apple. Buy unlimited quantities!
- ⚡ **Use panel** — quick-use stocked powers during gameplay

### Persistence
- 🏆 **Wins** — saved in localStorage, persist across sessions
- 📊 **Leaderboard** — Most Points · Longest Survive · Most Wins · Endless Time (top 10 each)
- ⏱ **Survive Bonus** — passive points every 60s just for staying alive

### Presentation
- 🏫 **SMS Gurugram classroom** — sky-blue walls, spinning ceiling fans, marble floors, iron window grilles, notice board, teacher's desk with 6 subject notebooks
- 🎵 **Background music** — chiptune free-time melody + danger drone, toggleable
- 🔊 **Sound effects** — every action has a procedural sound (Web Audio API)
- 📱 **Mobile** — on-screen D-pad for touch devices
- 📖 **Tutorial** — 6-page in-game guide

### Multiplayer
- 🌐 **WebRTC peer-to-peer** via PeerJS — no server, completely free
- Share a room code, see each other as coloured stickmen in real time
- Duplicate names blocked (case-insensitive)
- Up to 8 players in one room

---

## 🚀 Deploy to GitHub Pages

### Quick (no terminal needed)
1. Create a new repo at [github.com/new](https://github.com/new) — name it `school-mischief`
2. Click **uploading an existing file** → drag all files from this zip
3. Go to **Settings → Pages → Source: GitHub Actions**
4. Done! Live at `https://yourusername.github.io/school-mischief/`

### With Git
```bash
git clone https://github.com/yourusername/school-mischief
cd school-mischief
# copy files here
git add .
git commit -m "initial"
git push
```
Then enable **Settings → Pages → Source: GitHub Actions**.

Every future `git push` to `main` auto-redeploys in ~60 seconds.

---

## 🌐 Multiplayer Guide

1. Both players open the same game URL
2. Click **🌐 Multi** on the main menu or in the powerup bar
3. **Host:** Enter your name → Host Game → share the 8-character room code
4. **Join:** Enter your name → Join Game → paste the code → Join
5. Start the same difficulty — all players appear as coloured stickmen

> Names must be unique — joining with the same name as another player will be rejected.

---

## 📁 Project Structure

```
school-mischief/
├── index.html              ← Entire game (~120KB, zero dependencies)
├── README.md               ← This file
├── LICENSE                 ← MIT License
├── .gitignore
└── .github/
    └── workflows/
        └── deploy.yml      ← Auto-deploy to GitHub Pages on push
```

**No build tools. No npm. No server. Just one HTML file.**

---

## 📝 License

MIT — use, share, and modify freely.
