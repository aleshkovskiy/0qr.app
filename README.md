# 0qr.app — Free QR Code Generator, Forever

A fast, free, and private QR code generator that runs entirely in your browser. No ads. No registration. No tracking. No paywalls. Just QR codes.

## Why?

Every QR code generator out there is either:
- **Paid** — basic features locked behind a subscription
- **Requires signup** — just to generate a simple QR code
- **Cluttered with ads** — slow to load, painful to use
- **Tracks your data** — your URLs and content sent to their servers

0qr.app exists because generating a QR code should be instant, free, and private. Always.

## Features

- **Instant** — QR codes generated in real time as you type
- **Private** — everything happens in your browser, nothing is sent to any server
- **Free forever** — no subscriptions, no freemium tiers, no limits
- **No registration** — just open and use
- **Multiple QR types:**
  - URL / Link
  - Plain text
  - WiFi credentials
  - vCard (contact info)
  - Email (with subject & body)
  - SMS
  - WhatsApp message
  - Phone number
- **Customizable** — size, color themes, error correction level
- **Download as PNG** or copy to clipboard

## Tech Stack

- Pure HTML + CSS + JavaScript (no build tools, no framework)
- [QRCode.js](https://github.com/davidshimjs/qrcodejs) for QR generation
- Deployed on **Cloudflare Workers** — globally distributed, always fast, always free

## Self-hosting

Just serve `index.html` — that's the entire app. Works from any static host, CDN, or even directly from the filesystem (`file://`).

**Deploy your own copy in 2 minutes:**

```bash
git clone https://github.com/aleshkovskiy/0qr.app
cd 0qr.app
npx wrangler deploy
```

Or use [Cloudflare Pages](https://pages.cloudflare.com), [Netlify](https://netlify.com), [Vercel](https://vercel.com), or GitHub Pages — no build step required, just point at `index.html`.

## License

MIT — do whatever you want with it.
