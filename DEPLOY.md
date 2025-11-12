# Deploy to GitHub Pages

Your website is ready to deploy! Everything is committed to git locally.

## Quick Deploy (2 steps)

### Step 1: Create GitHub Repository

Go to: https://github.com/new

- **Repository name**: `dissecting-transformers-clear` (or any name you prefer)
- **Visibility**: Public
- **DO NOT** check "Add a README file"
- Click **Create repository**

### Step 2: Push to GitHub

Run these commands in the terminal:

```bash
cd /home/shailender/Desktop/website_Iclr/research-paper-site

# If you used a different repository name, update it here:
git remote set-url origin https://github.com/ShailenderGoyal/YOUR-REPO-NAME.git

# Push to GitHub
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Source", select **main** branch
4. Click **Save**
5. Wait 1-2 minutes

Your website will be live at:
**https://ShailenderGoyal.github.io/dissecting-transformers-clear/**

---

## Alternative: One-Command Deploy

If you have GitHub CLI installed:

```bash
# Create repo and push
gh repo create dissecting-transformers-clear --public --source=. --remote=origin --push

# Enable GitHub Pages
gh repo edit --enable-pages --pages-branch=main
```

---

## What's Included

✅ Complete website with all sections
✅ 7 high-quality figures from LaTeX
✅ Paper PDF
✅ Professional styling
✅ Mobile-responsive design
✅ All content from your paper

## File Structure

```
research-paper-site/
├── index.html           # Main website
├── static/
│   ├── paper.pdf       # Your paper
│   ├── css/            # Styles
│   ├── js/             # Scripts
│   └── images/
│       └── figures/    # All 7 figures
└── README.md
```

## Customization After Deploy

To make changes:
1. Edit `index.html`
2. Commit: `git commit -am "Update content"`
3. Push: `git push`
4. Wait ~1 minute for GitHub Pages to rebuild

---

**Need help?** The repository is ready locally at:
`/home/shailender/Desktop/website_Iclr/research-paper-site/`
