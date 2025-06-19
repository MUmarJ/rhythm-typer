# 🎵 Rhythm Typer

A browser-based rhythm typing game that challenges players to match keyboard inputs with visual timing cues. Inspired by Patatap and built with Paper.js and Howler.js.

![Rhythm Typer Demo](https://img.shields.io/badge/Status-Playable-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 🎮 Game Overview

**Rhythm Typer** is an interactive audiovisual experience where players must type the correct keys at the precise moment when two colored circles collide on screen. Each key corresponds to a unique sound and visual effect, creating a symphony of music and animation based on your timing and accuracy.

### Key Features

- 🎯 **Precision Timing**: Hit keys exactly when circles collide for perfect scores
- 🎵 **Audio Feedback**: Each key triggers unique sounds from the Neuronal Synchrony collection
- 🌈 **Visual Effects**: Dynamic colored circles with blend modes and animations
- 📊 **Scoring System**: Track your accuracy with miss/hit feedback
- 🎭 **Multiple Tracks**: Choose from 3 different rhythm patterns with varying difficulty
- ⚡ **Speed Modifiers**: Dynamic timing changes keep you on your toes

## 🚀 Quick Start

### Prerequisites

- Modern web browser with HTML5 Canvas support
- Audio playback capability
- Keyboard for input

### How to Play

1. **Launch the game**: Open `RhythmTyper2.html` in your web browser
2. **Select a track**: Choose from 3 available tracks (BooM!, DesI, or Hyype)
3. **Watch the guide**: A preview of the rhythm pattern will be displayed
4. **Hit the keys**: Press the shown key exactly when the circles collide
5. **Follow the beat**: Use visual and audio cues to maintain rhythm

### Game Controls

- **Keyboard Keys**: `q` `w` `e` `r` `t` `y` `u` `i` `o` `p` `a` `s` `d` `f` `g` `h` `j` `k` `l` `z` `x` `c` `v` `b` `n` `m`
- **F5**: Quick reset
- **Fullscreen**: Recommended for optimal experience

### Visual Cues

- **`+`**: Be quick for the next note
- **`~`**: Rhythm change incoming
- **`++`**: Extra fast timing required

## 📁 Project Structure

```
rhythm-typer/
├── 🎮 Game Files
│   ├── RhythmTyper2.html      # Main game (recommended)
│   ├── RhythmTyperOg.html     # Original version
│   ├── index.html             # Alternative entry point
│   └── circleExercise.html    # Practice mode
│
├── 🎨 Playground/Sandbox
│   ├── pata.html              # Create custom beats
│   ├── pata2.html             # Enhanced beat creator
│   ├── circles.html           # Circle animation demo
│   └── circles.css            # Styling for circles demo
│
├── ⚙️ Core Files
│   ├── rhythm.js              # Game logic
│   ├── data.js                # Key mappings and sound assignments
│   ├── paper-full.js          # Paper.js library (graphics)
│   └── howler.js              # Howler.js library (audio)
│
├── 🔊 Audio Assets
│   └── sounds/                # Sound effects collection
│       ├── bubbles.mp3
│       ├── clay.mp3
│       ├── confetti.mp3
│       └── ... (25 unique sounds)
│
└── 📚 Documentation
    └── README.md              # This file
```

## 🎯 Game Modes

### Main Game (`RhythmTyper2.html`)

The complete rhythm typing experience with:

- 3 pre-programmed tracks with varying complexity
- Scoring system and feedback
- Visual guides and timing hints

### Practice Modes

- **`circleExercise.html`**: Focus on timing without pressure
- **`pata.html`**: Free-play mode to experiment with sounds
- **`pata2.html`**: Enhanced sandbox for creating custom patterns

### Development Versions

- **`RhythmTyperOg.html`**: Original prototype version
- **`circles.html`**: Visual animation testing

## 🛠️ Technical Details

### Technologies Used

- **Paper.js**: 2D canvas graphics and animation
- **Howler.js**: Cross-browser audio management
- **Vanilla JavaScript**: Game logic and interaction
- **HTML5 Canvas**: Rendering and visual effects

### Key Mappings

Each keyboard key is mapped to a unique sound and color:

| Key | Sound         | Key | Sound    | Key | Sound      |
| --- | ------------- | --- | -------- | --- | ---------- |
| `q` | Bubbles       | `a` | Pinwheel | `z` | Suspension |
| `w` | Clay          | `s` | Piston-1 | `x` | Timer      |
| `e` | Confetti      | `d` | Piston-2 | `c` | UFO        |
| `r` | Corona        | `f` | Prism-1  | `v` | Veil       |
| `t` | Dotted Spiral | `g` | Prism-2  | `b` | Wipe       |
| `y` | Flash-1       | `h` | Prism-3  | `n` | Zig-zag    |
| `u` | Flash-2       | `j` | Splits   | `m` | Moon       |
| `i` | Flash-3       | `k` | Squiggle |     |            |
| `o` | Glimmer       | `l` | Strike   |     |            |
| `p` | Moon          |     |          |     |            |

### Performance Optimization

- Optimized for 1920px width resolution
- Dynamic circle positioning based on viewport size
- Efficient collision detection using Paper.js intersections
- Audio preloading with Howler.js

## 🎨 Creating Custom Patterns

You can create your own rhythm patterns by modifying the `gameMap` array in the main game files:

```javascript
var gameMap = [
  "t+o+t^t^o%t^t$o$t^t^o%t^t$o", // Track 1: BooM!
  "v$s^v%s^v%s^v%s^v$s^v%s+h+f", // Track 2: DesI
  "p+p+p+p$p$p$p$p$p$p%p^p^o%p^p%o%p^p^o%p^p%o", // Track 3: Hyype
  "", // Add your custom track here
];
```

### Pattern Syntax

- **Letters**: Keyboard keys to press
- **`+`**: Slight speed increase
- **`$`**: Position offset (small)
- **`%`**: Position offset (medium)
- **`^`**: Position offset (large)

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:

- 🎵 Create new rhythm patterns
- 🎨 Add visual effects and animations
- 🔊 Integrate new sound libraries
- 🐛 Report bugs and issues
- 📖 Improve documentation

### Development Setup

1. Clone the repository
2. Open any HTML file in a modern web browser
3. Start experimenting with the code!

No build process required - everything runs directly in the browser.

## 🎓 Educational Use

This project demonstrates several important web development concepts:

- **Canvas API**: 2D graphics programming
- **Web Audio**: Sound management and playback
- **Game Development**: Timing, collision detection, scoring
- **Event Handling**: Keyboard input and user interaction
- **Animation**: Smooth 60fps animations with requestAnimationFrame

Perfect for learning about:

- HTML5 Canvas graphics
- Audio programming in web browsers
- Game timing and collision detection
- Interactive animation techniques

## 📜 Credits

- **Inspired by**: [Patatap](https://patatap.com/) by Jonobr1
- **Sound Effects**: Neuronal Synchrony collection (MIT License)
- **Graphics Library**: [Paper.js](http://paperjs.org/)
- **Audio Library**: [Howler.js](https://howlerjs.com/)
- **Course Inspiration**: Colt Steele's Udemy Web Development Course

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🎮 Ready to Play?

**Start with**: `RhythmTyper2.html` - Select a track and feel the rhythm!

**Practice with**: `pata.html` - Create your own beats and experiment

**Have fun and keep the rhythm! 🎵**

**Online Demo**
https://mumarj.github.io/rhythm-typer/
