# Host Your Ladakh Marathon Tracker on GitHub Pages

Follow these steps to host your marathon tracker for free on GitHub Pages.

---

## Step 1: Create a New Repository on GitHub

1. Go to **https://github.com/new**
2. Fill in:
   - **Repository name:** `ladakh-marathon-tracker` (or any name you prefer)
   - **Description:** Ladakh 3:45 Marathon Training Plan Tracker
   - **Visibility:** Public
   - **Do NOT** initialize with README (we already have files)
3. Click **Create repository**

---

## Step 2: Push Your Files to GitHub

Open Terminal and run these commands (replace `YOUR_USERNAME` with your GitHub username):

```bash
cd /Users/jayantwaldia/ladakh-marathon-tracker

# Initialize git
git init

# Add all files
git add index.html README.md

# Commit
git commit -m "Add Ladakh Marathon training tracker"

# Add your GitHub repo as remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/ladakh-marathon-tracker.git

# Push to GitHub (use main branch)
git branch -M main
git push -u origin main
```

When prompted, enter your GitHub username and password (or use a Personal Access Token if you have 2FA enabled).

---

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/YOUR_USERNAME/ladakh-marathon-tracker`
2. Click **Settings** (top menu)
3. In the left sidebar, click **Pages** (under "Code and automation")
4. Under **Source**, select **Deploy from a branch**
5. Under **Branch**, select `main` and `/ (root)`
6. Click **Save**

---

## Step 4: Access Your Live Site

After 1–2 minutes, your site will be live at:

**https://YOUR_USERNAME.github.io/ladakh-marathon-tracker/**

Example: If your username is `jayantwaldia`, your URL would be:
**https://jayantwaldia.github.io/ladakh-marathon-tracker/**

---

## Notes

- **Progress is saved locally** — The tracker uses `localStorage`, so each visitor's workout data stays in their browser. It won't sync across devices.
- **Updates** — To update the site, edit files, then run:
  ```bash
  git add .
  git commit -m "Update tracker"
  git push
  ```
- **Custom domain** — You can add a custom domain in the Pages settings if you have one.
