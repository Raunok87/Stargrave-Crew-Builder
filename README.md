# 🛸 Stargrave — Ultimate Crew Builder & Knowledge Base

A modern, standalone, offline-first squad builder, campaign roster manager, and comprehensive knowledge base for the **Stargrave: Science-Fiction Wargames in the Ravaged Galaxy** tabletop miniatures game by Joseph A. McCullough (Osprey Games).

Zero dependencies. Zero build step. Fully responsive across phones, tablets, laptops, and ultra-wide gaming monitors (1080p, 1440p, 4K, 21:9, and 32:9).

---

## ⚡ Features at a Glance

### 1. 🛠 Crew Builder & Roster Manager
- **Captain & First Mate Pickers**: Choose from 14 backgrounds across all official rulebooks and expansions. Automatically enforces the rules: Captain chooses exactly 6 powers; First Mate chooses 4 powers with +2 TN difficulty. Supports the Paladin's Captain-only restriction and stat choices.
- **Timing Markers**: All powers display explicit **`⏳ BEFORE GAME`**, **`⚔️ DURING GAME`**, and **`🏆 AFTER GAME`** badges on main selection cards so you never miss a pre-game setup ability or post-game campaign roll.
- **Recruit Crew Roster**: Complete roster of all 32 standard and specialist soldiers. Add soldiers with automatic 8-crew cap enforcement, 4-specialist maximum checks, and custom nicknames.
- **Armoury, Gear & Ship Upgrades**: Creation-phase weapons, shields, combat gear, and ship upgrades with steppers and automatic calculations.
- **Sticky Budget Console**: Real-time credits tracking (`Budget / Spent / Left`) with visual progress meter and active warning indicators. Automatically awards the **Aristocrat** bonus (bumping budget to 450cr or 500cr plus a free gear upgrade selection).
- **Campaign & House Rules**: Built-in toggle for custom tournament / house rules, including *"No more than two of the same specialist soldier"* with visual limit badges and cap enforcement.
- **Export & Print**: Clean, formatted print stylesheet for tabletop crew sheets, one-click text roster clipboard export, and full JSON file backup/restore.

### 2. 📖 Backgrounds Codex
- Comprehensive lore, mechanical stats, and tactical overviews for all 14 backgrounds.
- **What Goes With What**: 4-tier synergy guides covering Partner Pairings, Crew Synergies, Signature Combos, and Recommended Loadouts.

### 3. ⚡ Powers & Spells Knowledge Base
- Searchable browser of all 70 psychic powers, combat tech, and alien powers.
- Filter by Category (*Line of Sight, Self, Touch, Area, Out of Game*), Strain, Target Number (TN), Core Background, and **Activation Timing** (*Before Game, During Game, After Game*).

### 4. 📦 Armoury & Loot Knowledge Base
- Searchable database of 65+ weapons, gear, tech items, and campaign loot tables.
- Toggle between card grid view and dense tabular reference sheet.

---

## 🚀 Running Locally

No installation or node modules required!
1. Clone or download this repository.
2. Double-click **`index.html`** to open it in any web browser (Chrome, Edge, Firefox, Safari, Brave).
3. Everything runs 100% locally in your browser with automatic `localStorage` saving.

---

## 🌐 Deploying to GitHub Pages with a Custom Domain

This repository is pre-configured and ready to host publicly on **GitHub Pages** with custom DNS.

### Step 1: Create a Public GitHub Repository
1. Go to [github.com/new](https://github.com/new).
2. Set the repository name (e.g. `stargrave` or `stargrave-builder`).
3. Set visibility to **Public**.
4. Leave *"Initialize with README"* unchecked (we already have one).
5. Click **Create repository**.

### Step 2: Push Updates to GitHub
You can use **GitHub Desktop** or run Git from the terminal:

```bash
git add .
git commit -m "Update powers with activation rules, strain recoil, and interactive navigation"
git push
```

*(If using **GitHub Desktop**, simply commit the modified files and click **Push origin**).*

---

### Step 3: Enable GitHub Pages
1. On your GitHub repository page: [github.com/Raunok87/Stargrave-Crew-Builder](https://github.com/Raunok87/Stargrave-Crew-Builder)
2. Click **Settings** (top navigation bar) -> **Pages** (in left sidebar).
3. Under **Build and deployment**:
   - **Source**: Select **Deploy from a branch**.
   - **Branch**: Select `main` and folder `/ (root)`.
4. Click **Save**.
5. Within 1–2 minutes, GitHub Pages will deploy your site at `https://raunok87.github.io/Stargrave-Crew-Builder/`.

---

### Step 4: Configure Your Custom Domain & DNS

#### A. If using a Subdomain (e.g., `stargrave.yourdomain.com`):
1. Log in to your DNS provider (Cloudflare, Namecheap, GoDaddy, Google Cloud DNS, etc.).
2. Add a **CNAME record**:
   - **Type**: `CNAME`
   - **Name / Host**: `stargrave` (or your chosen subdomain prefix)
   - **Target / Value**: `raunok87.github.io`
   - **TTL**: Auto or 3600

#### B. If using an Apex Domain (e.g., `yourdomain.com`):
1. Add four **A records** pointing to GitHub Pages IP addresses:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
2. (Optional) Add a CNAME for `www`:
   - **Type**: `CNAME` | **Name**: `www` | **Target**: `raunok87.github.io`

#### C. Set Custom Domain in GitHub:
1. In your GitHub repository, go to **Settings** -> **Pages**.
2. Under **Custom domain**, enter your domain name (e.g., `stargrave.yourdomain.com`).
3. Click **Save**. GitHub will automatically commit a `CNAME` file to the root of your repository.
4. Check the box for **Enforce HTTPS** (may take a few minutes while Let's Encrypt provisions the free SSL certificate).

---

## 📱 Device & Display Support

The application uses CSS fluid layout scaling (`clamp()`, auto-fill CSS grids, and viewport units) rather than rigid desktop widths:
- **Ultra-Wide Monitors (21:9 & 32:9)**: Smoothly expands across the full width, rendering multiple side-by-side cards, recruit rosters, and tables without cramped text or wasted side margins.
- **Desktop & Laptops (1080p, 1440p, 4K)**: Optimized 2-to-4 column layout for tactical planning.
- **Tablets & Mobile**: Adaptive single-column collapse with horizontally scrollable equipment/soldier tables and touch-friendly controls.

---

## ⚖️ Legal & Attribution

*Stargrave: Science-Fiction Wargames in the Ravaged Galaxy* is designed by Joseph A. McCullough and published by Osprey Games. This application is an unofficial, fan-made creation tool intended to assist players in building crews and managing campaign games. Please support the game by purchasing official rulebooks, supplements, and miniatures.
