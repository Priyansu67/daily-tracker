# Daily Tracker

Plan and track tasks by **month**, **week**, and **day**. Organize your roadmap, log progress, and import or export CSV—all in the browser with data stored locally.

## Features

- **Roadmap view** — Months and weeks with day-based task lists (MON–SUN)
- **Task management** — Add and edit tasks with title, duration, details, URL, phase, tags, and milestone flag
- **Progress** — Check off tasks; progress is shown per day, week, and month
- **Week settings** — Set hours per day type (WFH, Office, Weekend) and map weekdays to day types
- **CSV import** — Import a checklist CSV (Notion-export style) as a new roadmap or merge progress only
- **CSV export** — Export your roadmap and completion state to a CSV file for backup or reuse
- **Start fresh** — Replace the roadmap with an empty one (progress/checked state is kept)
- **Dark / light theme** — Toggle with persistence
- **Responsive** — Usable on desktop and mobile; only the main content area scrolls on large screens

Data is stored in the browser (IndexedDB). No server or account required.

## Tech stack

- **React 19** + **TypeScript**
- **Vite**
- **react-icons** (io5)

## Getting started

### Prerequisites

- Node.js (v18+)

### Install

```bash
npm install
```

### Run locally

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Build for production

```bash
npm run build
```

Output is in `dist/`. Serve that folder with any static host.

### Preview production build

```bash
npm run preview
```

### Lint

```bash
npm run lint
```

## Project structure

- `src/App.tsx` — Main app and UI
- `src/types.ts` — Roadmap types and seed/helpers
- `src/db.ts` — IndexedDB (roadmap, checked state, settings)
- `src/csv.ts` — CSV parse (import) and build (export)
- `src/time.ts` — Duration parsing and formatting
- `src/index.css` — Styles and responsive layout

## License

Private. See repository settings for terms.
