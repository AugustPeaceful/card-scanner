# Card Scanner PWA

Business card scanner powered by **Claude Vision API**.  
Reads printed text + handwritten notes in any language (EN, RU, JP, KR, CN).

## Files

```
index.html     ← full app (single file)
manifest.json  ← PWA manifest
sw.js          ← service worker (offline cache)
icon-192.png   ← app icon
icon-512.png   ← app icon large
README.md      ← this file
```

## Deploy to GitHub Pages

1. Upload all 6 files to a **public** GitHub repo
2. Settings → Pages → Branch: main → Save
3. Open `https://USERNAME.github.io/REPO-NAME/` in **Safari** on iPhone
4. Share → Add to Home Screen

## First Launch

1. App asks for **Claude API Key**
2. Get free key: [console.anthropic.com](https://console.anthropic.com) → API Keys → Create Key
3. Key saved locally on device only

## Usage

1. Tap **Камера** or **Галерея** → select business card photo
2. Tap **Сканировать**
3. Claude reads: printed text + handwritten notes + all languages
4. Edit fields if needed → **Добавить в контакты**
5. Export: **CSV** or **JSON**

## Cost

~$0.01 per card = $5 for ~500 cards

## Why Claude Vision?

Tesseract OCR fails on:
- Handwritten Russian/English notes
- Mixed Japanese + English cards  
- Low contrast or angled photos

Claude Vision handles all of these correctly.
