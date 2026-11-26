# Runner Game

A 3D endless lane-runner built with **Three.js** in a single HTML file — no build step, no dependencies to install.

![Three.js](https://img.shields.io/badge/Three.js-000000?logo=threedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)

## Gameplay

- Dodge red obstacles by switching between three lanes
- The game speeds up the longer you survive
- Your score climbs with every obstacle you pass

## Controls

| Platform | Move left | Move right |
|----------|-----------|------------|
| Desktop  | `←` | `→` |
| Mobile   | Tap ◀ button | Tap ▶ button |

## How it's built

- **Rendering:** Three.js scene with a perspective chase camera, distance fog, and ambient + directional lighting
- **Movement:** The player eases toward the target lane each frame for smooth lane changes
- **Obstacles:** Spawned in a random lane far down the track and moved toward the camera; collisions are checked with bounding distances
- **Difficulty:** Speed ramps up with every obstacle wave, and off-screen obstacles are removed from the scene to keep it light
- **Mobile-first:** Touch controls with `preventDefault` to stop scroll/zoom while playing

## Run locally

Just open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```
