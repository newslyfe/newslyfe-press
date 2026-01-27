# NewsLyfe

<p align="center">
  <img src="docs/logo/logo.png" alt="NewsLyfe Logo" width="120" />
</p>

International news aggregator and analyst. Over 100,000 articles within a 24-hour window, from nearly 7,000 sources across ~200 countries.

**Core principle:** Chronological display, no algorithms. Full control over your news feed.

**Tech:** React, IndexedDB, tab-based workspace. Android app (stable) + Desktop (beta).

//----------------------  eddig kész!!!////////////////

---

## Problem

- 7000+ sources, 200 countries, 90+ languages — fragmented and unmanageable
- Existing aggregators use algorithms that hide, rank, or filter content
- No single interface for global news without manipulation

## Solution

- Chronological-only feed with client-side filtering
- 100k+ articles in rolling 24h window, zero algorithmic manipulation
- Real-time translation + keyword alerts in 90+ languages
- One interface, all sources

//----------------------  Problem + Solution KÉSZ!!!////////////////

---

## Technical Implementation

**Client-side architecture for algorithmic neutrality:**
- IndexedDB stores 100k+ articles locally — no server-side ranking or tracking
- Tab-based workspace with persistent state across sessions
- Privacy by design: zero profiling, all filtering client-side

**90+ language support:**
- Real-time translation engine
- Keyword alerts in any language

**Performance at scale:**
- Virtualized lists + lazy loading handle massive feeds
- Incremental indexing without UI blocking
- Smooth scrolling through thousands of articles

**Why not server-side?** Zero manipulation means zero server-side ranking. Client-side filtering = user control.

//----------------------  Technical Implementation KÉSZ!!!////////////////

---

## Platforms

### 📱 Mobile (Android) - Stable Release

<p align="center">
  <a href="https://play.google.com/store/apps/details?id=com.newslyfe.mobile">
    <img src="docs/screenshots/1-n-k.png" alt="NewsLyfe Mobile App" width="100%" />
  </a>
</p>

<p align="center">
  <img src="docs/screenshots/2-k-globalnews.png" alt="Global News" width="24%" />
  <img src="docs/screenshots/3-ai-news-analyst.png" alt="AI News Analyst" width="24%" />
  <img src="docs/screenshots/4-smart-alerts.png" alt="Smart Alerts" width="24%" />
  <img src="docs/screenshots/5-alert-lang.png" alt="Alerts in your language" width="24%" />
</p>

**Key features:**
- 🌍 Global reach: 200 countries
- 🗣️ Instant translation with one tap
- 🔔 Smart alerts in 90+ languages
- 🤖 AI analysis (experimental)

[![Google Play](https://img.shields.io/badge/Google_Play-Download-green?logo=google-play)](https://play.google.com/store/apps/details?id=com.newslyfe.mobile)

---

### 🖥️ Desktop (Web/Electron) - Public Beta

<p align="center">
  <img src="docs/screenshots/web-full.png" alt="Desktop Interface" width="70%" />
</p>

**Key features:**
- Tab-based workspace with persistent state
- Advanced filtering by country, language, keyword
- Bulk operations and saved searches
- Native desktop performance via Electron

[![Public Beta](https://img.shields.io/badge/Status-Public_Beta-orange)](https://github.com/nicenews/newslyfe-demo)

//----------------------  Platforms KÉSZ!!!////////////////

---

## Technology Stack

- **Frontend:** React + Context API
- **Storage:** IndexedDB (client-side persistence)
- **State:** Custom `TabController` for tab management
- **Platforms:** Android (stable) + Desktop Web/Electron (beta) + iOS (planned)

---

## 🚀 Development Status & Roadmap

The project is currently in active development. Top priorities:

- [ ] **MVP Functionality:** Stabilize and test core features.
- [ ] **Tab-based Workflow:** Refine tab creation, deletion, and organization.
- [ ] **Filter Pipeline:** Optimize and expand filtering and search logic.
- [ ] **Bugfixes & UX Polish:** Ongoing improvements based on user feedback.

---

## 🤝 Contribution & Feedback

This repository is open for public testing and bug reporting. Contributions are primarily internal at this stage.

**Feedback and bug reports are welcome via GitHub Issues.** Every comment helps us improve the software.

---

## 📜 License & Contact

The project license can be found in the `LICENSE` file. (Currently: Proprietary)

For questions, open an [Issue here](https://github.com/newslyfe/newslyfe-demo/issues), or email us at [newslyfe.team@gmail.com](mailto:newslyfe.team@gmail.com).
