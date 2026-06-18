# Cursor IDE Onboarding — Setup Report & Research Project

## Tools Installed

### 1. Cursor IDE
- Downloaded and installed from https://cursor.com/
- Platform: Windows 11

### 2. Claude Code Extension
- Installed via Cursor Extensions panel (search: "Claude Code")
- Logged in using Anthropic Console account (API key)

### 3. Codex Extension
- Installed via Cursor Extensions panel (search: "Codex")
- Installed by OpenAI (6.4M downloads)

---

## Research Project: AI-Powered SEO Content Production

### Why This Topic
AI-powered SEO content production sits at the intersection of my background in UI/UX design, web development, and digital marketing. As AI tools reshape how content is created and ranked, understanding how top practitioners use AI in their SEO workflows is directly applicable to real client work.

### Expert Selection Criteria
- Active publishers in 2025–2026 (not just theorists)
- Practitioner background with real client/agency experience
- Strong engagement on LinkedIn and/or YouTube
- Focus on the AI + SEO intersection specifically

### 10 Experts Selected

| # | Name | Focus | Platform |
|---|------|-------|----------|
| 1 | Nathan Gotch | AI SEO frameworks, agentic SEO | YouTube + LinkedIn |
| 2 | Lily Ray | Google updates, AI Overviews, content quality | LinkedIn + X |
| 3 | Aleyda Solís | Technical SEO, GEO/AEO strategy | YouTube + LinkedIn |
| 4 | Mike King | Relevance Engineering, AI/ML in SEO | YouTube + LinkedIn |
| 5 | Kevin Indig | AI Overviews data, LLM traffic research | LinkedIn + Newsletter |
| 6 | Ryan Law | Expert-led content, thought leadership | LinkedIn + Newsletter |
| 7 | Cyrus Shepard | Data-driven SEO experiments | LinkedIn + X |
| 8 | Brian Dean | AI content production, SEO frameworks | LinkedIn |
| 9 | Rand Fishkin | AI search visibility, audience research | YouTube + LinkedIn |
| 10 | Jori Ford | AI crawler behavior, technical experiments | LinkedIn + YouTube |

### Repository Structure

research/

├── sources.md                    # All 10 experts with links and annotations

├── linkedin-posts/               # Recent posts collected manually

│   ├── nathan-gotch.md

│   ├── lily-ray.md

│   ├── aleyda-solis.md

│   ├── mike-king.md

│   ├── kevin-indig.md

│   ├── ryan-law.md

│   ├── cyrus-shepard.md

│   ├── brian-dean.md

│   ├── rand-fishkin.md

│   └── jori-ford.md

└── youtube-transcripts/          # Transcripts via Supadata API

├── nathan-gotch-video1.md

├── nathan-gotch-video2.md

├── aleyda-solis-video1.md

├── aleyda-solis-video2.md

├── rand-fishkin-video1.md

├── rand-fishkin-video2.md

├── mike-king-video1.md

├── mike-king-video2.md

├── cyrus-shepard-video1.md

├── cyrus-shepard-video2.md

├── lily-ray-video1.md

├── lily-ray-video2.md

├── kevin-indig-video1.md

├── kevin-indig-video2.md

├── ryan-law-video1.md

├── ryan-law-video2.md

├── jori-ford-video1.md

└── jori-ford-video2.md
Data Collection Method

LinkedIn posts: Collected manually from each expert's profile (2–3 posts per expert)
YouTube transcripts: Collected via Supadata API using PowerShell in Cursor terminal


Setup Issues Encountered & Solutions
Issue 1: npm not recognized after installing Node.js
Solution: Closed and reopened Cursor IDE to reload PATH.
Issue 2: PowerShell execution policy blocked npm scripts
Solution: Ran Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
Issue 3: SSL certificate error during Claude Code install
Solution: Used --strict-ssl=false flag during npm install.
Issue 4: Claude Code requires Pro/Max subscription
Solution: Used Anthropic Console API key instead.
Issue 5: git not recognized
Solution: Installed Git for Windows from https://git-scm.com/download/win
Issue 6: PowerShell curl incompatible with standard flags
Solution: Used Invoke-RestMethod with -Headers @{"x-api-key"="..."} format instead.