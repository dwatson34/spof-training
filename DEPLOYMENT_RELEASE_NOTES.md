# Deployment Guide

This guide walks you through deploying the SPOF Training Suite to GitHub Pages.

---

## Prerequisites

Before you start, you'll need:

1. A GitHub account (free at https://github.com)
2. Git installed on your computer
3. All 26 files ready to upload (HTML modules + documentation)
4. About 15 minutes

---

## Step 1: Create or Access Your GitHub Repository

### If You Already Have a Repository

1. Go to **github.com/your-username/spof-training**
2. Skip to Step 2

### If You Need to Create One

1. Go to **github.com/new**
2. Repository name: `spof-training`
3. Description: "Interactive training platform for Xuber SPOF"
4. Make it **Public**
5. Click **Create repository**

---

## Step 2: Upload Files to GitHub

You have two options: **Web Upload** (easiest) or **Git Command Line** (recommended).

### Option A: Web Upload (Easiest)

1. Go to your repository: **github.com/your-username/spof-training**
2. Click **Add file** → **Upload files**
3. Drag and drop all 26 files into the upload box
4. Scroll down and click **Commit changes**
5. Add message: "Add SPOF training suite v1.0"
6. Click **Commit**

The files are now uploaded!

### Option B: Git Command Line (For Teams)

Open your terminal and run:

```bash
git clone https://github.com/your-username/spof-training.git
cd spof-training
# Copy all 26 files into this folder
git add .
git commit -m "Add SPOF training suite v1.0"
git push origin main
```

---

## Step 3: Enable GitHub Pages

1. Go to your repository settings
2. Scroll to **Pages** section
3. Under "Source", select **main** branch
4. Select **/ (root)** folder
5. Click **Save**

GitHub will show: "Your site is ready to be published at `https://your-username.github.io/spof-training/`"

---

## Step 4: Verify Deployment

1. Wait 1-2 minutes for GitHub Pages to deploy
2. Visit: **https://your-username.github.io/spof-training/**
3. You should see the training portal with 4 tabs
4. Test by:
   - Clicking each tab
   - Browsing modules
   - Clicking "Launch Module" on one
   - Taking a quiz

---

## Step 5: Share the URL

Your training platform is now live! Share this URL:

```
https://your-username.github.io/spof-training/
```

Send it to your team via:
- Email
- Slack
- Internal documentation
- Team wiki

---

## Common Issues & Solutions

### Page Shows 404 Error

**Problem:** "File not found"

**Solution:**
1. Check that `index.html` is in the repository root
2. Make sure it's spelled exactly `index.html` (lowercase)
3. Wait another minute for GitHub Pages to deploy
4. Do a hard refresh (Ctrl+Shift+R or Cmd+Shift+R)

### Page Loads But Looks Wrong

**Problem:** Missing styles or modules not loading

**Solution:**
1. Open browser Developer Tools (F12)
2. Check the Console tab for errors
3. Make sure all HTML files are in the root (not in folders)
4. Do a hard refresh

### Modules Don't Launch

**Problem:** Clicking "Launch Module" doesn't open the training

**Solution:**
1. Check that module HTML files are in the repository root
2. Verify file names match exactly (e.g., `v2_XE_HTMLUI_Beginner_Training.html`)
3. Check the browser console for 404 errors
4. Try a different module

### Quiz Scores Not Saving

**Problem:** Quiz scores disappear after closing the browser

**Solution:**
- This is normal! Scores are saved in localStorage, which is per-browser/device
- Students' scores won't transfer between devices or browsers
- This is a privacy feature — no data is sent anywhere

---

## Updating Your Training Platform

### To Add a New Module

1. Create the new HTML file (copy from an existing module)
2. Upload to GitHub using web upload or git push
3. Update `portal.html` to include the new module in the modules object
4. Commit and push
5. GitHub Pages automatically updates (1-2 minute delay)

### To Update Documentation

1. Edit the `.md` file directly on GitHub
2. Click the pencil icon (Edit)
3. Make changes
4. Scroll down and click **Commit changes**
5. Changes appear immediately

### To Fix a Bug or Typo

1. Navigate to the file on GitHub
2. Click the pencil icon (Edit)
3. Make the fix
4. Commit with message: "Fix: [description]"
5. Changes deploy in 1-2 minutes

---

## Rollback (Undo Changes)

If you make a mistake and want to undo:

1. Go to your repository
2. Click **Commits** (top area)
3. Find the commit before your mistake
4. Click the **<>** icon to view that version
5. Click **Browse files** to see what it looked like
6. If you want to revert, open a new commit reverting the changes

Or ask GitHub to recover a deleted file:

1. Go to **<> Code** tab
2. Click on the file path where the deleted file was
3. GitHub shows a "This file has been deleted" message
4. Click to restore it

---

## Performance & Scaling

### How Many Users Can It Handle?

GitHub Pages can handle **millions of requests per month** for static files. The SPOF training platform has **zero database**, so there's no bottleneck. You can share it with your entire organization without worrying about capacity.

### Does It Cost Anything?

No! GitHub Pages hosting is **completely free**. There are no bandwidth charges, no storage limits (up to 1GB per repo), and no per-user costs.

### How Do I See Usage Stats?

1. Go to your repository
2. Click **Insights** → **Traffic**
3. See how many people visited and where they came from

---

## Monitoring & Maintenance

### Weekly Checklist

- [ ] Check that the portal loads without errors
- [ ] Test one module end-to-end
- [ ] Verify quiz scoring works
- [ ] Check GitHub Insights for usage

### Monthly Tasks

- [ ] Review GitHub Issues for bugs or feedback
- [ ] Update documentation if needed
- [ ] Add new modules if available

---

## Disaster Recovery

If something goes catastrophically wrong:

1. **Revert to a known good commit:**
   - Go to **Commits**
   - Find the last good version
   - Revert the commits that broke things

2. **Restore from backup:**
   - Your repository is automatically backed up by GitHub
   - You can restore any previous version

3. **Start fresh:**
   - Delete the repository
   - Create a new one
   - Re-upload all files
   - Takes about 5 minutes

---

## Best Practices

1. **Test locally first** — Open HTML files in your browser before uploading
2. **Use meaningful commit messages** — Makes it easy to find changes later
3. **Keep backup copies** — Store files locally as well as on GitHub
4. **Version your releases** — Tag major updates (v1.0, v1.1, etc.)
5. **Monitor feedback** — Check GitHub Issues regularly

---

## Support

If you run into issues:

1. **Check the documentation** — Start here
2. **Search GitHub Issues** — Your problem might already be solved
3. **Open a new issue** — Describe what's broken and what you expected
4. **Check GitHub Status** — https://www.githubstatus.com/

---

## Next Steps

1. ✅ Upload files to GitHub
2. ✅ Enable GitHub Pages
3. ✅ Test the platform
4. ✅ Share the URL with your team
5. ✅ Monitor usage and gather feedback
6. Add new modules and update documentation as needed

---

**Last Updated:** October 2026  
**Questions?** Check the README or open an issue on GitHub
