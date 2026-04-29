# resumelytics 📄

> **Free ATS Resume Analyzer & Job Search Toolkit** — instant, browser-side, zero backend needed.

![HTML](https://img.shields.io/badge/HTML-single--file-orange?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![No backend](https://img.shields.io/badge/backend-none-blue?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/deploy-GitHub%20Pages-black?style=flat-square)
![Mobile Friendly](https://img.shields.io/badge/mobile-friendly-brightgreen?style=flat-square)
![Dark Mode](https://img.shields.io/badge/dark%20mode-supported-9B59B6?style=flat-square)
![Features](https://img.shields.io/badge/features-30+-blueviolet?style=flat-square)
![Analytics](https://img.shields.io/badge/analytics-Plausible-4F46E5?style=flat-square)

🔗 **Live demo:** [eknatha.github.io/resumelytics](https://eknatha.github.io/resumelytics/)

---

## ✨ What is resumelytics?

**resumelytics** is a fully client-side ATS resume analyzer and job search toolkit with 30+ tools — from instant ATS scoring and skill gap heatmaps to salary negotiation emails, notice period calculators, and an India-specific CTC take-home calculator.

Everything runs **100% in the browser**. No data is sent to any server. No signup. No cost.

---

## 🚀 Features

| Feature | Details |
|---|---|
| 📁 File support | PDF, DOCX, TXT — drag & drop or browse |
| ⚠️ File size warning | Auto-flags files >1MB (caution) and >2MB (critical — will fail ATS portals) |
| 📊 ATS score | Animated score ring out of 100 with grade label |
| 🔍 6-dimension analysis | Sections, quantified impact, action verbs, formatting, length, keyword match |
| 🎯 JD keyword match | Paste a JD → keyword match % + found vs. missing keyword chips |
| 🔥 Skill gap heatmap | Visual grid: matched JD skills (green) vs. missing skills (red) |
| ✨ Animated keyword highlight | Resume text viewer with JD keywords lighting up with staggered animation |
| 👤 Recruiter perspective | Every issue card shows a real recruiter's view |
| 🗺️ Score improvement roadmap | Prioritized action plan ranked by points each fix adds |
| 🔁 Overused word detector | Flags weak phrases with count + stronger alternatives |
| 🏆 Certification spotlight | Auto-detects CKA, CKS, AWS, GCP, Terraform, PMP and more |
| 🔤 Tense consistency checker | Detects mixed past/present tense with fix suggestions |
| 👁️ Before / after preview | Side-by-side bullet rewrites — weak vs. strong |
| 🐾 Resume health pet | Pixel-art pet whose health reflects your ATS score |
| 📅 Career timeline | Visual career timeline with colour-coded gap detector |
| ⚖️ Resume A/B compare | Upload two versions → side-by-side score diff + metric chart |
| ✍️ Bullet point rewriter | Paste weak bullet → 3 upgraded versions, click to copy |
| 💰 Salary range estimator | ₹ salary bands for 12 India role/level combos |
| 🧮 CTC take-home calculator | Full breakdown: PF, PT, income tax, joining bonus TDS |
| 📨 Referral message generator | 4-field form → tailored LinkedIn DM / email referral ask |
| 💼 Salary negotiation email | 6-field form → polished negotiation email with midpoint |
| 📆 Notice period calculator | Date picker → resignation date + email draft |
| 🎤 Interview question generator | 6–10 tailored questions based on resume + JD |
| 🔥 Score roast mode | Snarky recruiter-voice commentary on your score |
| 👁️ 6-second scan simulator | Blur simulator — see what a recruiter sees first |
| 📧 Cold outreach email | 5-field form → personalized cold email |
| ✉️ Interview follow-up email | 5-field form → warm thank-you + follow-up |
| ▲ Collapsible result sections | All panels collapse/expand individually |
| 🌙 Dark mode + High contrast | Header toggle, localStorage, respects OS preference |
| 🔡 Font size toggle | A+ / A++ / A+++ cycling, saved to localStorage |
| 📱 Mobile-first design | Fully responsive — phones, tablets, desktops |
| 📊 Plausible analytics | Privacy-first, no-cookie analytics |
| 💡 ATS tips | 6 built-in quick-fix tips |
| ⚡ Zero dependencies | No npm, no build step, no framework — single HTML file |

---

## 📐 ATS scoring breakdown

| Dimension | With JD | Without JD |
|---|---|---|
| Section completeness | 22% | 28% |
| Quantified impact | 18% | 22% |
| Action verbs | 15% | 20% |
| ATS formatting | 15% | 18% |
| Resume length | 10% | 12% |
| JD keyword match | 20% | — |

| Score | Grade | Meaning |
|---|---|---|
| 80–100 | Excellent | Strong ATS pass |
| 65–79 | Good | Likely to pass screening |
| 45–64 | Fair | May struggle with some ATS |
| 0–44 | Needs Work | High rejection risk |

---

## 🧮 CTC take-home calculator

Calculates real monthly take-home after all deductions with 6 configurable inputs:

**Inputs:** Annual CTC (₹L), Joining bonus (₹L), PF mode, Basic salary split, Income tax regime, Professional tax (state)

**Deductions calculated:**
- Employer PF contribution (subtracted from CTC to arrive at gross)
- Employee PF (standard cap ₹1800/mo or full 12% of basic)
- Professional tax (₹200/mo for KA/MH/AP, ₹150/mo Telangana, or ₹0)
- Income tax + 4% health & education cess

**Tax regimes supported:**

| Regime | Key feature |
|---|---|
| New regime 2025-26 | 0% up to ₹4L · Zero tax if taxable income ≤ ₹12L (87A rebate) |
| New regime 2024-25 | 0% up to ₹3L · Zero tax if taxable income ≤ ₹7L (87A rebate) |
| Old regime | Assumes 80C (₹1.5L) + HRA (40% of basic) + standard deduction ₹50K |
| No tax | For freshers / income under ₹12L |

**2025-26 new regime slabs (Budget 2025):**

| Taxable income | Rate |
|---|---|
| Up to ₹4L | 0% |
| ₹4L – ₹8L | 5% |
| ₹8L – ₹12L | 10% |
| ₹12L – ₹16L | 15% |
| ₹16L – ₹20L | 20% |
| ₹20L – ₹24L | 25% |
| Above ₹24L | 30% |

> **Key 2025-26 change:** Rebate u/s 87A raised from ₹7L to ₹12L — most people earning under ₹12.75L CTC pay zero income tax under the new regime.

**Joining bonus:** Shows gross bonus → TDS (~30%) → net bonus in hand, and calculates first month take-home (salary + net bonus).

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
- [x] File size warning (>1MB / >2MB)
- [x] 6-dimension ATS scoring engine
- [x] JD keyword match % with chip view
- [x] Skill gap heatmap
- [x] Animated keyword highlight viewer
- [x] Recruiter perspective notes on every issue
- [x] Score improvement roadmap
- [x] Overused word detector with alternatives
- [x] Certification spotlight (12+ cert types)
- [x] Tense consistency checker
- [x] Before / after bullet preview
- [x] Resume health pet (pixel-art)
- [x] Gap year detector with visual career timeline
- [x] Resume A/B compare (score diff + metric breakdown)
- [x] Bullet point rewriter (3 versions, click to copy)
- [x] Salary range estimator (12 India role/level combos)
- [x] CTC take-home calculator (2025-26 & 2024-25 slabs, PF, PT, bonus TDS)
- [x] Referral message generator
- [x] Salary negotiation email generator
- [x] Notice period calculator + resignation email
- [x] Interview question generator (role-aware, 6–10 Qs)
- [x] Score roast mode
- [x] 6-second scan simulator
- [x] Cold outreach email generator
- [x] Interview follow-up email generator
- [x] Collapsible result sections
- [x] Dark mode + High contrast mode
- [x] Font size toggle (A+ / A++ / A+++)
- [x] Mobile-first responsive design
- [x] Plausible privacy-first analytics
- [ ] Score history sparkline — improvement over time
- [ ] "Improve by X pts" goal badge
- [ ] "Share my score" PNG card for LinkedIn
- [ ] Export score report as PDF
- [ ] PWA — installable on phone home screen
- [ ] Cover letter checker
- [ ] Passive voice detector
- [ ] Bullet length color-coder
- [ ] AI deep analysis via Cloudflare Worker → Claude API

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
3. Test with PDF, DOCX, and pasted text — on desktop and mobile, light and dark mode
4. Open a PR with a brief description

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
