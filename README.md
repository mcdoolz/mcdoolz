# mcdoolz

Welcome to my profile. I build high-performance software, game engines, and autonomous systems.

---

## 🎲 Featured: DMGE (Dungeon Master Game Engine)

**DMGE** is a next-generation, offline-first Virtual Tabletop (VTT) and procedural world simulation engine engineered for tabletop roleplaying games. Built from the ground up for instantaneous response times, zero network dependency during sessions, and native AI-assisted map and encounter synthesis without relying on cloud LLMs.

### ⚡ Architectural Highlights

- **PixiJS 8 WebGL/WebGPU Rendering Engine**: Butter-smooth 60+ FPS map canvas supporting multi-layer rendering, dynamic weather, custom shaders, and responsive token transforms.
- **JEV System 1 Decision Architecture**: Joint Evaluation Vector decision model performing multi-head classification and continuous scoring in sub-millisecond timeframes. Zero token generation, zero hallucination, zero API costs.
- **Wave Function Collapse (WFC) Adjacency Solver**: Procedural dungeon, cave, and wilderness synthesis driven by socket adjacency rules, automatically generating raycasting vision-blocking walls (`BlockingSegment`) for instant Fog of War.
- **In-Browser Dictation to Map**: Game Masters can speak naturally using standard browser/OS Web Speech API. JEV extracts dungeon biomes, room configurations, threat levels, and lighting, triggering WFC to construct live playable battlemaps in real time.
- **8-Directional & Top-Down Scripted Sprites**: Full support for 8-direction animated sprites, transparent WebM video props, and autonomous NPC waypoint patrol scripting.
- **100% Offline-First Architecture**: Pulls public asset packs once from GitHub into client-side IndexedDB with shard management. Runs completely offline in the browser as a PWA.

---

## 📦 Open Asset Libraries

| Repository | Description | Format / Standards |
| :--- | :--- | :--- |
| [**dmge-tiles**](https://github.com/mcdoolz/dmge-tiles) | Modular, socket-tagged tile library for WFC map generation | 4-way sockets (`N/E/S/W`), LOS wall vectors, biome tags |
| [**dmge-props**](https://github.com/mcdoolz/dmge-props) | Interactive props, animated tokens, and scripted NPCs | WebM, PNG sheets, 8-way sprites, patrol waypoints |

---

## 🛠️ Tech Stack & Systems

- **Engines & Runtimes**: TypeScript, PixiJS 8, React, Node.js, WebGL, WebGPU, WebRTC P2P
- **Decision & Procedural AI**: JEV (Joint Evaluation Vector) System 1, Wave Function Collapse (WFC)
- **Local-First & Storage**: IndexedDB, Service Workers, PWA, fflate (.dmge format)
