# FoodHub - Netlify Deployment Guide

## Issue: Wrong Domain Name in Notifications

If you're seeing notifications that say "spice-and-soul-restaurant.netlify.app says..." instead of "FoodHub..." or "deliveryfoodhub...", this is because your Netlify site is currently deployed under the wrong subdomain.

---

## Solution

### **Option 1: Change Netlify Site Name** (Recommended)

1. Go to [Netlify Dashboard](https://app.netlify.com)
2. Select your site
3. Click **Site Settings** → **General** → **Site Details**
4. Click **Change site name**
5. Change from `spice-and-soul-restaurant` to `deliveryfoodhub`
6. Save changes

**New URL will be:** `https://deliveryfoodhub.netlify.app`

---

### **Option 2: Use Custom Domain**

1. In Netlify Dashboard, go to **Domain Settings**
2. Click **Add domain alias** or **Set up a custom domain**
3. Add your custom domain (e.g., `foodhub.com` or `deliveryfoodhub.com`)
4. Follow Netlify's instructions to configure DNS records
5. Once set up, all notifications will show your custom domain

---

## Browser Notification Display

When you click "Add to Cart" or perform other actions, the browser displays a notification. The domain shown in this notification is:

- The current website's domain/URL
- Automatically added by the browser for security purposes
- Cannot be changed via code

So fixing the Netlify site name will automatically fix the domain shown in notifications.

---

## Verification After Fix

After changing the domain, you should see:

- Notifications saying "**FoodHub**" or "**deliveryfoodhub**" instead of "spice-and-soul-restaurant"
- All browser tabs showing the new correct domain
- Updated URL in the address bar

---

## Need Help?

Refer to official Netlify documentation:

- [Change site name](https://docs.netlify.com/site-management/settings/#general)
- [Custom domains](https://docs.netlify.com/domains-https/custom-domains/configure-external-dns/)
