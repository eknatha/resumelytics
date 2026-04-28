# resumelytics 📄

> **Free ATS Resume Analyzer & Job Search Toolkit** — instant, browser-side, zero backend needed.

![HTML](https://img.shields.io/badge/HTML-single--file-orange?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![No backend](https://img.shields.io/badge/backend-none-blue?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/deploy-GitHub%20Pages-black?style=flat-square)
![Mobile Friendly](https://img.shields.io/badge/mobile-friendly-brightgreen?style=flat-square)
![Dark Mode](https://img.shields.io/badge/dark%20mode-supported-9B59B6?style=flat-square)
![Features](https://img.shields.io/badge/features-25+-blueviolet?style=flat-square)
![Analytics](https://img.shields.io/badge/analytics-Plausible-4F46E5?style=flat-square)

🔗 **Live demo:** [eknatha.github.io/resumelytics](https://eknatha.github.io/resumelytics/)

---

## ✨ What is resumelytics?

**resumelytics** is a fully client-side ATS resume analyzer and job search toolkit packed with 25+ tools — from instant ATS scoring and keyword heatmaps to salary negotiation emails and notice period calculators.

Upload your resume, paste a job description, and get an instant score out of 100 with specific fixes, keyword match analysis, a recruiter's perspective on every issue, and a full suite of job preparation tools — all running 100% in the browser. No signup. No cost. No data leaves your device.

---

## 🚀 Features

| Feature | Details |
|---|---|
| 📁 File support | PDF, DOCX, TXT — drag & drop or browse |
| ⚠️ File size warning | Auto-flags files >1MB (caution) and >2MB (critical — will fail ATS portals) |
| 📊 ATS score | Animated score ring out of 100 with grade label (Excellent / Good / Fair / Needs Work) |
| 🔍 6-dimension analysis | Sections, quantified impact, action verbs, formatting, length, keyword match |
| 🎯 JD keyword match | Paste a JD → keyword match % + found vs. missing keyword chips |
| 🔥 Skill gap heatmap | Visual grid: matched JD skills (green) vs. missing skills (red) with % coverage |
| ✨ Animated keyword highlight | Resume text viewer with JD keywords lighting up with staggered animation |
| 👤 Recruiter perspective | Every issue card shows a real recruiter's view on that specific problem |
| 🔁 Overused word detector | Flags weak phrases with count + stronger alternatives |
| 🏆 Certification spotlight | Auto-detects CKA, CKS, AWS, GCP, Terraform, PMP and 14 other certs |
| 🔤 Tense consistency checker | Detects mixed past/present tense — flags exact lines with fix suggestions |
| 📅 Gap year detector | Visual career timeline with colour-coded bars — flags gaps ≥ 6 months |
| ⚖️ Resume A/B compare | Upload two versions → side-by-side score diff + 5-metric bar chart |
| ✍️ Bullet point rewriter | Paste weak bullet → 3 upgraded versions with strong verbs + impact framing |
| 💰 Salary range estimator | ₹ salary bands for 12 India role/level combos (DevOps, SRE, Platform, Backend, Cloud) |
| 📨 Referral message generator | 4-field form → tailored LinkedIn DM / email referral ask |
| 💼 Salary negotiation email | 6-field form → polished negotiation email with % gap + midpoint suggestion |
| 📆 Notice period calculator | Date picker + period → resignation date, days remaining + full email draft |
| 🎤 Interview question generator | 6–10 tailored questions based on resume + JD |
| ▲ Collapsible result sections | All panels collapse/expand — reduce scroll fatigue |
| 🌙 Dark mode | Header toggle, localStorage, respects OS preference |
| 📱 Mobile-first design | Fully responsive — phones, tablets, and desktops |
| 📊 Plausible analytics | Privacy-first, no-cookie analytics — no GDPR issues |
| 💡 ATS tips | 6 built-in quick-fix tips |
| ⚡ Zero dependencies | No npm, no build step, no framework — single HTML file |

---

## 📐 Scoring breakdown

| Dimension | With JD | Without JD |
|---|---|---|
| Section completeness | 22% | 28% |
| Quantified impact | 18% | 22% |
| Action verbs | 15% | 20% |
| ATS formatting | 15% | 18% |
| Resume length | 10% | 12% |
| JD keyword match | 20% | — |

**Score grades:**

| Score | Grade | Meaning |
|---|---|---|
| 80–100 | Excellent | Strong ATS pass |
| 65–79 | Good | Likely to pass screening |
| 45–64 | Fair | May struggle with some ATS |
| 0–44 | Needs Work | High rejection risk |

---

## 📅 Gap year detector

Automatically runs after every analysis. Parses year ranges from the resume text and builds a visual horizontal timeline with colour-coded bars:

- **Green** — Employment period
- **Blue** — Education period
- **Red dashed** — Gap detected

Gaps ≥ 6 months are flagged with a preparation tip. Only appears when enough date data is detected in the resume.

---

## ⚖️ Resume A/B compare

Upload two resume files (PDF / DOCX / TXT) as Version A and Version B → click Compare:

- Side-by-side score cards with the winner highlighted
- `+X pts` / `−X pts` score difference indicator
- 5-metric bar chart: sections, quantified impact, action verbs, formatting, length

Useful for validating improvements before sending an updated resume.

---

## 💼 Salary negotiation email

6 fields — your name, HR name, role, company, offer received (₹L/yr), counter ask (₹L/yr):

- Calculates the % gap between offer and counter
- Suggests a midpoint as a fallback ask
- Auto-pulls your top 2 skills detected from the uploaded resume
- Includes an early 6-month review as an alternative ask
- One-click copy to clipboard

> Tip: Send within 24–48 hours of receiving the offer. Keep your tone warm — you're negotiating a partnership.

---

## 📆 Notice period calculator

4 fields — your name, manager's name, last working day (date picker), notice period (30/45/60/90 days):

- Calculates exact resignation date
- Shows days remaining until last working day
- Generates a complete, professional resignation email draft
- One-click copy to clipboard

---

## 📊 Plausible analytics

Privacy-first analytics via [Plausible.io](https://plausible.io) — no cookies, no fingerprinting, fully GDPR-compliant. Tracks page views and key interactions without collecting any personal data.

To activate: add your domain in the [Plausible dashboard](https://plausible.io/sites) after deploying to GitHub Pages. The script is already included in `<head>`.


---

## 🧰 Tech stack

| Library | Version | Purpose |
|---|---|---|
| [PDF.js](https://mozilla.github.io/pdf.js/) | 3.11.174 | Extract text from PDF resumes |
| [Mammoth.js](https://github.com/mwilliamson/mammoth.js) | 1.6.0 | Extract text from DOCX resumes |
| [Plausible](https://plausible.io) | latest | Privacy-first analytics |
| Vanilla JS + CSS | — | Everything else |

Fonts: DM Serif Display + Figtree + DM Mono via Google Fonts.

---

## 🗺️ Roadmap

- [x] PDF, DOCX, TXT upload + drag & drop
- [x] File size warning (>1MB caution / >2MB critical)
- [x] 6-dimension ATS scoring engine
- [x] JD keyword match % with chip view
- [x] Skill gap heatmap
- [x] Animated keyword highlight viewer
- [x] Recruiter perspective notes on every issue
- [x] Overused word detector with alternatives
- [x] Certification spotlight (14 cert types)
- [x] Tense consistency checker
- [x] Gap year detector with visual career timeline
- [x] Resume A/B compare (score diff + metric breakdown)
- [x] Bullet point rewriter (3 versions, click to copy)
- [x] Salary range estimator (12 India role/level combos)
- [x] Referral message generator
- [x] Salary negotiation email generator
- [x] Notice period calculator + resignation email
- [x] Interview question generator (role-aware, 6–10 Qs)
- [x] Collapsible result sections
- [x] Dark mode (localStorage + OS preference)
- [x] Mobile-first responsive design
- [x] Plausible privacy-first analytics
- [ ] Score history — sparkline chart of improvement over time
- [ ] "Share my score" PNG card for LinkedIn
- [ ] Export score report as PDF
- [ ] Role presets — pre-loaded keyword sets (DevOps / SRE / Backend / Data)
- [ ] PWA — installable on phone home screen
- [ ] AI deep analysis via Cloudflare Worker → Claude API backend
- [ ] Job board URL scanner (paste LinkedIn/Naukri URL → auto-fetch JD)

---

## 🤖 AI feature — coming soon

**Planned architecture:**

```
Browser  →  Cloudflare Worker / Vercel Edge  →  Claude API
```

Keeps the API key server-side, avoids CORS, zero infrastructure cost on the free tier. The "Deep AI Analysis" panel is already in the UI — just needs the backend wired up.

---

## 🤝 Contributing

1. Fork the repo
2. Edit `index.html` (entire app lives here)
3. Test with a real PDF, DOCX, and pasted plain text — on desktop and mobile, in light and dark mode
4. Open a PR with a brief description of what changed and why

Single-file, no-build-step philosophy — please keep it that way.

---

## 📄 License

MIT — free to use, fork, and deploy.

---

<p align="center">
  Built with ❤️ by <a href="https://eknathalabs.com/">EknathaLabs</a> for job seekers
  &nbsp;·&nbsp;
  <a href="https://github.com/eknatha">@eknatha</a>
</p>
