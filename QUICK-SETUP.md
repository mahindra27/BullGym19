# ✅ QUICK SETUP CHECKLIST - bullgym19.com

## 🎯 Goal
Connect your custom domain **bullgym19.com** to your Bull Gym website

---

## 📋 STEP-BY-STEP CHECKLIST

### ✅ PART 1: CLOUDFLARE DNS SETUP (Do this FIRST)

1. **[ ] Login to Cloudflare**
   - Go to: https://dash.cloudflare.com
   - Select domain: **bullgym19.com**

2. **[ ] Go to DNS Settings**
   - Click **DNS** in the left menu
   - Click **Records**

3. **[ ] Delete old records** (if any)
   - Remove any existing A or CNAME records for @ or www

4. **[ ] Add 4 A Records** (for apex domain)

   **Record 1:**
   - Type: `A`
   - Name: `@`
   - IPv4 address: `185.199.108.153`
   - Proxy: **DNS only** (gray cloud ⛅)

   **Record 2:**
   - Type: `A`
   - Name: `@`
   - IPv4 address: `185.199.109.153`
   - Proxy: **DNS only** (gray cloud ⛅)

   **Record 3:**
   - Type: `A`
   - Name: `@`
   - IPv4 address: `185.199.110.153`
   - Proxy: **DNS only** (gray cloud ⛅)

   **Record 4:**
   - Type: `A`
   - Name: `@`
   - IPv4 address: `185.199.111.153`
   - Proxy: **DNS only** (gray cloud ⛅)

5. **[ ] Add 1 CNAME Record** (for www subdomain)
   - Type: `CNAME`
   - Name: `www`
   - Target: `mahindra27.github.io`
   - Proxy: **DNS only** (gray cloud ⛅)

6. **[ ] Set SSL/TLS Mode**
   - Go to **SSL/TLS** → **Overview**
   - Set to: **Full** (not Flexible, not Full strict)
   - Click Save

---

### ✅ PART 2: GITHUB PAGES SETUP (Do this AFTER Cloudflare DNS)

7. **[ ] Enable GitHub Pages**
   - Go to: https://github.com/mahindra27/BullGym19/settings/pages
   - Under **Source**:
     - Branch: `main`
     - Folder: `/ (root)`
   - Click **Save**

8. **[ ] Add Custom Domain**
   - In the same GitHub Pages settings
   - Scroll to **Custom domain** section
   - Enter: `bullgym19.com`
   - Click **Save**
   - ⏱️ Wait for "DNS check successful" (may take 5-15 minutes)

9. **[ ] Wait for DNS Propagation**
   - ⏱️ Wait 15-30 minutes
   - Check status at: https://dnschecker.org (enter: bullgym19.com)

10. **[ ] Enable HTTPS**
    - After DNS check passes
    - Check ✅ **Enforce HTTPS**
    - ⏱️ Wait 10-15 minutes for SSL certificate

---

### ✅ PART 3: VERIFY YOUR WEBSITE IS LIVE

11. **[ ] Test Your URLs**
    - Visit: http://bullgym19.com (should redirect to https)
    - Visit: https://bullgym19.com (your website!)
    - Visit: https://www.bullgym19.com (should work)

12. **[ ] Check SSL Certificate**
    - Click padlock 🔒 in browser address bar
    - Should show "Connection is secure"

---

## 🎉 SUCCESS CRITERIA

✅ https://bullgym19.com shows your Bull Gym website
✅ Green padlock 🔒 appears in browser
✅ www.bullgym19.com also works
✅ No security warnings

---

## ⏱️ TIMELINE

| Time    | What to Do                           |
|---------|--------------------------------------|
| 0 min   | Add DNS records in Cloudflare        |
| 5 min   | Add custom domain in GitHub          |
| 15 min  | Wait for DNS propagation             |
| 30 min  | Enable HTTPS in GitHub               |
| 45 min  | ✅ Website live at bullgym19.com!    |

---

## 🆘 TROUBLESHOOTING

### Problem: "DNS check failed" in GitHub
**Solution:**
- Double-check all 4 A records are correct
- Ensure Cloudflare proxy is **OFF** (gray cloud)
- Wait another 10 minutes and try again

### Problem: "Enforce HTTPS" is grayed out
**Solution:**
- DNS check must pass first
- Wait 15-30 minutes after adding custom domain
- Try removing and re-adding custom domain

### Problem: Website shows 404
**Solution:**
- Check CNAME file exists in GitHub repo
- File should contain only: `bullgym19.com`
- No extra lines or spaces

---

## 📞 NEED HELP?

Check the complete guide: **CUSTOM-DOMAIN-SETUP.md**

**Mahindra Prasad**
- GitHub: @mahindra27
- LinkedIn: linkedin.com/in/mahindra-prasad-4b32b02ba

---

## 📱 AFTER GOING LIVE

**Update these places with your new URL:**
- [ ] Instagram bio: bullgym19.com
- [ ] TikTok profile
- [ ] Google Business Profile
- [ ] WhatsApp status
- [ ] Business cards
- [ ] Flyers and posters

---

**🚀 Your website will be live at: https://bullgym19.com**

**Let's make Bull Gym's online presence as strong as its members!** 💪🔥
