# NFDP_v17 Cloud Portal – Live Deploy Guide (Free)

This bundle is **deploy-ready** for both **Firebase Hosting** (recommended) and **GitHub Pages** (simple).

---

## Option A — Firebase Hosting (Google) ✅
**Prereqs:** Google account (use `anilram4@gmail.com`), Chrome, basic terminal

1. Install tools (one-time):
   - Windows/Mac: install Node.js (https://nodejs.org)
   - Then open Terminal/Command Prompt and run:
     ```bash
     npm install -g firebase-tools
     firebase login
     ```

2. Unzip this folder, open it in Terminal:
   ```bash
   cd NFDP_v17_Portal_Deploy
   ```

3. Set your Firebase project (first time):
   ```bash
   firebase projects:create nfdp-tumsar-portal --display-name "NFDP Tumsar Portal"
   firebase use nfdp-tumsar-portal
   ```
   *(If project already exists, just run `firebase use nfdp-tumsar-portal`)*

4. Deploy:
   ```bash
   firebase deploy
   ```

5. You’ll get a URL like:
   **https://nfdp-tumsar-portal.web.app**  → Share this as the **Live Portal**.

---

## Option B — GitHub Pages (Zero-config)
1. Create a repo: **nfdp-portal**
2. Upload files from this folder (index.html + others)
3. In the repo → Settings → Pages → Source = **main** branch → root (`/`) → Save
4. Your site will be at:
   **https://<your-username>.github.io/nfdp-portal/**

---

## Next Bindings (when ready)
- **Forgot Password (OTP)**: attach email service; subject → `Your NFDP One-Time Password (OTP)`
- **Google Sheet Binding**: connect to NFDP v16 Cloud Sheet via Apps Script / API proxy
- **DVC Verification**: simple Firebase collection `nfdp-verifications`

**Support:** Powered by R. Anil | 📞 8698398865 | Email: anilram4@gmail.com
