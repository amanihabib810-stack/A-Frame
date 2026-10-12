# 🌲 The Escape

A small 3D browser game built with A-Frame. You're lost in a dark, foggy swamp forest: find all 5 glowing orbs, reach the portal, and escape before the skeletons catch you.

<img width="1606" height="1011" alt="Näyttökuva 2026-10-12 kello 12 43 30" src="https://github.com/user-attachments/assets/59d991cf-11c2-40f0-8ba0-f038b35c334c" />

▶️ Play it here: [The Escape](https://amanihabib810-stack.github.io/A-Frame/)

### 🎮 How to play
- Click Start Game.
- Explore the forest and find the 5 glowing orbs (follow the light beams).
- Stand next to an orb and press E to collect it.
- Watch out: skeletons appear every few seconds and chase you. Punch them or roll past them.
- When all orbs are collected, the purple portal appears. Walk into it to escape!

You have 3 hearts ❤️. Lose them all and the game is over.

### Controls

| Key | Action |
|---|---|
| **W / S** or **↑ / ↓** | Walk forward / backward |
| **← / →** | Turn left / right |
| **A / D** | Step sideways |
| **Shift** + walk | Run |
| **E** | Pick up an orb |
| **F** | Punch |
| **Space** | Roll (dodge, you can't be hit while rolling) |
| **Q** | Wave 👋 |


### ✨ Features
Third-person camera that follows the player
Animated character: idle, walk, run (4 directions), roll, punch, hit and death
Enemies that spawn in waves and chase the player
Health (hearts), timer and orb counter
Subtitles: the character comments on what's happening
Start screen, win screen and game-over screen with Play Again / Home
Night swamp environment with fog, glowing pools and fireflies
Works on desktop, and in VR headsets through WebXR

### 🛠️ Built with
HTML and JavaScript
A-Frame 1.8.0 (built on three.js)
aframe-environment-component: forest, sky and fog
aframe-extras: model animations

### Custom A-Frame components I wrote:

Component	What it does
player-anims	Switches the player's animations based on the keys pressed
arrow-turn	Turns the player with the arrow keys
enemy	Makes a skeleton chase the player, attack and die
game	Game rules: orbs, portal, hearts, timer, enemy spawning, win/lose
swamp-decor	Scatters glowing pools and fireflies around the world

### 🚀 Run it locally
The game needs a local server, because browsers block loading 3D models from file://.

##### Option 1: VS Code

Install the Live Server extension.
Open the project folder, right-click index.html and choose Open with Live Server.

##### Option 2: Terminal

bash
```python3 -m http.server 8000```

Then open ```http://localhost:8000.```

### 📁 Project structure
```
A-Frame/
├── index.html      # The whole game: scene, components and UI
├── soldier.glb     # Player model
├── skeleton.glb    # Enemy model
├── screenshot.png  # Image for this README
└── README.md
```

### 📚 What I learned
How A-Frame's entity-component system works, and how to write my own components
Loading and animating 3D models (glTF/GLB) with THREE.AnimationMixer
Game logic: distance checks, enemy movement, health, timers and game states
Parent/child entities, so the camera and the character move together
Building UI overlays (screens, HUD, subtitles) with HTML and CSS on top of a 3D scene
Debugging with the browser console

### 🔮 Ideas for the future
 Sound effects and background music
 More levels with different environments
 Best-time leaderboard
 Trees and obstacles you can hide behind
 Mobile touch controls
 
### 🙏 Credits
Soldier by Quaternius via Poly Pizza, licensed CC-BY 3.0
Skeleton by Quaternius via Poly Pizza, Public Domain (CC0)
Started from the Learn A-Frame (VR) course on Codecademy
