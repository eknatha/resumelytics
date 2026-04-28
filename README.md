# resumelytics 📄

> **Free ATS Resume Analyzer & Score Checker** — instant, browser-side, zero backend needed.

![HTML](https://img.shields.io/badge/HTML-single--file-orange?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![No backend](https://img.shields.io/badge/backend-none-blue?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/deploy-GitHub%20Pages-black?style=flat-square)

🔗 **Live demo:** [eknathareddyp.github.io/resumelytics](https://eknathareddyp.github.io/resumelytics/)

---

## ✨ What is resumelytics?

**resumelytics** analyzes your resume against common ATS (Applicant Tracking System) rules and gives you an instant score out of 100 — with specific, actionable feedback. Paste a job description to also see your keyword match percentage.

Everything runs **100% in the browser**. No data is sent to any server. No signup. No cost.

---

## 🚀 Features

| Feature | Details |
|---|---|
| 📁 File support | PDF, DOCX, TXT — drag & drop or browse |
| 🎯 JD keyword match | Paste a job description → see found vs. missing keywords |
| 📊 ATS score | Animated score ring out of 100 with grade label |
| 🔍 6-dimension analysis | Sections, quantified impact, action verbs, formatting, length, keyword match |
| ⚠️ Issue cards | Severity-tagged: Critical / Warning / Suggestion / Pass |
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

## 🛠️ Getting started

### Deploy to GitHub Pages (recommended)

```bash
# 1. Fork or clone this repo
git clone https://github.com/eknathareddyp/resumelytics.git
cd resumelytics

# 2. Push to your GitHub
git remote set-url origin https://github.com/YOUR_USERNAME/resumelytics.git
git push -u origin main
```

Then enable Pages: **GitHub repo → Settings → Pages → Source → main / root**

Your site will be live at: `https://YOUR_USERNAME.github.io/resumelytics/`

---

### Run locally

```bash
git clone https://github.com/eknathareddyp/resumelytics.git
cd resumelytics
open index.html   # or double-click the file
```

> **Note for PDF support:** PDF.js requires a local HTTP server due to CORS.
> Use VS Code [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) or:
>
> ```bash
> python3 -m http.server 8000
> # Open http://localhost:8000 in your browser
> ```

---

## 📁 Repo structure

```
resumelytics/
├── index.html     ← entire app (single file)
└── README.md
```

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

- [ ] **AI-powered analysis** — deep role-specific feedback via backend API (Claude / OpenAI)
- [ ] **Export as PDF** — download your ATS score report
- [ ] **Score history** — compare resume versions over time
- [ ] **Role presets** — keyword templates for DevOps, SRE, Backend, Data Engineering, etc.
- [ ] **Dark mode**
- [ ] **LinkedIn import** — paste LinkedIn URL to auto-populate resume text

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
3. Test with a real PDF, a DOCX, and pasted plain text
4. Open a PR describing what you changed and why

Please keep the single-file, no-build-step philosophy intact.

---

## 📄 License

MIT — free to use, fork, and deploy.

---

<p align="center">
  Built with ❤️ by <a href="https://eknathalabs.com/">EknathaLabs</a> for job seekers
  &nbsp;·&nbsp;
  <a href="https://github.com/eknathareddyp">@eknathareddyp</a>
</p>
