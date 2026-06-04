# Farm Yawmi · مزرعة يومي

> Apple orchard dashboard — Khenchela, Algeria

## Setup Instructions (5 minutes)

### Step 1 — Create the GitHub repository

1. Go to [github.com](https://github.com) and log in as **benaicha07-rgb**
2. Click the **+** button (top right) → **New repository**
3. Repository name: `farm-yawmi`
4. Set to **Public**
5. Click **Create repository**

---

### Step 2 — Upload the files

1. In your new repository, click **uploading an existing file**
2. Upload these files:
   - `index.html` (the dashboard)
   - `.github/workflows/daily_email.yml` (the email automation)
   - `README.md` (this file)
3. Click **Commit changes**

> ⚠️ The `.github` folder may be hidden on your computer. Make sure to upload the workflow file inside `.github/workflows/`

---

### Step 3 — Enable GitHub Pages

1. In your repository, go to **Settings** → **Pages** (left sidebar)
2. Under **Source**, select **Deploy from a branch**
3. Branch: **main** / folder: **/ (root)**
4. Click **Save**
5. Wait 1–2 minutes — your dashboard will be live at:
   **https://benaicha07-rgb.github.io/farm-yawmi**

---

### Step 4 — Set up Gmail for sending emails

GitHub Actions needs permission to send emails from your Gmail.

1. Go to your Google Account → **Security** → **2-Step Verification** (enable if not already)
2. Go to **Security** → **App passwords**
3. Create a new App password:
   - App: **Mail**
   - Device: **Other** → type "Farm Yawmi"
4. Google gives you a 16-character password — **copy it**

---

### Step 5 — Add secrets to GitHub

1. In your repository, go to **Settings** → **Secrets and variables** → **Actions**
2. Click **New repository secret** and add:

| Name | Value |
|---|---|
| `MAIL_USERNAME` | `benaicha07@gmail.com` |
| `MAIL_PASSWORD` | *(the 16-char App password from Step 4)* |

---

### Step 6 — Test the email

1. Go to your repository → **Actions** tab
2. Click **Farm Yawmi — Daily Morning Brief**
3. Click **Run workflow** → **Run workflow**
4. Check your Gmail inbox — the daily brief should arrive within 1 minute

---

## Daily email schedule

- **Time:** 7:00 AM Algeria time (UTC+1) every day
- **Recipient:** benaicha07@gmail.com
- **Content:** Today's tasks, irrigation reminder, season stage, harvest alerts

## Dashboard URL

**https://benaicha07-rgb.github.io/farm-yawmi**

Open this on any device — phone, tablet, laptop — simultaneously.
