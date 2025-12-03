# 🚀 Setup Guide — Deploy to GitHub Pages

Follow these steps to deploy the landing page to your own GitHub Pages site.

---

## Step 1: Create a New GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `radiology-ai-landing` (or your preferred name)
3. **Important:** Select **Public** (required for free GitHub Pages)
4. Do NOT initialize with README (we'll push our own)
5. Click **Create repository**

---

## Step 2: Push This Code to Your New Repo

Open terminal in this folder and run:

```bash
# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: AI Radiology Assistant landing page"

# Add your remote (replace with your repo URL)
git remote add origin https://github.com/kazdatahelp/radiology-ai-landing.git

# Push to main branch
git push -u origin main
```

---

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (tab at the top)
3. Click **Pages** (left sidebar)
4. Under "Build and deployment":
   - **Source:** Select **GitHub Actions**
5. The workflow will run automatically

---

## Step 4: Wait for Deployment

1. Go to **Actions** tab in your repository
2. You should see "Deploy to GitHub Pages" workflow running
3. Wait for it to complete (green checkmark)
4. Usually takes 1-2 minutes

---

## Step 5: Access Your Site

Your site will be live at:

```
https://kazdatahelp.github.io/radiology-ai-landing/
```

Replace `kazdatahelp` and `radiology-ai-landing` with your GitHub username and repo name.

---

## Optional: Custom Domain

To use a custom domain like `radiology-ai.kz`:

### A. Configure GitHub

1. Rename `CNAME.template` to `CNAME`
2. Replace contents with your domain:
   ```
   radiology-ai.kz
   ```
3. Commit and push

### B. Configure DNS

Add these DNS records with your domain registrar:

**For apex domain (radiology-ai.kz):**
| Type | Name | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |

**For www subdomain:**
| Type | Name | Value |
|------|------|-------|
| CNAME | www | kazdatahelp.github.io |

### C. Enable HTTPS

1. Go to **Settings** → **Pages**
2. Check **Enforce HTTPS**
3. Wait for certificate (can take up to 24 hours)

---

## Troubleshooting

### Page shows 404

- Make sure the repository is **public**
- Check that `index.html` exists in the root
- Wait a few minutes after deployment

### Workflow failed

- Check the **Actions** tab for error details
- Ensure all files are committed and pushed

### Changes not showing

- Hard refresh: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)
- Check that the latest workflow completed successfully

---

## Making Updates

1. Edit `index.html` locally
2. Commit and push:
   ```bash
   git add .
   git commit -m "Update landing page content"
   git push
   ```
3. GitHub Actions will auto-deploy (1-2 minutes)

---

## Quick Commands Reference

```bash
# Clone (if starting fresh)
git clone https://github.com/kazdatahelp/radiology-ai-landing.git
cd radiology-ai-landing

# Make changes, then deploy
git add .
git commit -m "Your commit message"
git push

# Check deployment status
# Go to: https://github.com/kazdatahelp/radiology-ai-landing/actions
```

---

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Custom Domain Setup](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
