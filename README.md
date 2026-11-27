# ESC — Chennai Pulse & Grassroots Arena

**Stop Scrolling · Start Living.**  
A single-file, offline-first web application prototype for hyperlocal IRL social discovery, grassroots sports & competitions, inclusive safe-space connections, and local venue perks in Chennai — styled in a warm Madras sand & archival paper interface with zero build steps required.

---

## Table of Contents

- [Overview](#overview)
- [Core Tabs & Features](#core-tabs--features)
  - [1. Pulse (City Drops & Interactive Map)](#1-pulse-city-drops--interactive-map)
  - [2. Arena (Live Telecast, Competitions & Scout Radar)](#2-arena-live-telecast-competitions--scout-radar)
  - [3. Connect (Friends, Crews & Bidirectional Safe-Graph)](#3-connect-friends-crews--bidirectional-safe-graph)
  - [4. Hub (Chats, Perks Wallet & Chennai Passport)](#4-hub-chats-perks-wallet--chennai-passport)
- [Contextual Sidebar & Trust Model](#contextual-sidebar--trust-model)
- [Getting Started](#getting-started)
- [Optional Gemini 3.5 Flash-Lite Integration](#optional-gemini-35-flash-lite-integration)
- [Browser Storage & State](#browser-storage--state)
- [Tech Stack](#tech-stack)

---

## Overview

**ESC (`ESC V2 · Chennai Build`)** combines four real-world social loops inside a single self-contained `index.html`:

- **Discover & Host IRL Meetups (*Pulse*)** — Join local sports games, skate jams, chess nights, or safe-space circles across Chennai, or publish your own drop in seconds.
- **Compete & Spectate (*Arena*)** — Follow live local match tickers with spectator chat, enter grassroots tournaments as a squad or solo free agent, and browse regional standings & scout spotlights.
- **Meet Activity-First (*Connect*)** — Connect with Friends, Crews, or Spark matches using an inclusive, bidirectional Safe-Graph and 3-stop public-venue hangout plans.
- **Coordinate & Redeem (*Hub*)** — Manage IRL chats with pinned venue directions, claim local Chennai café/turf perks, and customize your Chennai Passport.

---

## Core Tabs & Features

### 1. Pulse (City Drops & Interactive Map)
- **Drops Feed & Search**: Natural-language filtering across drop titles, areas, categories, and tags (e.g., `"football"`, `"queer"`, `"skate"`, `"Adyar"`, `"free"`).
- **Category Pills**: `All`, `Sports`, `Hobbies`, `LGBTQ+ Safe`, `Women-Only`, and `Free`.
- **Interactive Chennai Map**: Toggle between card grid (**Drops**) and a live **Leaflet** map (CARTO Voyager tiles) with color-coded custom pins for Drops, Arena Tournaments, and Partner Perks, plus fly-to focus and one-click Google Maps directions.
- **Join Drop & Auto-Pass**: Joining a drop increments participant count, generates an `ESC-XXXX` pass in your Hub wallet, and opens/creates a dedicated group chat with the pinned venue plan.
- **Host a Drop Modal**: Create a new Chennai drop with title, category, public area, time, max spots, entry fee (`₹`), and inclusivity/skill tag.

### 2. Arena (Live Telecast, Competitions & Scout Radar)
- **Live Match Telecast Theater**: Switch between two live grassroots broadcasts (**5v5 Final** at *T. Nagar Arena Turf* and **Rapid Chess** at *Writer’s Café Courtyard*) featuring:
  - Real-time ticking match clock and live viewer count
  - Rotating play-by-play commentary ticker
  - One-click Cheer counter and live spectator chat
  - In-stream local sponsor deal strip
- **Open Chennai Competitions**: Register for tournaments (*Chennai Street 5v5 Turf Cup*, *Marina Skate Open*, *Madras Blitz Chess Championship*) either with a **Squad/Team** or as a **Solo Free Agent**, automatically issuing an `ARENA-XXXX` pass (with a 10% platform fee, waived to `₹0` for `ESC+` members).
- **Top Regional Teams**: Season 4 standings leaderboard across Football, Skate, and Chess.
- **Rising Talent (Scout Radar)**: Spotlight cards highlighting local grassroots MVPs with one-click **Endorse** support.

### 3. Connect (Friends, Crews & Bidirectional Safe-Graph)
- **Three Connection Modes**:
  - **Friends**: 1-on-1 activity buddies around Chennai neighborhoods.
  - **Crews**: Open local collectives (e.g., *Besant Boarders Crew*, *Madras Chess Collective*).
  - **Spark ✨**: Dating/connection mode powered by a **Bidirectional Safe-Graph**.
- **Bidirectional Safe-Graph**: In Spark mode, profiles appear only when your Passport gender/orientation preferences (`Man`, `Woman`, `Non-Binary` × `All`, `Straight`, `Gay`, `Lesbian`, `Queer`) mutually match the other person's preferences.
- **Community & Inclusive Identity Filter**: Filter cards by `All`, `LGBTQ+ Friendly`, `Queer`, `Women`, `Men`, `Non-Binary`, `Introvert`, and `Extrovert`.
- **Smart Plan**: Generates a 3-stop, public-venue Chennai itinerary tailored to the match's interests and area, with one-click **Send Plan & Chat**.

### 4. Hub (Chats, Perks Wallet & Chennai Passport)
- **Chats**:
  - Thread list for 1-on-1 connections, crews, and joined/hosted drops.
  - Pinned IRL plan banner with direct **Google Maps Directions**.
  - **Smart Icebreaker** button (`auto_awesome`) to pre-fill conversation openers.
  - Simulated replies using built-in fallbacks (or live contextual replies via Gemini 3.5 Flash-Lite when configured).
- **Perks & Passes**:
  - View all active drop, host, and tournament passes (`ESC-XXXX`, `HOST-XXXX`, `ARENA-XXXX`).
  - Claim limited local partner coupons (*The Brew Room*, *Decathlon OMR*, *Writer’s Café*, *Velocity Sports Turf*) with unique redemption codes and map directions.
- **Passport**:
  - Displays your **Show-Up Score (`98%`)**, IRL check-ins, active passes, and saved perks.
  - Edit your display name, Chennai neighborhood/campus, gender, Spark orientation preference, and community/vibe tags.
  - **ESC+ Membership (Demo)**: Simulated `₹149/mo` upgrade unlocking `0%` platform fees on tournament registrations.
  - **Reset Demo Data**: Restores the seeded Chennai dataset and clears local changes.

---

## Contextual Sidebar & Trust Model

On desktop viewports (`xl+`), a right-hand contextual sidebar provides:
- **Watching Now**: Live mini-scoreboard linking directly to the Arena telecast.
- **Instant Vibe Concierge**: One-click mood shortcuts (`⚽ Play tonight`, `🏳️‍🌈 Safe hangout`, `☕ Chill coffee`) that jump straight to matching drops or perks.
- **Your Next IRL Drop**: Quick preview of your latest active pass.

Clicking the shield icon (`verified_user`) opens the **Trust & Safety Model** modal outlining ESC's three pillars:
1. **Anti-Flake Show-Up Score** via public venue check-ins.
2. **Public Venues Only + Group-First Option** (never private addresses).
3. **Bidirectional Inclusive Safe-Graph** with dedicated LGBTQ+ & Women-Only safe spaces.

---

## Getting Started

No installation, package manager, or build step is required.

1. **Clone or download** the repository:
   ```bash
   git clone https://github.com/ibu112/Esc.git
   cd Esc
   ```
2. **Open `index.html`** directly in any modern browser, or serve it locally:
   ```bash
   npx serve .
   # or
   python -m http.server 8000
   ```

> **Note:** An internet connection is used for CDN assets (Tailwind CSS, Google Fonts, Material Symbols, Leaflet, and CARTO map tiles).

---

## Optional Gemini 3.5 Flash-Lite Integration

ESC runs completely offline/natively out of the box using its built-in **Instant Engine**. If you want live generative responses:

1. Navigate to **Hub → Passport**.
2. Scroll to **Optional Live AI Concierge (Gemini 3.5 Flash-Lite)**.
3. Paste a Google AI Studio key (`AIza...`), click **Test Key** to verify connectivity, and click **Save Key**.

When active (`GEMINI 3.5 LIVE`), the key powers personalized Smart Plan intros and dynamic chat responses using `gemini-3.5-flash-lite`. Your key is stored only in your browser's `localStorage` and can be cleared anytime.

---

## Browser Storage & State

All state is persisted client-side in `localStorage`:

| Key | Purpose |
| :--- | :--- |
| `esc_chennai_heritage_v2` | Stores user Passport settings, joined/hosted drops, tournament registrations, claimed perks, passes, and chat threads |
| `esc_gemini_key` | Optional Google AI Studio API key for `gemini-3.5-flash-lite` |

---

## Tech Stack

- **Core**: Vanilla HTML5, CSS3, and ES6+ JavaScript (single-file architecture in `index.html`)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) (CDN) + custom Madras sand/archival paper textures & inline SVG illustrations
- **Typography & Icons**: Google Fonts (`Fraunces`, `Plus Jakarta Sans`, `JetBrains Mono`) & Material Symbols Outlined
- **Maps**: [Leaflet](https://leafletjs.com/) (`v1.9.4`) with CARTO Voyager basemap tiles
- **Optional AI**: Google Generative Language API (`gemini-3.5-flash-lite`)
