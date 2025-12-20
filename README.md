# jeremysatre.com Website

Your personal brand website as founder of ZeroDrama.ai — hosted for **free** on GitHub Pages.

This site positions you as an organizational change management expert and drives traffic to ZeroDrama.ai. It uses your brand colors (Steel Blue, Lime Green, Coral Orange, Navy).

---

## Setup Instructions

### Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com) and sign up (it's free)

### Step 2: Create a New Repository
1. Click the **+** icon in the top right → **New repository**
2. Name it: `jeremysatre.com` (or any name you prefer)
3. Make sure it's set to **Public**
4. Check **"Add a README file"**
5. Click **Create repository**

### Step 3: Upload Your Website Files
1. In your new repository, click **Add file** → **Upload files**
2. Drag and drop the `index.html` file
3. Click **Commit changes**

### Step 4: Enable GitHub Pages
1. Go to your repository's **Settings** tab
2. In the left sidebar, click **Pages**
3. Under "Source", select **Deploy from a branch**
4. Under "Branch", select **main** and **/ (root)**
5. Click **Save**
6. Wait a few minutes — your site will be live at `https://yourusername.github.io/jeremysatre.com`

### Step 5: Add Your Custom Domain
1. Still in **Settings → Pages**, under "Custom domain"
2. Enter: `jeremysatre.com`
3. Click **Save**
4. Check **"Enforce HTTPS"** (may take a few minutes to become available)

### Step 6: Configure DNS in Squarespace
1. Log in to your Squarespace account
2. Go to **Settings** → **Domains** → **jeremysatre.com** → **DNS Settings**
3. **Delete** any existing A records and CNAME records for @ and www
4. **Add these A records** (all for the @ host):
   ```
   Type: A    Host: @    Points to: 185.199.108.153
   Type: A    Host: @    Points to: 185.199.109.153
   Type: A    Host: @    Points to: 185.199.110.153
   Type: A    Host: @    Points to: 185.199.111.153
   ```
5. **Add this CNAME record** for www:
   ```
   Type: CNAME    Host: www    Points to: yourusername.github.io
   ```
   (Replace `yourusername` with your actual GitHub username)

6. DNS changes can take **up to 48 hours** to propagate (usually much faster)

---

## Customizing Your Website

Edit the `index.html` file directly on GitHub:
1. Click on `index.html` in your repository
2. Click the **pencil icon** (Edit this file)
3. Make your changes
4. Click **Commit changes**

### What to Customize:

**Tagline** (line ~115):
```html
<p class="tagline">Your tagline or profession goes here</p>
```

**Bio** (line ~116-120):
```html
<p class="bio">
    Your introduction text here...
</p>
```

**Links** (line ~122-127):
```html
<a href="mailto:your@email.com">Email</a>
<a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
```

**Colors** (in the `:root` section near the top):
- `--color-bg`: Background color
- `--color-text`: Main text color
- `--color-accent`: Accent color (divider line, hover states)

---

## Cost Breakdown

| Item | Cost |
|------|------|
| GitHub Pages Hosting | **Free** |
| Domain (already owned at Squarespace) | Your existing cost |
| SSL Certificate | **Free** (via GitHub) |
| **Total Additional Cost** | **$0** |

---

## Maintenance Required

- **Almost none!** The site is pure HTML/CSS with no dependencies
- Update content by editing the HTML file when needed
- No security updates, no plugins, no databases

---

## Alternative: Keep Domain at Squarespace, Point Elsewhere

If you'd rather not deal with DNS, you can also:
1. Transfer the domain to a registrar like Cloudflare (~$10/year, at cost)
2. Cloudflare makes DNS management easier and adds free CDN/security

But the instructions above work perfectly fine with Squarespace!
