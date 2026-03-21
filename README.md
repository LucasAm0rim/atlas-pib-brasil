# Atlas PIB Brasil: Executive GDP Dashboard

![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=06131A)
![Vite](https://img.shields.io/badge/Vite-8-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-Data%20Viz-FF6B6B?style=for-the-badge)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=06131A)

> A premium macroeconomic dashboard designed to translate quarterly GDP data into a clear executive narrative through visual hierarchy, sector analysis, and presentation-ready storytelling.

![Project Cover](./public/github-cover.svg)

---

## About The Project

`Atlas PIB Brasil` is a portfolio-grade frontend project built to present Brazilian GDP data from the supply-side perspective with the polish of an institutional product.

Instead of treating the dashboard as a generic analytics screen, the interface was designed to behave like a presentation layer for committees, strategy teams, and portfolio discussions. The goal is not only to display data, but to help the reader understand what changed, where the pressure is concentrated, and which sectors are still sustaining the aggregate result.

### Core Intent

- Turn macroeconomic data into a high-clarity visual product
- Reduce friction in reading sector contribution and momentum
- Deliver a screen that feels presentation-ready from the first load
- Combine Apple-like compositional discipline with institutional dashboard density

---

## Design Direction

This project was built with strong emphasis on visual restraint, readability, and proportion.

### UX Principles

- **Single-glance hierarchy**: the most important message appears first
- **Calm density**: information is rich, but never noisy
- **Stable proportion**: cards, chart area, and insight panels keep visual balance even with scrolling
- **Presentation readiness**: the layout feels suitable for portfolio, GitHub showcase, and stakeholder demos

### Interface Decisions

- Sticky analytical sidebar for persistent context
- Compact hero area with immediate economic interpretation
- KPI row focused on signal, not decoration
- Main visualization area centered on trend, contribution, and table views
- Right rail condensed into executive summary and cycle quality radar
- Light and dark theme support for premium presentation

---

## Dashboard Features

### 1. Executive Narrative Layer

The opening section highlights the economic message behind the data, not just the numbers themselves. It frames the end of 2025 as a period of slower growth quality, with services still cushioning the negative industrial print.

### 2. Sector Analysis

The dashboard compares:

- total GDP
- services
- industry
- agriculture
- net taxes

Users can isolate specific series through the sidebar filters to simplify the reading and focus only on the sectors relevant to the discussion.

### 3. Multiple Analytical Views

The same dataset can be read through:

- **Sector evolution** with line charts
- **Contribution by sector** with stacked bars
- **Quarterly table** for precise numeric reading

### 4. Executive Insight Blocks

The right column condenses the interpretation into:

- key narrative bullets
- cycle quality scorecards
- quarter-over-quarter deltas
- monitoring watchpoints

---

## Architecture & Frontend Structure

The application is organized as a modular React interface with clear separation between data, UI primitives, domain components, and formatting utilities.

### Folder Structure

```text
src/
├── components/
│   ├── ui/
│   │   ├── Button.jsx
│   │   └── Panel.jsx
│   ├── AnalyticsPanel.jsx
│   ├── HeroSection.jsx
│   ├── InsightsColumn.jsx
│   ├── MetricsOverview.jsx
│   └── Sidebar.jsx
├── data/
│   └── macroData.js
├── lib/
│   └── formatters.js
├── App.jsx
├── index.css
└── main.jsx
```

### Technical Decisions

- `App.jsx` orchestrates state, theme, filters, and view selection
- `macroData.js` centralizes dashboard content, labels, and metrics
- `formatters.js` isolates numeric display logic
- `AnalyticsPanel.jsx` is lazy-loaded to improve initial delivery
- UI primitives keep the visual system reusable and easier to evolve

---

## Technical Stack

- **Core**: React 19
- **Build Tool**: Vite 8
- **Charts**: Recharts
- **Icons**: Lucide React
- **Styling**: Tailwind CSS 4 + custom CSS system
- **Interaction**: `useDeferredValue`, `startTransition`, lazy loading and suspense fallback

---

## Performance & Delivery

This project is not only visually polished; it was also prepared with delivery quality in mind.

- Analytical panel separated into its own lazy-loaded chunk
- Build configured for GitHub Pages deployment
- Light and dark themes persisted locally
- README and repository assets prepared for portfolio presentation

---

## How To Run

### 1. Clone the repository

```bash
git clone https://github.com/SEU_USUARIO/atlas-pib-brasil.git
cd atlas-pib-brasil
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run the development server

```bash
npm run dev
```

### 4. Build for production

```bash
npm run build
```

### 5. Preview the production build

```bash
npm run preview
```

---

## Deploy

The project is already configured for GitHub Pages through GitHub Actions.

### Required Steps

1. Push the repository to GitHub
2. Open `Settings`
3. Go to `Pages`
4. Set `Build and deployment` to `GitHub Actions`

After that, every push to `main` will trigger a new deploy.

---

## What This Project Demonstrates

- Strong frontend composition and visual hierarchy
- Product thinking beyond generic dashboard templates
- Ability to turn raw data into a polished presentation layer
- Clean React structure for scalable interface work
- Attention to detail in both UI and repository presentation

---

## Repository Presentation Tips

For the GitHub repository itself, a strong short description would be:

> Executive dashboard for Brazilian GDP analysis with premium UI, sector comparison, and presentation-ready macro storytelling.

Suggested topics:

- `react`
- `vite`
- `dashboard`
- `macroeconomics`
- `recharts`
- `frontend`
- `data-visualization`
- `portfolio-project`

---

## Author

Built as a portfolio-ready frontend project focused on design quality, analytical storytelling, and premium presentation.
