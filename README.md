# Dr. Sudaroli Dhananjeyan — Academic Profile Website

Personal academic website built for GitHub Pages.

**Live at:** `https://sudaroli1.github.io` (after deployment)

---

## Files

```
├── index.html      ← Main profile page
├── cv.html         ← Full CV page
├── style.css       ← All styles
├── script.js       ← Scroll animations
└── README.md       ← This file
```

---

## How to Deploy (Step-by-Step)

### Step 1 — Create a GitHub account
Go to [github.com](https://github.com) and sign up if you don't have an account.

### Step 2 — Create a new repository
1. Click the **+** icon → **New repository**
2. Name it exactly: `sudaroli1.github.io`  
   *(replace `sudaroli1` with your actual GitHub username)*
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload the files
**Option A (easy — browser upload):**
1. In your new repository, click **Add file → Upload files**
2. Drag and drop all 5 files: `index.html`, `cv.html`, `style.css`, `script.js`, `README.md`
3. Click **Commit changes**

**Option B (using Git):**
```bash
git clone https://github.com/sudaroli1/sudaroli1.github.io
cd sudaroli1.github.io
# Copy all files here
git add .
git commit -m "Initial site"
git push
```

### Step 4 — Enable GitHub Pages
1. Go to your repository → **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose **main** branch, **/ (root)** folder
4. Click **Save**

### Step 5 — Wait ~2 minutes
Your site will be live at: `https://sudaroli1.github.io`

---

## Updating Content

To update any section, just edit the HTML file and re-upload (or push via Git).

**Common updates:**
- New publication → Add a `<div class="pub-item">` block in `index.html` under Publications
- New talk → Add a `<div class="talk-item">` in the talks section
- Update contact info → Search for `oli.sudar@gmail.com` in both HTML files

---

## Add a Profile Photo (Optional)

1. Save your photo as `photo.jpg` in the same folder
2. In `index.html`, replace the `<div class="hero-visual">` section with:
```html
<div class="hero-visual">
  <img src="photo.jpg" alt="Dr. Sudaroli Dhananjeyan" style="width:280px;height:280px;border-radius:50%;object-fit:cover;border:3px solid var(--violet);" />
</div>
```

---

## Custom Domain (Optional, ~₹800/year)

1. Buy a domain like `sudaroli.com` from Namecheap or Google Domains
2. In your repo → Settings → Pages → Custom domain → enter your domain
3. Add a CNAME DNS record at your registrar pointing to `sudaroli1.github.io`

---

Built with plain HTML/CSS/JS — no frameworks, no build step.
