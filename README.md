# Famanova — AI-Powered Daily News Brief | Morning Intelligence for the World

> **All you need to know today — in one scroll.**  
> Live global headlines · Real-time stock & crypto markets · Local weather · Daily insights · Free forever

[![Live Site](https://img.shields.io/badge/Live%20Site-famanova.com-gold?style=flat-square)](https://famanova.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Powered by AI](https://img.shields.io/badge/Powered%20by-AI-blue?style=flat-square)](#)
[![No Server Required](https://img.shields.io/badge/No%20Server-Static%20HTML-orange?style=flat-square)](#)

---

## 🌍 What is Famanova?

**Famanova** is a free, AI-curated **daily news brief website** that delivers the world's most important stories, live financial market data, real-time local weather, and a daily wisdom insight — all in a single, beautiful, fast-loading web page.

No app to download. No account required. No clutter. Just open [famanova.com](https://famanova.com) every morning and know everything you need to start your day in under 60 seconds.

Whether you're in **London, New York, Lagos Dubai, Nairobi, Toronto, Sydney, Singapore, or Johannesburg** — Famanova serves your local weather automatically and delivers globally relevant news, every single day.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 📰 **AI News Summaries** | Top 5 global stories summarised by AI — updated on every page load |
| 📈 **Live Market Data** | Real-time prices for S&P 500, NASDAQ, Bitcoin, Ethereum, Gold & Oil |
| 🌤 **Local Weather** | Auto-detects your city via GPS — current conditions + 4-day forecast |
| 💡 **Daily Insight** | A rotating wisdom quote + AI fact of the day |
| 📬 **Morning Brief Newsletter** | Subscribe free — one email, every morning, ~60 seconds to read |
| ⚡ **Zero Loading Time** | Pure static HTML/CSS/JS — no frameworks, no bloat, loads in < 1s |
| 📱 **Mobile-First Design** | Fully responsive — looks perfect on any screen, any device |
| 🌐 **Works Globally** | Weather and news adapt to your location anywhere in the world |

---

## 🔎 SEO Keywords This Project Targets

> *This section exists to help search engines correctly index and categorise Famanova.*

**Primary Search Intent:**
- daily news brief website
- AI news summary today
- morning news in one page
- best daily briefing website
- one page news website
- free morning briefing
- what happened today in the world
- top news stories today AI summary
- morning intelligence brief
- news summary website free

**Financial / Market Keywords:**
- live stock market update today
- Bitcoin price today live
- gold price today USD
- S&P 500 today live
- crypto market update today
- daily market snapshot free
- financial news brief today
- Nasdaq live price today
- morning market brief

**Weather Keywords:**
- local weather today free
- weather for my city right now
- real-time weather update
- weather without an app
- browser weather widget

**Audience-Specific Keywords:**
- morning news for professionals
- daily briefing for entrepreneurs
- busy professional news summary
- news digest for executives
- AI curated news for students
- global news in 60 seconds
- news for people with no time

**International / Regional Keywords:**
- daily news brief Nigeria
- morning news Africa today
- AI news summary UK
- daily briefing United States
- morning brief Canada
- daily news Australia
- top stories India today
- world news Arabic English French
- global morning briefing Europe
- daily news brief South Africa
- news summary Middle East
- Asian markets morning brief

**Competitor Alternatives (What People Search Before Finding Famanova):**
- alternative to Morning Brew
- alternative to The Skimm
- alternative to Axios AM
- alternative to TLDR newsletter
- alternative to Finimize
- one page news site like The Week
- free news aggregator 2025
- AI news digest site

---

## 🚀 Live APIs & Data Sources

Famanova is powered by a live multi-source data waterfall — no manual updates ever needed:

```
NEWS WATERFALL:
  1st → thenewsapi.com     (primary — live global headlines)
  2nd → worldnewsapi.com   (fallback — top stories by country)
  3rd → webz.io            (fallback — deep news index)
  4th → Curated static     (silent last resort — never shows errors)

MARKET WATERFALL:
  1st → Yahoo Finance      (no API key — live quotes)
  2nd → Finnhub.io         (API key — real-time financial data)
  3rd → Twelve Data        (API key — global market coverage)
  4th → Static values      (silent last resort)

WEATHER:
  → OpenWeatherMap API     (GPS geolocation → live conditions + forecast)
  → Nominatim (OSM)        (reverse geocoding — city name from coordinates)
```

Markets auto-refresh every **60 seconds**. News and weather refresh on every **page load**. Zero cron jobs. Zero servers. Zero maintenance.

---

## 🗂 Project Structure

```
famanova/
│
├── index.html          ← The entire website (single file, deploy anywhere)
├── README.md           ← This file
└── LICENSE             ← MIT License


### Option 1 — GitHub Pages (Free)

```bash
# 1. Fork or clone this repo
git clone https://github.com/YOUR_USERNAME/famanova.git

# 2. Push index.html to your repo
cd famanova
git add .
git commit -m "Deploy Famanova"
git push origin main

# 3. Go to Settings → Pages → Deploy from main branch
# Your site is live at: https://YOUR_USERNAME.github.io/famanova
```

### Option 2 — Vercel (Free, Fastest)

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
cd famanova
vercel

# Done — live in ~30 seconds with a global CDN
```

### Custom Domain Setup

# On GitHub Pages:
1. Settings → Pages → Custom Domain → enter famanova.com
2. Add CNAME file containing: famanova.com
3. Update DNS at your registrar
```

---

## 🔑 API Key Configuration

Open `index.html` and locate the `CONFIG` block near the bottom:

```javascript
const CONFIG = {
  OWM_KEY:        'YOUR_OPENWEATHERMAP_KEY',   // openweathermap.org — free
  THENEWS_KEY:    'YOUR_THENEWSAPI_KEY',        // thenewsapi.com — free tier
  WORLDNEWS_KEY:  'YOUR_WORLDNEWSAPI_KEY',      // worldnewsapi.com — free tier
  WEBZ_TOKEN:     'YOUR_WEBZ_TOKEN',            // webz.io — 1,000 calls/month free
  FINNHUB_KEY:    'YOUR_FINNHUB_KEY',           // finnhub.io — free tier
  TWELVEDATA_KEY: 'YOUR_TWELVEDATA_KEY',        // twelvedata.com — free tier
};
```

All APIs listed above have **free tiers** sufficient for thousands of daily visitors.

---

## 🌐 SEO Architecture

Famanova is built with organic search visibility baked into every element:

### On-Page SEO
- ✅ Semantic HTML5 structure (`<header>`, `<article>`, `<section>`, `<footer>`)
- ✅ Optimised `<title>` and `<meta description>` tags
- ✅ Open Graph tags for rich social media previews
- ✅ Canonical URL tag
- ✅ Keyword-rich heading hierarchy (H1 → H2 → H3)
- ✅ Alt text on all visual elements
- ✅ Schema markup ready (NewsArticle JSON-LD — add per story)

### Technical SEO
- ✅ Sub-1-second load time (single static HTML file, no server)
- ✅ Mobile-first responsive design (Google mobile-first indexing)
- ✅ No render-blocking resources
- ✅ Minification-ready
- ✅ HTTPS on all deployment platforms
- ✅ Core Web Vitals optimised (LCP, FID, CLS)

### Content SEO Strategy
- Fresh news content on every page load = Googlebot sees new content daily
- Long-tail keyword targeting across finance, tech, health, world news verticals
- Internal linking structure via newsletter CTA and affiliate placements
- User engagement signals: low bounce rate (bookmark-worthy daily utility)

---


## 🌍 International SEO Targeting

Famanova is designed to rank globally. Target languages and regions:

| Region | Language | Search Engine | Strategy |
|---|---|---|---|
| West Africa | English | Google | "daily news Nigeria / Ghana / Kenya" |
| UK & Ireland | English | Google / Bing | "morning briefing UK", "daily news summary Britain" |
| North America | English | Google / Bing | "morning news digest USA Canada" |
| South Asia | English | Google | "daily brief India Pakistan Bangladesh" |
| East Africa | English / Swahili | Google | "habari za leo" (news today) |
| Middle East | Arabic / English | Google | "ملخص الأخبار اليومي" (daily news summary) |
| Europe | English / French / German | Google / Bing | "résumé des nouvelles du jour" |
| Australia / NZ | English | Google | "morning news summary Australia" |
| Southeast Asia | English | Google | "daily news brief Singapore Malaysia" |

---

## 🔗 Backlink & PR Strategy

High-authority sites to pitch Famanova to:

- **ProductHunt** — "Today's Top Launches" visibility
- **IndieHackers** — "Show IH: I built a one-page news site"
- **HackerNews** — "Show HN: Free AI daily brief — no app, no account"
- **Lifehacker** — "Best morning routine websites"
- **The Next Web** — AI tools coverage
- **TechCrunch** — Startup tools roundup
- **Medium / Substack** — Guest articles on AI tools and productivity
- **AppSumo** — Lifetime deal listing (once premium tier is live)

---

## 🤝 Contributing

Contributions, ideas, and issue reports are welcome.

1. Fork the repository
2. Create your branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add: your feature description'`
4. Push: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📜 License

MIT License — free to use, modify, and distribute.  
See [LICENSE](LICENSE) for full terms.

---

## 🙏 Acknowledgements

Built with:
- [OpenWeatherMap](https://openweathermap.org) — weather data
- [thenewsapi.com](https://thenewsapi.com) — global news
- [Finnhub.io](https://finnhub.io) — financial data
- [Twelve Data](https://twelvedata.com) — market quotes
- [Yahoo Finance](https://finance.yahoo.com) — market data
- [Google Fonts](https://fonts.google.com) — Playfair Display, DM Mono, Crimson Pro
- [NordVPN](https://nordvpn.com) — affiliate partner
- [NordPass](https://nordpass.com) — affiliate partner
- [Morning Brew](https://morningbrew.com) — referral partner

---

<div align="center">

**[famanova.com](https://famanova.com)** · Built with ❤️ · Powered by AI · Free forever

*The world's smartest morning brief — one scroll, every day.*

</div>
