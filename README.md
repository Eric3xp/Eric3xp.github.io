# 🎨 Graphic Designer Portfolio Website

A dark, editorial portfolio website for graphic designers — built with pure HTML, CSS & JavaScript. No frameworks, no dependencies (except Google Fonts).

## 📁 File Structure

```
portfolio/
├── index.html      ← Main HTML file
├── style.css       ← All styles
├── main.js         ← Animations & interactivity
└── README.md       ← This file
```

## 🚀 How to Host on GitHub Pages

### Step 1 — Set up Git & create the repo
1. Open the project folder in **VS Code**
2. Open the terminal (`Ctrl + `` ` ``)
3. Run the following commands:

```bash
git init
git add .
git commit -m "Initial commit: portfolio website"
```

### Step 2 — Create a GitHub repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **+** button → **New repository**
3. Name it: `portfolio` (or `yourusername.github.io` for a personal domain)
4. Leave it **Public**
5. Do **NOT** check "Add README" (you already have files)
6. Click **Create repository**

### Step 3 — Push your code to GitHub
GitHub will show you commands. Run these in VS Code terminal:

```bash
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
git branch -M main
git push -u origin main
```

### Step 4 — Enable GitHub Pages
1. On your GitHub repo page, click **Settings**
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Choose **main** branch → **/ (root)** folder
5. Click **Save**

Your site will be live in ~1 minute at:
**`https://YOUR_USERNAME.github.io/portfolio/`**

> If you named the repo `yourusername.github.io`, it will be at `https://yourusername.github.io`

---

## ✏️ How to Customize

| What to change | Where |
|---|---|
| Your name | `index.html` → hero section & about initials |
| Job title | `index.html` → `.hero-tag` |
| Bio text | `index.html` → about section |
| Projects | `index.html` → `.projects-grid` cards |
| Email | `index.html` → `.contact-email` |
| Social links | `index.html` → `.contact-socials` |
| Color accent | `style.css` → `--accent` variable |
| Background | `style.css` → `--bg` variable |
| Profile photo | Replace `.about-img-placeholder` with `<img src="photo.jpg" alt="Your Name">` |

## 🖼️ Adding a Real Profile Photo
Replace this in `index.html`:
```html
<div class="about-img-placeholder">
  <span class="about-initials">AK</span>
</div>
```
With:
```html
<img src="images/photo.jpg" alt="Your Name" class="about-photo">
```
And add in `style.css`:
```css
.about-photo {
  width: 240px;
  height: 300px;
  object-fit: cover;
  border-radius: 12px;
  border: 1px solid var(--border);
}
```

## ✅ Live Preview in VS Code
Install the **Live Server** extension → right-click `index.html` → **Open with Live Server**
