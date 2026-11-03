# 🔗 Noble Miles — Permanent Redirect Portal

This repository hosts the permanent, mobile-friendly redirect gateway for **Noble Miles**.

- **Permanent Public Link:** [https://navi-31.github.io/Noble-Miles-Link/](https://navi-31.github.io/Noble-Miles-Link/)
- **Current Target URL:** `https://tried-biz-hall-collective.trycloudflare.com/`

---

## 📱 How to Change the Cloudflare Tunnel URL From Your Phone (30 Seconds)

Whenever your Cloudflare Quick Tunnel URL changes on Termux / your Android phone, you can update your permanent link directly from your mobile browser without touching a computer or terminal:

1. Open **Chrome** (or any mobile browser) on your phone.
2. Go to your repository:  
   👉 `https://github.com/Navi-31/Noble-Miles-Link`
3. Tap on the file named **`index.html`**.
4. Tap the **pencil icon (✏️)** at the top right to edit the file.
5. Look at **line 18**:
   ```javascript
   const TARGET_URL = "https://your-new-tunnel.trycloudflare.com/";
   ```
6. Replace the old tunnel URL with your new Cloudflare URL (make sure it ends with `" ;`).
7. Scroll down and tap the green button: **"Commit changes..."** ➔ then tap **"Commit changes"**.

🎉 **That's it!** GitHub Pages will automatically update within ~30 seconds, and your permanent LinkedIn / trial link will immediately start pointing to the new tunnel.

---

## ⚙️ Initial One-Time GitHub Pages Setup (From Mobile Browser)

1. Open `https://github.com/Navi-31/Noble-Miles-Link` in your mobile browser.
2. Tap the **Settings** tab (gear icon ⚙️).  
   *(If on mobile view, tap the `...` menu or switch to "Desktop site" if Settings isn't immediately visible).*
3. In the left-hand menu, tap **Pages**.
4. Under **"Build and deployment"** ➔ **Source**:
   - Select **"Deploy from a branch"**.
   - Under **Branch**, select **`main`** and folder **`/(root)`**.
5. Tap **Save**.
6. Wait 1–2 minutes. Your permanent link will go live at:  
   **`https://navi-31.github.io/Noble-Miles-Link/`**

---

## 🛡️ Technical Architecture
- **Single File:** Self-contained `index.html` with zero npm packages, zero frameworks, and zero external CDNs.
- **Immediate Execution:** Uses `window.location.replace()` for instant redirect without cluttering the browser history.
- **Graceful Fallback:** If the live tunnel takes more than 3.5 seconds or is temporarily restarting, a clean Noble Miles branded screen appears with a direct link and retry button.
- **Zero Secrets:** No tokens, credentials, or private keys are used or exposed.
