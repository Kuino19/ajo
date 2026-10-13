# ₦ Ajo Tracker (Progressive Web App)

A modern, fast, and offline-first **Progressive Web App (PWA)** built to manage rotating thrift contributions, daily/weekly savings circles, and Ajo/Esusu groups seamlessly.

![Ajo Tracker](icon-192.png)

---

## ✨ Features

- **🔄 Rotating Round Tracking**: Track member turns, beneficiaries, contribution frequencies, and running totals.
- **📱 Installable Progressive Web App (PWA)**:
  - Add to Home Screen on iOS and Android or install as a desktop application.
  - Complete with high-resolution app icons, maskable icons, and a custom theme color (`#0f7b4a`).
- **⚡ 100% Offline-First**: Built with a Service Worker (`sw.js`) that pre-caches all assets. Track payments anywhere even without internet access.
- **🔒 Passcode / PIN Protection**:
  - Secure your savings data with a 4-digit PIN lock screen.
  - Client-side salted SHA-256 cryptographic hashing.
  - Built-in session lock button and emergency recovery options.
- **📲 Direct WhatsApp Integration**: Format contribution updates, receipts, and round summaries with a single click to paste directly into your WhatsApp group.
- **💾 Easy Backup & Restore**: Export full JSON backups or restore data across devices with zero setup.

---

## 📁 Repository Structure

```
ajo/
├── index.html               # Main PWA application & UI
├── manifest.json            # Web App Manifest
├── sw.js                    # Service Worker for offline caching
├── favicon.svg              # Vector brand favicon
├── favicon.ico              # Standard favicon
├── icon-192.png             # PWA app icon (192x192)
├── icon-512.png             # PWA app icon (512x512)
├── icon-maskable-192.png    # Adaptive maskable icon (192x192)
├── icon-maskable-512.png    # Adaptive maskable icon (512x512)
├── apple-touch-icon.png     # iOS touch icon (180x180)
└── README.md                # Project documentation
```

---

## 🚀 Getting Started

### Run Locally

Since Service Workers require an HTTP/HTTPS origin, serve the folder with any static local server:

```bash
# Using Python
python -m http.server 8080

# Or using Node.js
npx serve .
```

Open `http://localhost:8080` in your browser.

---

## 🌐 Deploy to GitHub Pages

1. In your GitHub repository, navigate to **Settings** > **Pages**.
2. Under **Build and deployment** > **Branch**, select `main` (root) and click **Save**.
3. Your Ajo Tracker PWA will be live at `https://kuino19.github.io/ajo/`!

---

## 📄 License

MIT License. Free for community savings circles and personal use.
