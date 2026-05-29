# jitesh.solutions

> **A Windows 98-style interactive portfolio OS** — built with React, powered by nostalgia.

A fully interactive desktop environment that doubles as a personal portfolio for **Rachamadugu Jitesh** — Software Engineer & AI Systems Architect. Navigate between sections inside draggable windows, play classic DOS games, listen to original music, and explore projects spanning AI, ML, and full-stack engineering.

---

## Preview



---

## The Experience

When you open the site, you're greeted by a **Windows 98 desktop** — teal background, pixel-perfect taskbar, Start button, and a set of desktop icons. Click any icon to open a window. Drag, minimize, and navigate just like the real thing.

### Desktop Icons

| Icon | Opens |
|------|-------|
| My Showcase | Main portfolio window (Home, About, Experience, Projects, Contact) |
| Doom | Classic id Software FPS via DOSBox |
| Digger | 1983 PC classic |
| Scrabble | Word game |
| Oregon Trail | The iconic 1971 edutainment game |
| Credits | About this portfolio |

---

## Portfolio Sections

### About
**Software Engineer & AI Systems Architect** with a focus on explainability-first ML design, low-latency processing pipelines, and production-ready inference systems.

### Experience

**HSBC** — Generative AI Engineer Intern *(Jan 2025 – Mar 2025 | Pune)*
- Banking News & Deal Intelligence Engine
- Cross-Asset Stress Scenario Simulator
- Real-Time FX Market Microstructure Monitor
- Deal and M&A activity tracking with NLP-powered sentiment analysis
- Real-time FX data ingestion and market microstructure analytics

**Artificial Intelligence Research Intern** *(May 2024 – Sep 2024 | India)*
- ResNet-50 based image classification
- Medical image preprocessing pipeline
- Model performance evaluation and NLP-focused feature engineering

**Freelancing & Client Projects**
- Client work and collaborations built outside of full-time roles

### Projects

| Project | Description |
|---------|-------------|
| Multi-Agent Hub | Dynamic agent orchestration with LangGraph, multi-provider LLM integration |
| RAG System | End-to-end Retrieval-Augmented Generation pipeline with vector database integration |
| AI Chatbot for Cruise Company | Context-aware LLM generation with semantic caching |
| AI-driven Code Review Automation | Security-focused static analysis with contextual vulnerability explanations |
| Document Extraction & Validation Pipeline | Structured output validation, document parsing and field normalization in Python |
| Legal & Compliance Workflow Intake System | Designed for batch-processing of mixed document formats |
| Malaria Blood Cell Classification | ResNet-50 based classification with medical image preprocessing |
| Banking News & Deal Intelligence Engine | Real-time news scraping, NLP relevance scoring, custom alert and monitoring system |
| Starlit Journals | Anonymous posting with codenames — zero personal data, mood tracking and collections |
| Jitesh Wordle | Wordle but with a JITESH-based twist |

### Music & Sound

Original music produced by Jitesh — playable directly in the portfolio:

| Track | Genre |
|-------|-------|
| Break [Demo] | Drum & Bass |
| Break [Drums and Sub] | Drum & Bass |
| Edge [W.I.P.] | Electronic |
| Exploring House | House |

### Certifications

- Oracle Certified Professional

---

## Tech Stack

### Portfolio App
| Layer | Technology |
|-------|-----------|
| Framework | React (Create React App) |
| Animation | Framer Motion |
| DOS Emulation | js-dos + wdosbox (WebAssembly / DOSBox) |
| Fonts | MS Sans Serif, Millennium, Millennium Bold, Terminal (custom TTF) |
| Styling | CSS Modules |

### Skills & Tools (from portfolio content)
`Python` `Azure / GCP / AWS` `LangGraph` `RAG Pipelines` `Vector Databases` `Celery / Redis` `Prompt Guardrails` `Monte Carlo Simulation` `ResNet-50` `NLP` `Cloud-Native`

---

## Project Structure

```
jitesh.solutions/
├── index.html              # Entry point (assets served under /os/)
├── favicon.ico
├── manifest.json
├── asset-manifest.json
├── me.jpg                  # Profile photo
├── resume.pdf              # Downloadable resume
├── robots.txt
│
├── static/
│   ├── css/                # Compiled stylesheets
│   ├── js/                 # React bundle + chunks
│   └── media/              # Fonts, images, audio tracks
│
├── js-dos/                 # DOSBox WebAssembly emulator
│   ├── js-dos.js
│   ├── wdosbox.wasm
│   └── wdosbox.shared.wasm
│
├── doom.jsdos              # Doom game bundle
├── digger.jsdos            # Digger game bundle
├── scrabble.jsdos          # Scrabble game bundle
└── trail.jsdos             # Oregon Trail game bundle
```

---

## Running Locally

The app assets reference the `/os/` path prefix, so it must be served from a parent directory:

```bash
# Clone the repo
git clone https://github.com/jitesh523/jitesh.solutions.git

# Create the /os/ structure and serve
mkdir -p /tmp/portfolio/os
cp -r jitesh.solutions/. /tmp/portfolio/os/
cd /tmp/portfolio
python3 -m http.server 8080
```

Open **http://localhost:8080/os/** in your browser.

---

## Deployment

To deploy on any static host (Netlify, Vercel, GitHub Pages), ensure the site is served from a sub-path named `os/` or configure a rewrite rule to map `/` → `/os/`.

**Netlify example** (`netlify.toml`):
```toml
[[redirects]]
  from = "/*"
  to = "/os/:splat"
  status = 200
```

---

## Contact

Built with ☕ and a deep love for retro aesthetics.

**Rachamadugu Jitesh**
- GitHub: [@jitesh523](https://github.com/jitesh523)
- Use the **CONTACT** window inside the portfolio to send a message directly

---

*© 2025 Rachamadugu Jitesh — Portfolio '25*
