# 🎮 Pacman Game

<div align="center">

![Pacman](https://img.shields.io/badge/Pacman-v1.0-green)
![License](https://img.shields.io/badge/License-MIT-blue)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

A classic Pacman game built with vanilla JavaScript and HTML5 Canvas.

[**Play Online**](https://pacman-game-gray-three.vercel.app)

</div>

## 🎯 Features

- **Classic Gameplay**: Navigate Pacman through the maze, eat all dots
- **4 Unique Ghosts**: Each with different AI personalities
  - 🟥 **Blinky**: Aggressive chaser
  - 🟪 **Pinky**: Ambusher - tries to intercept
  - 🟦 **Inky**: Random movement patterns
  - 🟧 **Clyde**: Shy - runs away when close
- **Power Pellets**: Turn ghosts blue and eatable for extra points
- **Progressive Difficulty**: Ghosts get faster each level
- **High Score System**: Scores persist across sessions
- **Responsive Controls**: Arrow keys or WASD

## 🎮 Controls

| Key | Action |
|-----|--------|
| `↑` / `W` | Move Up |
| `↓` / `S` | Move Down |
| `←` / `A` | Move Left |
| `→` / `D` | Move Right |
| `Space` | Pause/Resume |

## 🏆 Scoring

| Action | Points |
|--------|--------|
| Eat Dot | 10 |
| Eat Power Pellet | 50 |
| Eat Vulnerable Ghost | 200 |

## 🚀 Getting Started

### Play Online
Visit the live demo: [pacman-game.vercel.app](https://pacman-game-gray-three.vercel.app)

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/theblackmonkai/pacman-game.git
cd pacman-game
```

2. Open `index.html` in your browser (or serve it):
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .
```

3. Visit `http://localhost:8000`

## 📁 Project Structure

```
pacman-game/
├── index.html          # Main game file (HTML + CSS + JS)
├── .github/
│   └── workflows/      # GitHub Actions workflows
│       ├── vercel-deploy.yml
│       └── auto-release.yml
├── .changelog.json     # Changelog configuration
└── README.md           # This file
```

## 🛠️ Technologies Used

- **HTML5 Canvas** - Game rendering
- **Vanilla JavaScript** - Game logic (no frameworks!)
- **CSS3** - Styling and animations
- **GitHub Actions** - CI/CD automation
- **Vercel** - Deployment platform

## 🔄 Automation

This repo is configured with:

1. **Auto-deployment**: Every push to `main` automatically deploys to Vercel
2. **Release automation**: Tag releases with `v*` to auto-generate changelogs
3. **Changelog generation**: Commits with labels auto-generate release notes

## 🏷️ Releasing

To create a new release:

```bash
# Increment version (semantic versioning)
git tag v1.0.1

# Push tag to trigger release workflow
git push origin v1.0.1
```

The workflow will:
1. Generate a changelog from commits
2. Create a GitHub release
3. Deploy to Vercel

## 🎨 Customization

The game is fully customizable in `index.html`:

- **Map layout**: Edit the `map` array
- **Ghost behavior**: Modify `moveGhosts()` function
- **Speed**: Adjust `PACMAN_SPEED` and `GHOST_SPEED`
- **Colors**: Change theme in `<style>` section

## 📝 License

MIT License - feel free to use this project for learning or as a base for your own games!

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📧 Contact

Created by [@theblackmonkai](https://github.com/theblackmonkai)

---

<div align="center">
Made with ❤️ using vanilla JavaScript
</div>
