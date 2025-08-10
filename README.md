# React Webcam Filter Studio

## Overview
**React Webcam Filter Studio** is a **React + TypeScript + Vite** application that demonstrates real-time webcam video capture, processing, and filter effects using the **WebRTC `getUserMedia` API** and HTML5 `<canvas>`. It falls back to a local sample video if no webcam is available.

## Why this project exists
The purpose of this project is to:
- Demonstrate **React + TypeScript** skills applied to real-time multimedia scenarios.
- Show proficiency with **WebRTC APIs** and HTML5 video/canvas manipulation.
- Illustrate clean state management for UI-driven filters and effects.
- Provide a visually engaging portfolio example.

## Features
- **Live Webcam Capture** — Streams directly from the user’s camera.
- **Fallback Mode** — Plays a bundled sample video if webcam access is denied or unavailable.
- **Real-time Filters** — Adjust parameters on the fly:
  - Grayscale intensity
  - Sepia tone
  - Blur amount
- **Canvas Rendering** — Processes and displays video frames with active effects.
- **Responsive UI** — Works across desktop and laptop browsers.

> Key modules:
> - `src/App.tsx` — Main app logic for media capture, state management, and filter application.
> - `public/fallback1.mp4` — Fallback video used when webcam is unavailable.

## Quick start (clone & run)
```bash
# 1) Clone the repository
git clone <https://github.com/DennisNHanrieder/onm5.git>
cd onm5-main/onm5-main

# 2) Install dependencies
npm install

# 3) Start the development server
npm run dev
```

## Dependencies & setup
- **Core tech stack:** Node.js (v18+), React, TypeScript, Vite.
- **Package manager:** npm (pnpm/yarn also supported).
- **Recommended:** Use `nvm` or `asdf` to ensure Node version compatibility.

### Direct dependencies
- `react` — Component-based UI library.
- `react-dom` — DOM rendering for React components.

### Dev dependencies
- `typescript` — Static typing.
- `@vitejs/plugin-react` — Vite plugin for React.
- `eslint` + React plugins — Code style enforcement.
- `vite` — Development server and build tool.

## Common scripts
- **Install:** `npm install`
- **Development (HMR):** `npm run dev`
- **Build (production):** `npm run build`
- **Preview build:** `npm run preview`
- **Lint code:** `npm run lint`

## How to run tests
No tests are configured. Suggested setup:
```bash
npm install -D vitest @testing-library/react @testing-library/jest-dom jsdom
# Add to package.json:
# "test": "vitest"
npm test
```

## How to contribute
1. Fork the repository and create a feature branch.
2. Ensure new code follows the existing style and patterns.
3. Document any new functionality and UI changes.
4. Submit a pull request with a clear description.

## What powers the core functionality?
- **WebRTC `getUserMedia` API** — For webcam access and media streaming.
- **React + TypeScript** — Type-safe, component-based structure.
- **HTML5 `<canvas>`** — For real-time video frame manipulation.
- **Vite** — Fast, modern development tooling.
