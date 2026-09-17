# Neumorphic Live Calendar

Interactive weekly desktop calendar prototype built with React + TypeScript + Tauri.

## Run the UI
1. Install Node.js 20+.
2. `npm install`
3. `npm run dev`

## Run as a Windows desktop app
Install Rust and the Tauri prerequisites, then:
1. `npm install`
2. `npm run tauri dev`

## Current features
- Week navigation
- Seeded Sep 14–20, 2026 schedule
- Add tasks to any day
- Complete/delete tasks
- Persistent tasks via localStorage
- Overdue detection with shake animation on hover
- Ongoing/no-due-date section
- Neumorphic UI matching the supplied visual direction

## Live-wallpaper integration
This starter is the full interactive app layer. The Windows WorkerW/Progman attachment should be added as a native Windows-only module after validating the desktop UI. That native layer is OS-version-sensitive and should include a safe normal-window fallback so the app never interferes with Explorer or desktop icons.
