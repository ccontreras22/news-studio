# 🚀 Deployment Guide

## Quick Deploy Options

### Option 1: GitHub Pages (Free & Easy)

1. **Create a GitHub repository**
   - Go to https://github.com/new
   - Name it `spotify-news-studio`
   - Make it Public or Private (both work)

2. **Upload your files**
   ```bash
   cd /Users/ccontreras/spotify-workspace/news-studio
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/spotify-news-studio.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` → `/root`
   - Click Save

4. **Access your site**
   - URL will be: `https://YOUR-USERNAME.github.io/spotify-news-studio/`
   - Share this URL + PIN with your team

---

### Option 2: Netlify (Free, Drag & Drop)

1. **Go to Netlify**
   - Visit https://app.netlify.com/drop

2. **Drag the `news-studio` folder**
   - Just drag the entire folder into the browser
   - Wait for deployment (30 seconds)

3. **Get your URL**
   - You'll get a URL like: `https://random-name-123.netlify.app`
   - You can customize the name in Site Settings

4. **Share**
   - Share the URL + PIN (`1234` by default)

---

### Option 3: Vercel (Free)

1. **Install Vercel CLI** (optional)
   ```bash
   npm install -g vercel
   ```

2. **Deploy**
   ```bash
   cd /Users/ccontreras/spotify-workspace/news-studio
   vercel
   ```

3. **Or use the website**
   - Go to https://vercel.com/new
   - Import your GitHub repo or drag & drop

---

### Option 4: Internal Spotify Server

If you have access to an internal Spotify server:

1. Upload the entire `news-studio` folder
2. Make sure the folder structure stays intact:
   ```
   /your-server-path/news-studio/
   ├── index.html
   ├── fonts/
   └── README.md
   ```
3. Access via your internal URL

---

## 🔒 Security Checklist

Before deploying publicly:

- [x] PIN protection is enabled (default: `1234`)
- [ ] Change the default PIN to something secure
- [ ] Share the PIN only with authorized users
- [ ] Consider changing the PIN periodically
- [ ] For sensitive work, use server-side authentication instead

---

## 📝 Post-Deployment

1. **Test the deployment**
   - Open the URL in an incognito window
   - Try the PIN
   - Upload an image and create a design
   - Export a PNG

2. **Share with your team**
   - Send the URL
   - Send the PIN separately (email, Slack DM, etc.)
   - Include basic instructions

---

## 🎯 Custom Domain (Optional)

### GitHub Pages
- Settings → Pages → Custom domain
- Add your domain (e.g., `news-studio.yourcompany.com`)

### Netlify
- Domain settings → Add custom domain
- Update DNS records

### Vercel
- Project settings → Domains
- Add your domain

---

## 🔄 Updating After Deployment

### GitHub Pages
```bash
# Make your changes to index.html
git add .
git commit -m "Update design"
git push
# Wait 1-2 minutes for GitHub to rebuild
```

### Netlify
- Drag the updated folder again, or
- Connect to GitHub for auto-deploys

### Vercel
- Push to GitHub (if connected), or
- Run `vercel --prod` again

---

**Need help?** Check the main README.md for troubleshooting tips.
