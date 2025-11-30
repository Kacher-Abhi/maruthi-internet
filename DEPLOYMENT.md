# Deploying to Render

This guide will help you deploy your Maruthi Internet website to Render.

## Option 1: Deploy via Render Dashboard (Recommended)

### Step 1: Push to GitHub

1. Create a new repository on GitHub (if you haven't already)
2. Initialize git in your project folder:
   ```bash
   cd /Users/abhishekbkacher/Desktop/Maruthi-website
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

### Step 2: Connect to Render

1. Go to [Render Dashboard](https://dashboard.render.com/)
2. Sign up or log in to your Render account
3. Click **"New +"** button
4. Select **"Static Site"**

### Step 3: Configure Deployment

1. **Connect Repository:**
   - Connect your GitHub account
   - Select the repository you just created

2. **Configure Build Settings:**
   - **Name:** `maruthi-internet` (or any name you prefer)
   - **Branch:** `main` (or `master`)
   - **Root Directory:** Leave empty (or `.` if needed)
   - **Build Command:** Leave empty (no build needed for static site)
   - **Publish Directory:** Leave empty (or `.`)

3. **Click "Create Static Site"**

### Step 4: Wait for Deployment

- Render will automatically deploy your site
- You'll get a URL like: `https://maruthi-internet.onrender.com`
- The site will auto-deploy on every push to your main branch

## Option 2: Deploy via Render CLI

1. Install Render CLI:
   ```bash
   npm install -g render-cli
   ```

2. Login to Render:
   ```bash
   render login
   ```

3. Deploy:
   ```bash
   render deploy
   ```

## Custom Domain (Optional)

1. In your Render dashboard, go to your static site
2. Click on **"Settings"**
3. Scroll to **"Custom Domains"**
4. Add your domain (e.g., `maruthiinternet.com`)
5. Follow the DNS configuration instructions

## Environment Variables (if needed later)

If you need to add environment variables:
1. Go to your site settings in Render
2. Click on **"Environment"**
3. Add your variables

## Important Notes

- **Free Tier:** Render offers a free tier for static sites
- **Auto-Deploy:** Every push to your main branch will trigger a new deployment
- **HTTPS:** Your site will automatically have HTTPS enabled
- **Build Time:** Static sites deploy very quickly (usually under 1 minute)

## Troubleshooting

### If deployment fails:
1. Check that all files are committed to git
2. Ensure `index.html` is in the root directory
3. Check the build logs in Render dashboard

### If pages don't load:
- Make sure all file paths are relative (they already are)
- Check that CSS and JS files are in the same directory as HTML files

## Quick Deploy Checklist

- [ ] Code pushed to GitHub
- [ ] Render account created
- [ ] Static site created in Render
- [ ] Repository connected
- [ ] Deployment successful
- [ ] Site accessible via Render URL

---

**Your site will be live at:** `https://YOUR-SITE-NAME.onrender.com`

