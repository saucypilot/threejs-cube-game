This is a simple **3D browser-based game** using [Three.js](https://threejs.org/), where the player controls a green cube that can move and jump while avoiding incoming red enemy cubes falling from the distance. The game showcases basic physics such as gravity, velocity, and collision detection in 3D space.

## Features

- 3D scene rendered with `WebGLRenderer`
- Gravity and vertical bouncing logic
- Enemy cube spawner with increasing difficulty
- Keyboard-based player movement in XZ plane and jumping
- Real-time collision detection and game over condition
- Directional lighting and ambient lighting
- Smooth user interaction with `OrbitControls`

## How It Works

- The main player (`cube`) is an instance of a custom `box` class that inherits from `THREE.Mesh`. It has position, size, velocity, gravity, and optional Z-axis acceleration.
- Enemies spawn at increasing frequency and move toward the player.
- Collisions between the player and enemies are detected using AABB logic (axis-aligned bounding box).
- If a collision occurs, the game ends with an alert.

## Controls

| Key | Action           |
|-----|------------------|
| W   | Move forward     |
| A   | Move left        |
| S   | Move backward    |
| D   | Move right       |
| Space | Jump           |

## Technologies Used

- **Three.js** (module imports via CDN)
- **HTML + JS (ESModules)**
- **OrbitControls** for camera movement
