# NFDP v17 — Add-on Pages (GitHub Pages)
Date: October 29, 2025

Add these pages to your repo root:

- **verify.html** — Digital Verification Code checker (demo list with `DVC–TUM2025–001`).
- **otp.html** — Forgot Password (OTP) flow UI (demo only).

## How to link from index.html
Add links like:
```html
<a href="verify.html">Verify DVC</a> • <a href="otp.html">Forgot Password</a>
```

Later:
- Replace the JS list in `verify.html` with an API call to Firebase/Sheet.
- Connect `otp.html` to your email service to actually send OTPs.

Support: Powered by R. Anil • +91 8698398865 • Email: anilram4@gmail.com
