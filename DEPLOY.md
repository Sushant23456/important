# Deploy Valentine to GitHub Pages

## 1. Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in.
2. Click **+** (top right) → **New repository**.
3. Name it (e.g. `valentine` or `valentine-page`).
4. Choose **Public**, leave "Add a README" unchecked.
5. Click **Create repository**.

## 2. Push your project to GitHub

In Terminal, run these from your **Valentine** folder:

```bash
cd "/Users/sushanttiwari/Documents/Local Apps/Valentine"

# Initialize git (if not already)
git init

# Add all files
git add index.html images/

# Commit
git commit -m "Valentine page"

# Add your GitHub repo as remote (replace YOUR_USERNAME and REPO_NAME with yours)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push (use main branch for GitHub Pages)
git branch -M main
git push -u origin main
```

Replace:
- **YOUR_USERNAME** = your GitHub username  
- **REPO_NAME** = the repo you created (e.g. `valentine`)

## 3. Turn on GitHub Pages

1. Open your repo on GitHub.
2. Go to **Settings** → **Pages** (left sidebar).
3. Under **Source**, choose **Deploy from a branch**.
4. Under **Branch**, pick **main** and **/ (root)**.
5. Click **Save**.

## 4. Open your site

After 1–2 minutes, your site will be at:

**https://YOUR_USERNAME.github.io/REPO_NAME/**

Example: if your username is `johndoe` and the repo is `valentine`:
**https://johndoe.github.io/valentine/**

---

### Notes

- Put your photos in the **images** folder (`us1.jpg`, `us2.jpg`, etc.) before pushing so they appear on the live site.
- To update the site later: edit files, then run `git add .`, `git commit -m "Update"`, `git push`.
