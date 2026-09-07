# 🏃 GRANDMA'S GREAT CHASE

<div align="center">
  <img src="https://img.shields.io/badge/Three.js-r152-black?style=for-the-badge&logo=three.js&logoColor=white" alt="Three.js"/>
  <img src="https://img.shields.io/badge/Web_Audio_API-FF6B6B?style=for-the-badge&logo=web-audio-api&logoColor=white" alt="Web Audio API"/>
  <img src="https://img.shields.io/badge/No_Install-Required-4CAF50?style=for-the-badge" alt="No Install"/>
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="MIT License"/>
</div>

<div align="center">
  <h3>🐾 An original 3D endless runner built with Three.js</h3>
  <p><em>Collect coins, grab power-ups, and outrun Grandma for as long as you can!</em></p>
</div>

<p align="center">
  <a href="#-play-now">Play Now</a> •
  <a href="#-features">Features</a> •
  <a href="#-how-to-play">How to Play</a> •
  <a href="#-tech-stack">Tech Stack</a> •
  <a href="#-screenshots">Screenshots</a> •
  <a href="#-development">Development</a>
</p>

---

## 🎮 Play Now

**[Play Grandma's Great Chase in your browser →](https://ypengly.github.io/grandmas-great-chase/)**

*No downloads, no installations, no sign-ups — just open and play!*

---

## ✨ Features

<div align="center">
  <table>
    <tr>
      <td align="center" width="33%">
        <h3>🏃 Endless Runner</h3>
        <p>Infinite procedurally generated course with increasing difficulty</p>
      </td>
      <td align="center" width="33%">
        <h3>🪙 Coin Collection</h3>
        <p>Collect coins that persist between runs and unlock new characters</p>
      </td>
      <td align="center" width="33%">
        <h3>⚡ Power-ups</h3>
        <p>Speed boosts, shields, and magnet effects to help your escape</p>
      </td>
    </tr>
    <tr>
      <td align="center">
        <h3>🎨 Unlockable Characters</h3>
        <p>Spend your hard-earned coins to unlock new runners</p>
      </td>
      <td align="center">
        <h3>🎵 Synthesized Audio</h3>
        <p>All sound effects and music generated live with Web Audio API</p>
      </td>
      <td align="center">
        <h3>📱 Mobile Friendly</h3>
        <p>Touch controls with swipe gestures for on-the-go gameplay</p>
      </td>
    </tr>
  </table>
</div>

### 🎯 Core Mechanics

- **Three lanes** to dodge obstacles and collect items
- **Jump** over barriers and **slide** under obstacles
- **Progressive difficulty** as your distance increases
- **Persistent progress** with localStorage saving
- **Responsive design** that works on any screen size

---

## 🎮 How to Play

### Getting Started

1. Open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge)
2. No server required — just double-click the file!
3. First load fetches Three.js and Google Fonts from CDN

### Controls

| Action | Desktop | Mobile |
|--------|---------|--------|
| Change Lane | ←/→ or A/D | Swipe Left/Right |
| Jump | ↑/Space/W | Swipe Up or Tap |
| Slide | ↓/S | Swipe Down |

### Game Objectives

1. **Run as far as possible** while avoiding obstacles
2. **Collect coins** to unlock new characters
3. **Grab power-ups** for temporary advantages
4. **Set new high scores** and beat your best distance

### Characters

Unlock new runners with coins collected across all your runs:
- Default Runner (unlocked)
- More characters to discover...

---


---

## 💻 Tech Stack

| Category | Technology |
|----------|------------|
| 3D Engine | Three.js r152 |
| Audio | Web Audio API (synthesized) |
| Fonts | Google Fonts (CDN) |
| Storage | localStorage |
| Languages | HTML5, CSS3, JavaScript |
| Architecture | Single-page application |

### Why No External Assets?

- **100% self-contained** — no image, sound, or model files to load
- **Instant loading** — everything generated procedurally
- **Legal compliance** — no copyrighted or licensed assets used
- **Lightweight** — minimal bandwidth usage

---

## 🚀 Development

### Project Structure

```
grandmas-great-chase/
├── index.html          # Main HTML file
├── css/
│   └── style.css      # All styles
├── js/
│   ├── game.js        # Core game logic
│   ├── scene.js       # Three.js scene setup
│   ├── audio.js       # Web Audio synthesis
│   └── ui.js          # Interface management
└── README.md
```

### Local Development

```bash
# Clone the repository
git clone https://github.com/yourusername/grandmas-great-chase.git
cd grandmas-great-chase

# Open in browser (no build step required!)
open index.html
```

### Making Changes

1. Edit `js/game.js` for gameplay mechanics
2. Modify `js/scene.js` for visual elements
3. Update `js/audio.js` for sound effects
4. Changes are live on refresh — no compilation needed!

### Customization

#### Adding New Characters

1. Add character data to the `characters` array in `js/game.js`
2. Define color scheme and model variations
3. Set unlock cost in coins

#### Modifying Power-ups

Power-up types are defined in `js/game.js`:
- Speed Boost: Increases movement speed
- Shield: Protects from one obstacle
- Magnet: Attracts nearby coins

#### Adjusting Difficulty

Balance parameters in `js/game.js`:
- `SPEED_INCREMENT`: How fast the game speeds up
- `OBSTACLE_SPAWN_RATE`: How often obstacles appear
- `MAX_SPEED`: Maximum game speed

---

## 🧪 Testing

### Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Full Support |
| Firefox | 88+ | ✅ Full Support |
| Safari | 14+ | ✅ Full Support |
| Edge | 90+ | ✅ Full Support |
| Mobile Chrome | Latest | ✅ Full Support |
| Mobile Safari | Latest | ✅ Full Support |

### Manual Testing Checklist

- [ ] Game loads without console errors
- [ ] All controls work (keyboard and touch)
- [ ] Obstacles spawn and function correctly
- [ ] Coins are collectible and count increases
- [ ] Power-ups work as intended
- [ ] Character selection saves and loads
- [ ] High score persists between sessions
- [ ] Audio plays on all browsers
- [ ] Responsive on different screen sizes
- [ ] Performance is smooth at 60fps

---

## 📊 Performance Optimization

- **Instanced rendering** for repeated objects
- **Object pooling** for obstacles and coins
- **LOD (Level of Detail)** for distant objects
- **Efficient geometry** with minimal polygons
- **RequestAnimationFrame** for smooth 60fps gameplay

---

## 🤝 Contributing

We welcome contributions! Here's how:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

### Development Guidelines

- Keep it self-contained (no external assets)
- Maintain performance (60fps on average hardware)
- Support touch and keyboard equally
- Write clean, documented code

---

## 📄 License

MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Credits

- **Three.js** — 3D rendering engine
- **Google Fonts** — Web typography
- **Web Audio API** — Synthesized audio
- **You** — For playing and supporting the game!

---

<div align="center">
  <sub>Made with ❤️ by a solo developer</sub>
  <br/>
  <sub>Grandma's Great Chase is an original creation — all code and content are completely original</sub>
</div>
