# 🌐 Custom Domain Setup Guide - bullgym19.com

## Overview
This guide will help you connect your Cloudflare domain **bullgym19.com** to your GitHub Pages website.

---

## 📋 Prerequisites
✅ Domain purchased: bullgym19.com (Cloudflare)
✅ GitHub repository: https://github.com/mahindra27/BullGym19
✅ CNAME file created in repository

---

## 🔧 STEP 1: Configure DNS in Cloudflare

### A. Login to Cloudflare Dashboard
1. Go to https://dash.cloudflare.com
2. Select your domain: **bullgym19.com**
3. Go to **DNS** → **Records**

### B. Add DNS Records

**Delete any existing A or CNAME records for @ and www, then add these:**

#### For Apex Domain (@) - Add 4 A Records:
```
Type: A
Name: @
IPv4 address: 185.199.108.153
TTL: Auto
Proxy status: DNS only (gray cloud)

Type: A
Name: @
IPv4 address: 185.199.109.153
TTL: Auto
Proxy status: DNS only (gray cloud)

Type: A
Name: @
IPv4 address: 185.199.110.153
TTL: Auto
Proxy status: DNS only (gray cloud)

Type: A
Name: @
IPv4 address: 185.199.111.153
TTL: Auto
Proxy status: DNS only (gray cloud)
```

#### For WWW Subdomain - Add 1 CNAME Record:
```
Type: CNAME
Name: www
Target: mahindra27.github.io
TTL: Auto
Proxy status: DNS only (gray cloud)
```

### C. Important DNS Settings
- **Proxy status:** Set to **DNS only** (gray cloud icon) for all records
- **SSL/TLS Mode:** Go to SSL/TLS → Overview → Set to **Full** or **Full (strict)**

---

## 🔧 STEP 2: Configure GitHub Pages

### A. Enable GitHub Pages
1. Go to: https://github.com/mahindra27/BullGym19/settings/pages
2. Under **Source**:
   - Branch: `main`
   - Folder: `/ (root)`
3. Click **Save**

### B. Add Custom Domain
1. In the same GitHub Pages settings
2. Under **Custom domain**, enter: `bullgym19.com`
3. Click **Save**
4. Wait for DNS check (may take a few minutes)
5. Once verified, check ✅ **Enforce HTTPS** (this enables SSL certificate)

---

## ⏱️ STEP 3: Wait for DNS Propagation

DNS changes can take:
- **Minimum:** 5-10 minutes
- **Maximum:** 24-48 hours (rare)
- **Typical:** 1-2 hours

### Check DNS Propagation:
- Visit: https://dnschecker.org
- Enter: `bullgym19.com`
- Check if A records point to GitHub's IPs

---

## ✅ STEP 4: Verify Your Website

After DNS propagation, test these URLs:

1. **http://bullgym19.com** (should redirect to https)
2. **https://bullgym19.com** (your main site)
3. **https://www.bullgym19.com** (should work)
4. **https://mahindra27.github.io/BullGym19** (should redirect to your custom domain)

---

## 🔒 SSL Certificate (HTTPS)

GitHub automatically provides a **free SSL certificate** via Let's Encrypt:
- ✅ No cost
- ✅ Auto-renewal every 90 days
- ✅ Enabled when you check "Enforce HTTPS"

**Important:** Wait 15-30 minutes after adding custom domain before enabling HTTPS.

---

## 🐛 Troubleshooting

### Issue 1: "DNS check failed"
**Solution:**
- Verify A records point to correct GitHub IPs
- Ensure proxy is **disabled** (gray cloud) in Cloudflare
- Wait 10-15 minutes and try again

### Issue 2: "Certificate not issued"
**Solution:**
- Uncheck "Enforce HTTPS"
- Remove custom domain, save
- Re-add custom domain, save
- Wait 10 minutes
- Enable "Enforce HTTPS" again

### Issue 3: "404 Not Found"
**Solution:**
- Check CNAME file exists in repository root
- Verify it contains only: `bullgym19.com`
- Push changes to GitHub

### Issue 4: "Too many redirects"
**Solution:**
- In Cloudflare: SSL/TLS → Overview
- Set mode to **Full** (not Flexible)

---

## 📊 Quick Reference

### GitHub Pages IPs (for A records):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

### Cloudflare DNS Summary:
| Type  | Name | Value/Target          | Proxy |
|-------|------|-----------------------|-------|
| A     | @    | 185.199.108.153       | ❌    |
| A     | @    | 185.199.109.153       | ❌    |
| A     | @    | 185.199.110.153       | ❌    |
| A     | @    | 185.199.111.153       | ❌    |
| CNAME | www  | mahindra27.github.io  | ❌    |

---

## 🎯 Expected Timeline

| Time      | Status                                    |
|-----------|-------------------------------------------|
| 0 min     | DNS records added in Cloudflare           |
| 5 min     | DNS propagation starts                    |
| 15 min    | Custom domain added in GitHub             |
| 30 min    | DNS fully propagated                      |
| 45 min    | SSL certificate issued                    |
| 60 min    | ✅ Website live at https://bullgym19.com  |

---

## 🔄 Future Updates

When you update your website:
```bash
git add .
git commit -m "Updated content"
git push
```
Changes appear at **bullgym19.com** within 1-2 minutes!

---

## 📱 After Going Live

1. **Update Social Media:**
   - Instagram bio: bullgym19.com
   - TikTok profile
   - Google Business Profile

2. **Update Marketing Materials:**
   - Business cards
   - Flyers
   - WhatsApp status

3. **SEO:**
   - Submit to Google Search Console
   - Add to Google My Business
   - Share on social media

---

## 🆘 Need Help?

### Cloudflare Support:
- Dashboard: https://dash.cloudflare.com
- Community: https://community.cloudflare.com

### GitHub Pages Docs:
- Custom Domains: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

### Developer Contact:
- **Mahindra Prasad**
- GitHub: @mahindra27
- LinkedIn: linkedin.com/in/mahindra-prasad-4b32b02ba

---

**🎉 Once complete, your website will be live at:**
# https://bullgym19.com 🚀

**Professional, fast, and secure!** 💪🔥
