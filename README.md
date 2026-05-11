# Manuel Rebol — Portfolio

Personal portfolio website for Manuel Rebol, Systems Engineering student at Universidad Tecnológica Nacional (UTN).

**Live site:** https://ManuelRebol.github.io

## Tech Stack

- HTML5, CSS3, Vanilla JavaScript — no frameworks, no build tools
- Deployed automatically via **GitHub Actions** → GitHub Pages

---

## 🚀 Deploy to GitHub Pages (first time setup)

### Step 1 — Create the GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Repository name: **`ManuelRebol.github.io`** (must match exactly)
3. Set visibility: **Public**
4. Do NOT add a README (you already have one)
5. Click **Create repository**

### Step 2 — Push your code

Open a terminal inside the `portfolio-landing-page/` folder and run:

```bash
git init
git add .
git commit -m "feat: initial portfolio"
git branch -M main
git remote add origin https://github.com/ManuelRebol/ManuelRebol.github.io.git
git push -u origin main
```

### Step 3 — Enable GitHub Actions as the Pages source

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Build and deployment → Source**, select **GitHub Actions**
4. Save

### Step 4 — Watch it deploy ✅

1. Go to the **Actions** tab of your repository
2. You'll see a workflow called **"Deploy to GitHub Pages"** running
3. Wait ~1-2 minutes
4. Visit **https://ManuelRebol.github.io** 🎉

---

## 🔄 Future updates

Every time you push to `main`, the site redeploys automatically — no extra steps needed:

```bash
git add .
git commit -m "update: your message here"
git push
```

---

## 📁 Project structure

```
portfolio-landing-page/
├── .github/
│   └── workflows/
│       └── deploy.yml   ← GitHub Actions workflow
├── index.html           ← Main page
├── assets/
│   ├── css/style.css    ← All styles
│   ├── js/main.js       ← Scroll animations & nav
│   └── img/
│       └── profile.jpeg ← Your profile photo (copy from CV/)
├── .gitignore
└── README.md
```

## ⚠️ Before pushing

Make sure to copy your profile photo:
```
Source:      CV\PerfilLinkedIn0126.jpeg
Destination: portfolio-landing-page\assets\img\profile.jpeg
```

---

## Local development

Open `index.html` directly in a browser, or use any static server:

```bash
npx serve .
```
