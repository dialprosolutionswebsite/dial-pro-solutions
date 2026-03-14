# Dial Pro Solutions — Website

Smart Business Savings & Technology Solutions

**Live at:** [dialprosolutions.co.uk](https://dialprosolutions.co.uk)

---

## Deploy to Netlify + Connect GoDaddy Domain

Follow these steps exactly to get your site live with your custom domain.

---

### STEP 1 — Create a GitHub Account (if you don't have one)

1. Go to [github.com](https://github.com)
2. Click **Sign up** and create a free account
3. Verify your email address

---

### STEP 2 — Upload This Project to GitHub

**Option A — Using GitHub Desktop (Easiest)**

1. Download [GitHub Desktop](https://desktop.github.com/) and install it
2. Sign in with your GitHub account
3. Click **File → Add Local Repository**
4. Select the folder containing this project
5. Click **Publish Repository**
6. Give it a name like `dial-pro-solutions`
7. Make sure **Keep this code private** is checked if you want it private
8. Click **Publish Repository**

**Option B — Using GitHub Website (Drag & Drop)**

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `dial-pro-solutions`
3. Click **Create repository**
4. On the next page, click **uploading an existing file**
5. Drag and drop ALL the files from this project folder
6. Click **Commit changes**

---

### STEP 3 — Create a Free Netlify Account

1. Go to [netlify.com](https://netlify.com)
2. Click **Sign up** → choose **Sign up with GitHub**
3. Authorize Netlify to access your GitHub

---

### STEP 4 — Deploy the Site on Netlify

1. Once logged into Netlify, click **Add new site**
2. Choose **Import an existing project**
3. Click **Deploy with GitHub**
4. Find and select your `dial-pro-solutions` repository
5. Netlify will auto-detect the settings from `netlify.toml` — **do not change anything**
6. Click **Deploy site**
7. Wait 2–3 minutes for the build to complete
8. Your site will go live at a temporary address like `amazing-name-123.netlify.app`

---

### STEP 5 — Connect Your GoDaddy Domain

#### In Netlify:

1. Go to your site in Netlify
2. Click **Domain management** (or **Set up a custom domain**)
3. Type your domain: `dialprosolutions.co.uk`
4. Click **Verify** → then **Add domain**
5. Netlify will show you **nameserver addresses** that look like:
   ```
   dns1.p01.nsone.net
   dns2.p01.nsone.net
   dns3.p01.nsone.net
   dns4.p01.nsone.net
   ```
   **Copy all 4 of these — you'll need them in the next step.**

#### In GoDaddy:

1. Go to [godaddy.com](https://godaddy.com) and sign in
2. Click your name (top right) → **My Products**
3. Find your domain and click **DNS** or **Manage DNS**
4. Scroll to the **Nameservers** section
5. Click **Change** → choose **Enter my own nameservers (advanced)**
6. Delete the existing nameservers
7. Enter Netlify's 4 nameservers (from the step above)
8. Click **Save**
9. Confirm the change when prompted

**That's it!** DNS changes take between **30 minutes and 48 hours** to fully propagate. Netlify will automatically set up your free SSL certificate (https) once the domain is active.

---

### STEP 6 — Set Up www Redirect (Optional but Recommended)

In Netlify → Domain management:
1. Click **Add domain alias**
2. Add `www.dialprosolutions.co.uk`
3. Netlify will automatically redirect `www` to your main domain

---

## How Lead Forms Work

All enquiry forms on the website use **Netlify Forms** — they work automatically when the site is deployed on Netlify. No extra setup needed.

Form submissions will appear in:
**Netlify Dashboard → Your Site → Forms**

You can also set up **email notifications** for each form:
1. Go to **Site settings → Forms → Form notifications**
2. Add an email notification
3. Enter `support@dialprosolutions.co.uk`
4. Save — you'll now get an email every time someone submits a form

---

## Pages

| Page | URL |
|------|-----|
| Home | `/` |
| Card Payments | `/card-payments` |
| Gas Energy | `/gas-energy` |
| Electric Energy | `/electric-energy` |
| Business Websites | `/business-websites` |
| Other Solutions | `/other-solutions` |
| About | `/about` |
| Contact | `/contact` |

---

## Contact Details on the Site

- **Phone/WhatsApp:** 0131 381 0343
- **Email:** support@dialprosolutions.co.uk
- **Address:** 5 South Charlotte Street, Edinburgh, EH2 4AN
- **Hours:** Monday–Friday, 9:30 AM – 7:00 PM

---

## Tech Stack

- React + Vite
- TailwindCSS
- Framer Motion (animations)
- Netlify Forms (lead capture)
- Wouter (routing)
