# 🦋 Butterfly Conservation Society

India's premier butterfly documentation, citizen science, and conservation platform.

## Quick Start

```bash
npm install
npm start
```

Opens at http://localhost:3000

## Build for Production

```bash
npm run build
```

## Project Structure

```
src/
├── data/           Static data (categories, team, sightings, stats)
├── services/       API layer (swap dummy data for real fetch here)
├── context/        Global state — Context API + useReducer
├── components/
│   ├── layout/     Navbar, Footer
│   ├── shared/     Loader, StatusBadge, Avatar, GlobalSearch
│   ├── modals/     SpeciesModal, MemberModal
│   └── map/        IndiaMap (SVG)
├── pages/          HomePage, SpeciesPage, TeamPage, AboutPage
└── styles/         global.css (CSS variables + animations)
```

## Pages
- **Home** — Hero, stats dashboard, species family cards
- **Species** — Grid + map view, filter by family/subcategory
- **Team** — Department filter, member cards with full profile modal
- **About** — Story, values, timeline, contact, social links

## Design Tokens (CSS Variables)
```css
--bg: #04080a
--green: #52c97b
--ff: 'Cormorant Garamond' (display)
--fb: 'DM Sans' (body)
```

## Connecting Real Data
Replace `src/services/api.js` dummy functions with real `fetch()` calls.
All API methods are: `getCategories()`, `getTeam()`, `getStats()`, `getSightings(filters)`.
