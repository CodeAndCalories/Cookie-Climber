[README.md](https://github.com/user-attachments/files/25373776/README.md)
# 🍪 Cookie Climb

> *A tiny mouse's epic quest for the ultimate snack.*

**Cookie Climb** is a browser-based 2D arcade platformer where you play as a small mouse trying to scale the treacherous heights of a kitchen counter to reach the cookie jar. Climb ladders, shimmy up yarn, dodge cat paws, duck falling objects, and pray the human doesn't walk by and shake everything loose.

---

## 🎮 Play It

Open `index.html` in any modern browser — no install, no dependencies, no nonsense. Just cookies.

**Hosted on GitHub Pages:** [your-username.github.io/cookie-climb](https://your-username.github.io/cookie-climb)

---

## 🕹️ Controls

| Input | Action |
|-------|--------|
| `W` / `↑` | Move up / Climb ladder |
| `S` / `↓` | Move down / Descend ladder |
| `A` / `←` | Move left |
| `D` / `→` | Move right |
| `SPACE` | Jump |

> **Tip:** Walk into a ladder or yarn and press `W` to start climbing. Press `SPACE` mid-ladder to leap off dramatically.

---

## 🏠 The World

You're a tiny mouse in a full-sized kitchen. What looks like a simple jump is actually a multi-story climb. The levels take place across:

- **The Floor** — your starting point and the place you'll return to when things go badly
- **Wooden Shelves** — rickety ledges full of hazards
- **The Kitchen Counter** — the final frontier, where the cookie jar sits waiting

Each level adds more platforms, tighter gaps, and nastier obstacles between you and your goal.

---

## ⚠️ Obstacles

### 🐾 Cat Paws
A lazy cat swipes its paw across the shelves at regular intervals. Time your climbs between swipes or get knocked back to the start.

### 🥫 Falling Objects
Cans, rolling pins, and other kitchen debris tumble from above and bounce off platforms. Watch the shadows and move fast.

### 👣 Giant Human
In later levels, a giant human stomps through the kitchen, shaking the entire counter. Objects fall, platforms vibrate, and you get knocked loose if you're not on the floor. The screen shakes. Your heart shakes. Everything shakes.

---

## 🌟 Features

- **5 escalating levels** — each with new platform layouts and harder obstacle patterns
- **Animated mouse character** — complete with walking legs, a tail, and a tiny backpack
- **Yarn climbing** — wobbly, physics-animated yarn balls anchored to the counter
- **Screen shake** — when the human walks by, you feel it
- **Invincibility frames** — you get a brief reprieve after being hit (the mouse blinks)
- **Directional goal arrow** — always points you toward the cookie jar
- **Score system** — earn points every second you survive, plus big bonuses for completing levels
- **3 lives** — use them wisely
- **Single HTML file** — the entire game is one self-contained file, no build tools required

---

## 📁 File Structure

```
cookie-climb/
│
├── index.html      # The entire game — HTML, CSS, and JavaScript in one file
└── README.md       # You are here
```

---

## 🚀 Deploying to GitHub Pages

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set the source to **Deploy from a branch → main → / (root)**
4. Save — your game will be live in about 60 seconds at `https://your-username.github.io/cookie-climb`

---

## 🛠️ Built With

- Vanilla HTML5 Canvas (no frameworks, no libraries)
- Pure JavaScript game loop with `requestAnimationFrame`
- CSS for UI and overlays
- Google Fonts: [Press Start 2P](https://fonts.google.com/specimen/Press+Start+2P) + [Fredoka One](https://fonts.google.com/specimen/Fredoka+One)

---

## 🧠 How It Works

The game uses a straightforward architecture:

- **`buildLevel(n)`** — generates platform, ladder, yarn, obstacle, and goal data for each level
- **`update()`** — handles physics (gravity, collision), player input, obstacle movement, and win/lose conditions
- **`draw()`** — renders the kitchen background, all game objects, the animated player, and HUD elements each frame
- Player movement uses AABB collision detection against platform rectangles
- Ladder/yarn climbing is detected by checking if the player's center X overlaps the climbable object's range

---

## 📜 License

MIT — do whatever you want with it. Bake cookies. Share them.

---

*Made with ❤️ and a deep craving for chocolate chip cookies.*
