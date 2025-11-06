# Raven Mott — Portfolio

A single‑file, dependency‑free **personal portfolio website** built with plain **HTML/CSS/JS**. It highlights projects (Gestura, CropNet, Food Website), research, experience, and includes an embedded Google Form for contact.

Live demo (optional): host on GitHub Pages, Netlify, or Vercel following the instructions below.

---

## ✨ Features

* **Single file** (`index.html`) — quick to deploy anywhere
* **Responsive** layout with accessible markup
* **Sections:** About, Education, Projects, Research, Experience, Contact, Resume
* **Project links** wired:

  * Gestura — [https://github.com/Rmot1202/Gestura](https://github.com/Rmot1202/Gestura)
  * Food Website — [https://github.com/Rmot1202/Food-Website](https://github.com/Rmot1202/Food-Website) • Demo: [https://rmot1202.pythonanywhere.com/](https://rmot1202.pythonanywhere.com/)
  * CropNet — [https://github.com/Rmot1202/Cropnet](https://github.com/Rmot1202/Cropnet)
* **Contact** via embedded Google Form
* **Zero build tools** required

---

## 🗂 Project Structure

```
.
└── index.html          # Your entire portfolio site
```

If you add a resume PDF, place it next to `index.html`:

```
.
├── index.html
└── Raven_Mott_Resume.pdf
```

---

## 🚀 Quick Start

1. **Download** `index.html` (from this repo or ChatGPT canvas).
2. (Optional) Place your resume as `Raven_Mott_Resume.pdf` in the same folder.
3. Open `index.html` locally to preview.

---

## 🔧 Customize

Open `index.html` and edit the items below:

| Area          | What to change                               | Where                 |
| ------------- | -------------------------------------------- | --------------------- |
| Name/Title    | "Raven Mott" and page `<title>`              | Header + `<head>`     |
| Meta          | `<meta name="description">`, Open Graph tags | `<head>`              |
| Highlights    | Bulleted items in **Highlights** card        | `.hero-card`          |
| Skills chips  | `<span class="chip">…</span>` list           | HERO section          |
| Education     | Degree/GPA/scholarships                      | `#education` section  |
| Projects      | Titles, descriptions, links                  | `#projects` section   |
| Research      | Project names & blurbs                       | `#research` section   |
| Experience    | Roles & blurbs                               | `#experience` section |
| Contact email | `mailto:Mottraven43@gmail.com`               | `#contact` section    |
| Google Form   | `iframe src="…"`                             | `#contact` section    |
| Resume button | `Raven_Mott_Resume.pdf`                      | `#resume` section     |

> **Tip:** To embed a Google Form inline, use the **Send → `<> Embed`** option in Google Forms and paste the `src` it provides. The current file already embeds `https://forms.gle/H5KCoieyjJcjqdWL7`.

---

## 🌐 Deploy

Choose one host (all free for static sites):

### GitHub Pages

1. Create a new repo (e.g., `ravenmott.github.io` or any name).
2. Add `index.html` (and `Raven_Mott_Resume.pdf`).
3. In **Settings → Pages**:

   * If the repo is `ravenmott.github.io`: it auto‑publishes to `https://ravenmott.github.io/`.
   * Otherwise: set **Source** to `main` and **/ (root)**.

**CLI (optional):**

```bash
mkdir portfolio && cd portfolio
cp /path/to/index.html .
# optionally: cp Raven_Mott_Resume.pdf .
git init && git add . && git commit -m "Initial site"
# Using GitHub CLI
gh repo create ravenmott.github.io --public --source=. --push
```

### Netlify (drag‑and‑drop)

1. Log in → **Add new site → Deploy manually**.
2. Drag the folder containing `index.html`.
3. You’ll get `https://<random>.netlify.app`.

### Vercel (import from Git)

1. **New Project** → import your GitHub repo.
2. Framework: **Other** (no build step).
3. Build command: *None* • Output directory: `/`.

---

## 🔒 Privacy & Security Notes

* The contact form is hosted by **Google Forms**. Responses are stored in your Google account according to your form settings.
* If you later switch to a custom backend, ensure you validate inputs and protect any API keys.

---

## 🧰 Tech Notes

* Pure HTML/CSS with a small amount of vanilla JS for the footer year.
* Uses modern CSS (custom properties, `color-mix()` for subtle theming). Works in all current evergreen browsers; degrades gracefully.
* No frameworks, no external fonts.

---

## ✅ To‑Do (Optional Enhancements)

* Add a **/assets** folder (favicons, images)
* Add **SEO**: `og:image`, favicon, sitemap
* Add **Analytics** (Plausible or GA)
* Add a **Projects.json** + small JS to render cards from data
* Add **dark‑mode toggle** (currently adapts via `prefers-color-scheme`)

---

## 📝 License

If you intend others to reuse this template, add a license (MIT recommended). Example `LICENSE` contents:

```
MIT License — Copyright (c) 2025 Raven Mott
Permission is hereby granted, free of charge, to any person obtaining a copy...
```

---

## 🙌 Credits

Designed and authored by **Raven Mott**. Built as a lightweight, fast‑to‑deploy personal site showcasing Android, AI/ML, data science, and cybersecurity work.
