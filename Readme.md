# Deepanshu Garg — Portfolio Website

A professional, single-file portfolio site built for the UK financial industry. Hosted for free on **GitHub Pages** with zero dependencies, no build step, and no backend.

---

## 📂 Repository structure

```
portfolio/
├── index.html      ← the entire site (rename portfolio.html → index.html)
└── README.md       ← this file
```

> Everything lives in one HTML file — fonts load from Google Fonts CDN, and
> the favicon is an inline SVG. Nothing else to install or configure.

---

## 🚀 Step-by-step: publish on GitHub Pages

### Step 1 — Create a GitHub account (skip if you already have one)

1. Open [https://github.com](https://github.com) in your browser.
2. Click **Sign up** and complete the registration with your email and a password.
3. Verify your email address when GitHub sends the confirmation link.

---

### Step 2 — Create a new repository

1. Once logged in, click the **+** icon in the top-right corner and select **New repository**.
2. In the **Repository name** field type exactly:

   ```
   portfolio
   ```

3. Optionally add a short description, e.g. *"Personal finance portfolio website"*.
4. Make sure **Public** is selected (GitHub Pages requires this on free accounts).
5. Tick **Add a README file** — this creates the default branch for you automatically.
6. Click **Create repository**.

---

### Step 3 — Upload the files

1. Inside your new repository you will see the auto-generated `README.md`.
2. Click **Add file → Upload file** (the button near the top-right of the file list).
3. Drag and drop (or browse to) the two files:

   | File on your computer | Name it in GitHub |
   |---|---|
   | `portfolio.html` | **`index.html`** ← important: must be named exactly this |
   | `README.md` (this file) | `README.md` |

4. Scroll down to **Commit changes**, add an optional message like *"Initial portfolio upload"*, and click **Commit changes**.

---

### Step 4 — Enable GitHub Pages

1. In your repository, click **Settings** (the gear icon in the top navigation tabs).
2. In the left sidebar, click **Pages**.
3. Under **Branch**, select **main** (or **master** — whichever branch GitHub created).
4. Under **Folder**, select **/ (root)**.
5. Click **Save**.

GitHub will show a green banner with your live URL. It usually looks like:

```
https://[your-github-username].github.io/portfolio/
```

> It can take up to **60 seconds** for the site to go live the first time.

---

### Step 5 — View & share your site

1. Open the URL GitHub gave you in any browser.
2. You should see your full portfolio — scroll through every section to confirm everything renders correctly.
3. Copy the URL and share it on your LinkedIn profile, CV, or anywhere else.

---

## ✏️ How to make changes later

| What you want to do | How |
|---|---|
| Edit text / add a new project | Open `index.html` in GitHub → click the pencil ✏️ icon → edit → commit |
| Change your email or phone | Search for the relevant text in `index.html` and update it |
| Update the canonical URL | Find `og:url` and `canonical` in the `<head>` and replace the username part |

---

## 🔧 What was changed to make it GitHub-friendly

| Change | Why |
|---|---|
| Removed all `/cdn-cgi/…` Cloudflare email-obfuscation URLs | Those paths only exist on Cloudflare-proxied servers; they return 404 on GitHub Pages |
| Restored plain `mailto:` links | The correct, standard way to link to an email address — works everywhere |
| Removed the `email-decode.min.js` Cloudflare script | No longer needed; the email addresses are now in plain text |
| Added `<meta>` SEO tags (description, keywords, author, robots) | Helps Google and Bing index and rank the page |
| Added Open Graph (`og:…`) tags | Makes the link show a rich preview card when shared on LinkedIn, Slack, etc. |
| Added Twitter / X card tags | Same as above but for Twitter / X shares |
| Added `<link rel="canonical">` | Tells search engines the single authoritative URL — avoids duplicate-content penalties |
| Added an inline SVG favicon | The browser tab shows your "DG" logo instead of a broken icon — no extra file needed |

---

## 📬 How the contact form works

There is no server or database behind the contact form. When a visitor fills it in and clicks **Send Message**, the browser opens their default email client (Outlook, Gmail, Apple Mail, etc.) with a pre-filled email addressed to **deepanshugarg2110@gmail.com**. You receive the message the moment they hit Send — no third-party service required.

---

## 📄 License

This portfolio is for personal use only.