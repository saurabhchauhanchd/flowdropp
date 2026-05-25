# FlowDrop: Git + Auto-Deploy Setup Guide

## Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. **Repository name:** `flowdrop` (or whatever you want)
3. **Description:** Free automation workflow ideas library
4. **Public** (so people can discover it)
5. Click **Create repository**

## Step 2: Push Your Files to GitHub

Run these commands from your terminal:

```bash
# Navigate to your project folder (or create a new one)
mkdir flowdrop
cd flowdrop

# Download or copy these files into the folder:
# - index.html
# - README.md
# - netlify.toml
# - package.json
# - .gitignore

# Initialize git and push
git init
git add .
git commit -m "Initial FlowDrop deployment"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/flowdrop.git
git push -u origin main
```

**Replace `YOUR-USERNAME` with your actual GitHub username.**

## Step 3: Connect to Netlify with Auto-Deploy

1. Go to [app.netlify.com](https://app.netlify.com)
2. Click **"New site from Git"**
3. Select **GitHub** → authorize if needed
4. Search for your `flowdrop` repository and select it
5. **Build settings:**
   - Build command: *(leave empty)*
   - Publish directory: `.` (or just blank)
6. Click **Deploy site**

**That's it!** 🎉

## Step 4: Your Site is Live

Netlify will give you a live URL like: `https://flowdrop-abc123.netlify.app`

You can:
- **Customize the domain** (Settings → Domain management)
- **Set a custom domain** you own

## Step 5: Auto-Deploy on Every Push

Now, every time you push to GitHub:

```bash
# Make changes to index.html
git add index.html
git commit -m "Added 10 new workflows"
git push
```

Netlify automatically:
1. Detects the push
2. Rebuilds your site
3. Deploys the new version
4. Your live site updates in ~30 seconds

No manual deployment needed ever again.

## Step 6: Manage Your Site

In Netlify dashboard, you can:
- View deployment history
- Rollback to previous versions
- Set up environment variables
- Add custom headers/redirects
- Enable analytics
- Set up a custom domain

---

## Troubleshooting

**"Repository not found"**
- Make sure you're logged into the right GitHub account
- Check that the repo exists and is public

**"Deploy failed"**
- Check Netlify deploy logs (Deployments → Failed deployment → Logs)
- Make sure `index.html` is in the root of your repo

**"My changes aren't showing"**
- Wait 30-60 seconds for the deployment to finish
- Do a hard refresh in your browser (Ctrl+Shift+R on Windows, Cmd+Shift+R on Mac)
- Check the Netlify deployment log to confirm it succeeded

---

## Next Steps

1. ✅ Create GitHub repo
2. ✅ Push files
3. ✅ Connect to Netlify
4. 📝 Add a custom domain (optional)
5. 🤖 Build AI workflow generator feature (optional)
6. 📧 Set up newsletter signup (optional)

---

**Your FlowDrop site will be live and auto-deploying in < 5 minutes!**
