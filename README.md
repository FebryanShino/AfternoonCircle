# AfterNoon Web: Circle Fan Tracker and Trainer Toolkit

This folder contains the production build of **AfterNoon Web**, an unofficial companion web application for the **Uma Musume: Pretty Derby** circle **AfterNoon**.

- **Circle Name:** AfterNoon
- **Circle ID:** 746888162
- **Circle Leader:** 水分 (`883117653`)
- **Motto:** "OSHI RUNNER IS THE WINNER"

---

## Overview

AfterNoon Web tracks monthly circle fan gains, honors top monthly contributors on a championship podium, keeps past season records in a Hall of Fame, and provides practical tools for trainers: factor receipt stitching, Champions Meeting course breakdowns, and race simulations.

---

## Features for Trainers

### 1. Monthly Circle Standings
- **Top 3 Championship Podium:** Features the top three fan earners of the month with their representative trainee (supporting 3D idle animations or classic 2D portraits), costume title, and fan numbers.
- **Roster Standings (Ranks 4 to 30):** Full member roster searchable by trainer name or Uma Musume name. Sortable by monthly fan gain, today's fan gain, total career fans, or team evaluation score.
- **Circle Rank & Tier:** Displays our circle's live in-game rank and official tier badge (SS, S+, S, A+, etc.), with 24-hour daily fan delta tracking.
- **Monthly Target Pacing Graph:** Progress chart comparing our circle's actual cumulative fan gains against the month's target pace.
- **Export Standings:** Generates clean, high-resolution standings cards in dark or light mode, ready to share on Discord or Twitter/X.

### 2. Trainer Profiles
- Inspect individual members to see their representative trainee, 14-day fan trajectory graphs, and daily breakdowns.

### 3. Circle Hall of Fame
- Historical archive of completed monthly seasons.
- Displays past final circle ranks, total fans earned, and the Monthly MVP Trainer spotlight.

### 4. Receipt Factor Maker
- Drop or upload factor list screenshots from your training runs.
- Automatically detects scroll order and stitches the screenshots into a single vertical receipt image without scrollbars.
- Calculates cumulative star counts for duplicate factors across parent trainees.
- Exports inheritance data into Gametora-compatible JSON for sharing and build planning.
- Download the stitched receipt as a PNG or JPG image.

### 5. Champions Meeting Breakdown
- Complete course topology with race phases: Opening Leg, Middle Leg, Late Race, Final Straight, corners, slopes, and uphill/downhill sections.
- Character tier recommendations and skill priority guides for the active tournament track.
- Skill impact simulations showing acceleration curves, speed gain, and distance benefit.

### 6. Race Simulator
- Test trainee stats, running styles (Runner, Leader, Betweener, Chaser), and skill combinations against race course presets.

---

## How to View and Host This Build

Because this is a pre-built static application with client-side hash routing (`HashRouter`), it can be hosted on any static web host or viewed locally.

### Viewing Locally
Browsers block certain local file requests when opening `index.html` directly via the `file://` protocol. To view the build on your computer, run a lightweight static server:

```bash
# Using npx (requires Node.js)
npx serve .

# Or using Python 3
python -m http.server 8080
```
Then open `http://localhost:3000` (or `http://localhost:8080`) in your browser.

### Deploying to the Web
Upload all contents of this folder directly to any static hosting service:
- **Cloudflare Pages:** Connect repository or drag and drop this folder.
- **GitHub Pages:** Deploy this folder directly to your `gh-pages` branch.
- **Netlify / Vercel:** Deploy as a pre-built static site.

---

## Legal & Attribution

This is a non-commercial, fan-made tool created by and for circle AfterNoon.

All Uma Musume: Pretty Derby game content, character illustrations, names, and trademarks belong to **Cygames, Inc.** Character data and community references are sourced via public resources including GameTora for personal, non-commercial utility.
