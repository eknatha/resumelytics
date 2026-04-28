# resumelytics 📄

> **Free ATS Resume Analyzer & Score Checker** — instant, browser-side, zero backend needed.

![HTML](https://img.shields.io/badge/HTML-single--file-orange?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![No backend](https://img.shields.io/badge/backend-none-blue?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/deploy-GitHub%20Pages-black?style=flat-square)
![Mobile Friendly](https://img.shields.io/badge/mobile-friendly-brightgreen?style=flat-square)
![Dark Mode](https://img.shields.io/badge/dark%20mode-supported-9B59B6?style=flat-square)
![Features](https://img.shields.io/badge/features-20+-blueviolet?style=flat-square)

🔗 **Live demo:** [eknatha.github.io/resumelytics](https://eknatha.github.io/resumelytics/)

---

## ✨ What is resumelytics?

**resumelytics** is a fully client-side ATS resume analyzer packed with 20+ tools to help job seekers write, fix, and prepare better resumes — with zero backend, zero signup, and zero cost.

Upload your resume, paste a job description, and get an instant score out of 100 with specific fixes, keyword match analysis, a recruiter's perspective on every issue, and a full suite of job preparation tools — all running 100% in the browser.

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
| 🔁 Overused word detector | Flags weak phrases ("responsible for", "worked on") with count + stronger alternatives |
| 🏆 Certification spotlight | Auto-detects CKA, CKS, AWS, GCP, Terraform, PMP and 14 other certs — displays as icon cards |
| 🔤 Tense consistency checker | Detects mixed past/present tense — flags exact lines with fix suggestions |
| ✍️ Bullet point rewriter | Paste weak bullet → get 3 upgraded versions with strong verbs + impact framing |
| 💰 Salary range estimator | ₹ salary bands for 12 India role/level combos (DevOps, SRE, Platform, Backend, Cloud) |
| 📨 Referral message generator | 4-field form → tailored LinkedIn DM / email referral ask with auto-detected skills |
| 🎤 Interview question generator | 6–10 tailored questions based on resume + JD (DevOps, Cloud, Leadership, Behavioral) |
| ▲ Collapsible result sections | All panels collapse/expand individually — reduce scroll fatigue on long reports |
| 🌙 Dark mode | Header toggle, saved to localStorage, respects OS preference on first visit |
| 📱 Mobile-first design | Fully responsive — tested on phones, tablets, and desktops |
| 💡 ATS tips | 6 built-in quick-fix tips for job seekers |
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

## 🔁 Overused word detector

Scans resume text for 15 common weak phrases and shows:
- The exact phrase detected with occurrence count
- A red frequency bar scaled to how often it appears
- 2–4 stronger action verb alternatives

Detected phrases include: `responsible for`, `worked on`, `helped with`, `team player`, `detail-oriented`, `passionate about`, `leverage`, `synergy`, `proactive`, and more.

---

## 🏆 Certification spotlight

Automatically detects 14 certification types and displays them as icon cards:

| Cert | Full name |
|---|---|
| CKA / CKS / CKAD | Kubernetes certifications |
| AWS Certified | All AWS cert variants |
| GCP / Azure AZ-xxx | Google Cloud & Microsoft Azure |
| Terraform Associate | HashiCorp certification |
| PMP | Project Management Professional |
| CCNA / CCNP | Cisco networking |
| RHCE / RHCSA | Red Hat certifications |
| CISSP | Security certification |
| SAFe | Scaled Agile Framework |

---

## 💰 Salary range estimator

12 role + experience level combinations with India market data (2024–25):

| Role | Level | Range |
|---|---|---|
| DevOps Engineer | Junior (0–3 yrs) | ₹5–10L/yr |
| DevOps Engineer | Mid (3–6 yrs) | ₹12–22L/yr |
| DevOps Engineer | Senior (6–10 yrs) | ₹22–38L/yr |
| SRE | Mid (3–6 yrs) | ₹14–24L/yr |
| SRE | Senior (6–10 yrs) | ₹24–42L/yr |
| Platform Engineer | Mid (3–6 yrs) | ₹16–28L/yr |
| Platform Engineer | Senior (6–10 yrs) | ₹26–45L/yr |
| Platform Engineer | Principal (10+ yrs) | ₹40–70L/yr |
| Backend Engineer | Mid / Senior | ₹14–42L/yr |
| Cloud Architect | Mid / Senior | ₹18–55L/yr |

Each estimate includes a median, market context tags, and a recruiter insight tip.

---

## 📨 Referral message generator

Fill 4 fields — contact name, company, role, your name — and get a tailored referral ask message for LinkedIn DM or email. The message auto-pulls:

- Your top 3 detected skills from the resume (Kubernetes, Terraform, cloud, etc.)
- Implied years of experience from date ranges in the resume
- One-click copy to clipboard

---

## ▲ Collapsible result sections

Every results panel can be individually collapsed or expanded using the toggle button in the section header. Useful when re-analyzing multiple times — collapse sections you've already acted on. All sections reset to expanded on "Analyze another resume."

---

## 🧰 Tech stack

| Library | Version | Purpose |
|---|---|---|
| [PDF.js](https://mozilla.github.io/pdf.js/) | 3.11.174 | Extract text from PDF resumes |
| [Mammoth.js](https://github.com/mwilliamson/mammoth.js) | 1.6.0 | Extract text from DOCX resumes |
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
- [x] Bullet point rewriter (3 versions, click to copy)
- [x] Salary range estimator (12 India role/level combos)
- [x] Referral message generator (LinkedIn DM / email)
- [x] Interview question generator (role-aware, 6–10 questions)
- [x] Collapsible result sections
- [x] Dark mode (localStorage + OS preference)
- [x] Mobile-first responsive design
- [ ] Score history — compare versions over time with sparkline chart
- [ ] Export score report as PDF
- [ ] Role presets — pre-loaded keyword sets (DevOps / SRE / Backend / Data)
- [ ] Resume A/B compare — score diff between two versions
- [ ] "Share my score" PNG card for LinkedIn
- [ ] PWA — installable on phone home screen
- [ ] AI deep analysis via Cloudflare Worker → Claude API backend

---

## 🤖 AI feature — coming soon

**Planned architecture:**

```
Browser  →  Cloudflare Worker / Vercel Edge  →  Claude API
```

Keeps the API key server-side, avoids CORS, zero infrastructure cost on the free tier.

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
