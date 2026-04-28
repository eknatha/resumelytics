# resumelytics 📄

> **Free ATS Resume Analyzer & Score Checker** — instant, browser-side, zero backend needed.

![HTML](https://img.shields.io/badge/HTML-single--file-orange?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![No backend](https://img.shields.io/badge/backend-none-blue?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/deploy-GitHub%20Pages-black?style=flat-square)
![Mobile Friendly](https://img.shields.io/badge/mobile-friendly-brightgreen?style=flat-square)

🔗 **Live demo:** [eknatha.github.io/resumelytics](https://eknatha.github.io/resumelytics/)

---

## ✨ What is resumelytics?

**resumelytics** analyzes your resume against common ATS (Applicant Tracking System) rules and gives you an instant score out of 100 — with specific, actionable feedback and a recruiter's perspective on every issue.

Paste a job description to unlock keyword match %, a skill gap heatmap, and animated keyword highlighting directly on your resume text.

Everything runs **100% in the browser**. No data is sent to any server. No signup. No cost.

---

## 🚀 Features

| Feature | Details |
|---|---|
| 📁 File support | PDF, DOCX, TXT — drag & drop or browse |
| 🎯 JD keyword match | Paste a job description → see found vs. missing keywords |
| 📊 ATS score | Animated score ring out of 100 with grade label |
| 🔍 6-dimension analysis | Sections, quantified impact, action verbs, formatting, length, keyword match |
| 🔥 Skill gap heatmap | Visual grid: matched skills (green) vs missing skills (red) with % coverage |
| ✨ Animated keyword highlight | Resume text viewer with JD keywords lighting up with staggered animation |
| 👤 Recruiter perspective | Every issue card shows what a real recruiter thinks when they see that problem |
| ⚠️ Issue cards | Severity-tagged: Critical / Warning / Suggestion / Pass |
| 📱 Mobile-first design | Fully responsive — works on phones, tablets, and desktops |
| 💡 ATS tips | 6 built-in quick-fix tips for job seekers |
| ⚡ Zero dependencies | No npm, no build step, no framework — single HTML file |

---

## 📐 Scoring breakdown

The ATS score is calculated across 6 dimensions, weighted based on whether a job description is provided:

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

## 🔥 Skill gap heatmap

When a job description is pasted, resumelytics extracts the most important keywords from the JD (weighted by frequency) and displays them as a color-coded grid:

- **Green cell (✓)** — keyword found in your resume
- **Red cell (✗)** — keyword missing from your resume
- Summary stat: `X of Y JD skills matched · Z% coverage`

---

## ✨ Animated keyword highlight

After analysis, your resume text renders in a scrollable viewer where every matched JD keyword animates in with a staggered green highlight — so you can visually confirm exactly which terms are landing and which sections need more keyword coverage.

---

## 👤 Recruiter perspective notes

Every issue card includes a recruiter's real-world take. For example:

> *"Without numbers, recruiters can't gauge impact. 'Improved performance' tells me nothing. 'Improved response time by 60%' tells me everything."*

9 unique recruiter notes cover: missing sections, weak action verbs, no quantified achievements, ATS formatting issues, resume length, missing LinkedIn, missing GitHub, and low keyword match.


---

## 🧰 Tech stack

| Library | Version | Purpose |
|---|---|---|
| [PDF.js](https://mozilla.github.io/pdf.js/) | 3.11.174 | Extract text from PDF resumes |
| [Mammoth.js](https://github.com/mwilliamson/mammoth.js) | 1.6.0 | Extract text from DOCX resumes |
| Vanilla JS + CSS | — | Scoring engine, UI, animations |

Fonts: [DM Serif Display](https://fonts.google.com/specimen/DM+Serif+Display) + [Figtree](https://fonts.google.com/specimen/Figtree) + [DM Mono](https://fonts.google.com/specimen/DM+Mono) via Google Fonts.

---

## 🗺️ Roadmap

- [x] PDF, DOCX, TXT upload + drag & drop
- [x] 6-dimension ATS scoring engine
- [x] JD keyword match %
- [x] Skill gap heatmap
- [x] Animated keyword highlight viewer
- [x] Recruiter perspective notes on every issue
- [x] Mobile-first responsive design
- [ ] Dark mode toggle
- [ ] Score history (compare resume versions)
- [ ] Export score report as PDF
- [ ] Role presets (DevOps / SRE / Backend / Data Engineer keyword templates)
- [ ] Resume A/B compare (upload two versions, see score diff)
- [ ] AI-powered deep analysis via backend API (Claude / OpenAI)
- [ ] Job board URL scanner (paste LinkedIn/Naukri URL → auto-fetch JD)

---

## 🤖 AI feature — coming soon

The "Deep AI Analysis" section is reserved for a future backend integration. The current release is intentionally API-free so it works as a zero-cost static site.

**Planned architecture:**

```
Browser  →  Cloudflare Worker / Vercel Edge  →  Claude API
```

This keeps the API key server-side and avoids CORS issues. Contributions welcome.

---

## 🤝 Contributing

PRs and issues are welcome!

1. Fork the repo
2. Edit `index.html` (entire app lives here)
3. Test with a real PDF, a DOCX, and pasted plain text — on both desktop and mobile
4. Open a PR describing what you changed and why

Please keep the single-file, no-build-step philosophy intact.

---

## 📄 License

MIT — free to use, fork, and deploy.

---

<p align="center">
  Built with ❤️ by <a href="https://eknathalabs.com/">EknathaLabs</a> for job seekers
  &nbsp;·&nbsp;
  <a href="https://github.com/eknatha">@eknatha</a>
</p>
