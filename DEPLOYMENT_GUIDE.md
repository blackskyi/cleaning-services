# GitHub Pages Deployment Guide for Cleaning Services Site

## ✅ COMPLETED:
- Created new git repository
- Copied cleaning-services.html as index.html
- Made initial commit

---

## 📋 NEXT STEPS TO DEPLOY:

### **STEP 1: Create GitHub Repository**

1. Go to: https://github.com/new
2. **Repository name:** `cleaning-services` (or `ileana-cleaning`)
3. **Description:** "Professional cleaning and organizing services in Los Angeles"
4. **Visibility:** ✅ Public (required for free GitHub Pages)
5. **DO NOT** initialize with README, .gitignore, or license
6. Click **"Create repository"**

---

### **STEP 2: Push Your Code to GitHub**

After creating the repo, GitHub will show you commands. Run these in your terminal:

```bash
cd /Users/gokul/cleaning-site

# Add GitHub as remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/cleaning-services.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Example if your GitHub username is "blackskyi":**
```bash
git remote add origin https://github.com/blackskyi/cleaning-services.git
git branch -M main
git push -u origin main
```

---

### **STEP 3: Enable GitHub Pages**

1. Go to your repository on GitHub
2. Click **Settings** (top right)
3. Click **Pages** (left sidebar)
4. Under **"Source"**:
   - Branch: Select `main`
   - Folder: Select `/ (root)`
5. Click **Save**

**Wait 2-3 minutes**, then your site will be live at:
```
https://YOUR-USERNAME.github.io/cleaning-services/
```

---

### **STEP 4: Test Your Live Site**

Visit: `https://YOUR-USERNAME.github.io/cleaning-services/`

**Check:**
- ✅ Page loads correctly
- ✅ Stripe payment buttons work
- ✅ Phone number is clickable
- ✅ All images load
- ✅ Responsive on mobile

---

## 🌐 STEP 5: ADD CUSTOM DOMAIN (LATER)

Once you buy a domain (like **homecleaningorganizing.com**), you can connect it:

### **A. In Your Domain Registrar (Namecheap, GoDaddy, etc.):**

Add these DNS records:

**For root domain (homecleaningorganizing.com):**
```
Type: A
Host: @
Value: 185.199.108.153
TTL: Automatic

Type: A
Host: @
Value: 185.199.109.153
TTL: Automatic

Type: A
Host: @
Value: 185.199.110.153
TTL: Automatic

Type: A
Host: @
Value: 185.199.111.153
TTL: Automatic
```

**For www subdomain:**
```
Type: CNAME
Host: www
Value: YOUR-USERNAME.github.io
TTL: Automatic
```

### **B. In GitHub Pages Settings:**

1. Go to repository **Settings** > **Pages**
2. Under **"Custom domain"**, enter: `homecleaningorganizing.com`
3. Wait for DNS check (green checkmark)
4. ✅ Enable **"Enforce HTTPS"** (free SSL!)

**Your site will now be at:** `https://homecleaningorganizing.com`

---

## 🚀 QUICK UPDATES PROCESS

Whenever you want to update the website:

```bash
cd /Users/gokul/cleaning-site

# Make your changes to index.html

# Commit and push
git add .
git commit -m "Updated pricing/content"
git push

# Site updates automatically in 1-2 minutes!
```

---

## 📊 CURRENT STATUS

- ✅ Local git repo created: `/Users/gokul/cleaning-site/`
- ✅ index.html ready to deploy
- ⏳ Waiting for: GitHub repository creation
- ⏳ Waiting for: Push to GitHub
- ⏳ Waiting for: GitHub Pages enabled

---

## 💰 COST BREAKDOWN

**Current (Free hosting):**
- GitHub Pages: **$0/month**
- Custom domain (when ready): **~$12/year**
- SSL certificate: **$0** (automatic with GitHub Pages)

**Total: FREE until you add domain!**

---

## 🆘 NEED HELP?

If you get stuck:
1. Check GitHub repo was created successfully
2. Make sure repo is **Public** (not Private)
3. Wait 2-3 minutes after enabling Pages
4. Clear browser cache if site doesn't update

---

## 🎯 WHAT'S YOUR GITHUB USERNAME?

Tell me your GitHub username and I'll give you the exact commands to run!
