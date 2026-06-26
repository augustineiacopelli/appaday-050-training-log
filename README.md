# 050 · Training Log

**AppADay** — App #050  
**Category:** Data Viz (D)  
**Live URL:** https://augustineiacopelli.github.io/appaday-050-training-log/  
**Date:** 2026-06-26

---

## What It Does

Training Log is a personal run tracker that lives entirely in your browser. Log every workout with distance, duration, type, how you felt, fuel used, and notes — then watch your stats and chart update instantly. A weekly mileage chart visualizes training load over time with bars or a dot-connected line, color-coded by the most intense run type in each period. All data is stored in localStorage with no account required.

## Features

- **Run logging** — date, distance (miles), duration (mm:ss or hh:mm:ss), workout type, feel, and notes
- **Fuel tracking** — add one or more fuel entries per run with time-into-run and name; manage presets in Settings
- **Live stats** — total miles, total run count, this-week mileage, and overall average pace
- **Weekly mileage chart** — canvas bar or line chart with 1W/2W/4W (day buckets) and 12W/26W/All (week buckets) views
- **Color-coded by intensity** — bars and dots colored by dominant run type: Race (purple) > Interval (red) > Tempo (amber) > Long (blue) > Easy (green); legend auto-updates to show only types present in view
- **Hover/touch tooltip** — shows date and mileage for any bar or point
- **This-week dot grid** — Monday–Sunday view showing miles per day at a glance
- **Full run history table** — with auto-calculated pace, type pill, feel emoji, and per-row pencil (edit) and × (delete) buttons
- **Run detail modal** — tap any row to see all fields including fuel log, shoes, and notes
- **Edit runs** — pencil button in the table or Edit button in the detail modal pre-populates the log form; Save Changes updates in place
- **Settings gear** — manage shoe collection with active-shoe selection (auto-applied to new runs, shown as indicator on log form) and fuel presets
- **Persistent storage** — everything saved to localStorage, survives page refresh

## Tech

Single-file vanilla HTML/CSS/JS. No frameworks, no dependencies, no build step. Canvas chart with `arcTo`-based rounded corners for Safari/iOS compatibility. Emoji stored as named slugs and resolved at render time to avoid localStorage serialization artifacts.

## Part of a Three-Day Arc

- **Day 049 — Pace Planner** — generate a week-by-week training plan for a goal race
- **Day 050 — Training Log** — log your actual runs with stats and chart ← *you are here*
- **Day 051 — Pace + Log** — combined app with plan and log side by side, with actual vs. goal mileage overlay

---

*Part of the [AppADay](https://augustineiacopelli.github.io/appaday/) project — one complete web app shipped every day.*
