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
- **Customizable** — size (up to 1280px), 5 color themes, error correction level (L/M/Q/H), a center logo, and a caption label
- **Export your way** — download PNG or SVG, copy the image to the clipboard, or share it (native Web Share on mobile)
- **Keyboard shortcuts** — `⌘↵` download, `⌘C` copy, `⌘⇧S` SVG
- **Drag to save** — drag the QR straight into Finder or a chat window

## Tech Stack

- Pure HTML + CSS + JavaScript (no build tools, no framework) — the whole app is a single `index.html`
- [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) for QR generation (canvas + SVG output, full UTF-8 support)
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
