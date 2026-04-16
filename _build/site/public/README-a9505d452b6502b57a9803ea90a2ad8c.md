# Academic Website — MyST Markdown + GitHub Pages

A personal academic website built with [MyST Markdown](https://mystmd.org) and deployed via GitHub Pages.

## 🗂 File Structure

```
├── myst.yml              # Site configuration & table of contents
├── index.md              # Home page (bio, news)
├── research.md           # Research, projects and publications
├── assets/
│   ├── profile.jpg       # Your profile photo
│   └── cv.pdf            # Your CV PDF
└── .github/
    └── workflows/
        └── deploy.yml    # Auto-deploy to GitHub Pages
```

## 🚀 Getting Started

### 1. Personalize the content

Replace all placeholder text (name, email, institution, papers, etc.) in each `.md` file.
Add your photo as `assets/profile.jpg` and your CV PDF as `assets/cv.pdf`.

### 2. Update `myst.yml`

Edit the `title`, `authors`, `github`, and `nav` fields to match your info.

### 3. Preview locally

```bash
npm install -g mystmd
myst start
```

Open [http://localhost:3000](http://localhost:3000) to see your site.

### 4. Deploy to GitHub

1. Create a new GitHub repository named `yourusername.github.io`
2. Push this folder to it:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git remote add origin https://github.com/yourusername/yourusername.github.io
   git push -u origin main
   ```
3. Go to **Settings → Pages** in your repo and set Source to **GitHub Actions**
4. Your site will be live at `https://yourusername.github.io` after the first push!

## ✏️ Updating your site

Edit any `.md` file, commit, and push — GitHub Actions will rebuild and redeploy automatically.

## 📚 Resources

- [MyST Markdown docs](https://mystmd.org/guide)
- [MyST GitHub Pages deployment guide](https://mystmd.org/guide/deployment-github-pages)
- [MyST directives reference](https://mystmd.org/guide/directives)
