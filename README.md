# ps-template

A Claude Code skill that generates a stunning personal website from your resume PDF — deployed to GitHub Pages in minutes.

## Quick Start

**1. Fork this repo**

Click **Fork** on the top right, then rename it to your own name (e.g. `john-doe` or `yourname-site`) under **Settings → General → Repository name**.

**2. Clone your fork**

```bash
git clone https://github.com/<your-username>/<your-repo-name>
cd <your-repo-name>
```

**3. Enable GitHub Pages**

Go to **Settings → Pages → Source: GitHub Actions**

**4. Add your resume PDF**

Drop your resume PDF into the repo root.

**5. Generate your site**

Open Claude Code and run:

```
/resume-website
```

Claude reads your PDF, asks a few design questions, and generates `index.html`.

**6. Push to deploy**

```bash
git add index.html
git commit -m "Add personal site"
git push
```

Your site goes live at `https://<your-username>.github.io/<your-repo-name>/`

---

## How it works

- Claude reads your resume PDF and extracts all content
- Asks design questions (vibe, colors, animations)
- Generates a polished, production-grade `index.html` — pure HTML/CSS/JS, no build tools
- GitHub Actions auto-deploys on every push to `main`

## Stack

- Pure static HTML + CSS + JS
- Google Fonts via CDN
- GitHub Actions for CI/CD
- GitHub Pages for hosting
