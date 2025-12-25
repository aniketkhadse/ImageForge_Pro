# ImageForge Pro

ImageForge Pro is a client-side web app for converting, optimizing, and compressing images directly in your browser — no uploads, no server, 100% private.

Live demo: https://image-forge-pro.vercel.app/

## Features

- Convert images between formats (JPEG, PNG, WebP, AVIF, etc.)
- Adjust quality/compression using a slider
- Resize images (width/height) and preserve aspect ratio
- Batch processing and preview of images
- Download processed images individually or as a ZIP (powered by JSZip & FileSaver.js)
- Runs fully in-browser (no files are uploaded to a server)

## How it works

1. Open the app in a modern browser (Chromium, Firefox, Safari).
2. Drag & drop images into the upload area or click the upload button.
3. Choose output format, set compression/quality, and optional size changes.
4. Preview processed results in the image grid.
5. Download each image or download all processed images as a ZIP archive.

## How to use locally

No build step is required for quick testing. You can either:

- Open `index.html` directly in your browser (double-click), or
- Serve the folder with a simple HTTP server for best compatibility (recommended):

  - Python 3:

    ```bash
    python -m http.server 8000
    ```

    Then open `http://localhost:8000` in your browser.

  - Node (serve):

    ```bash
    npm install -g serve
    serve .
    ```

## Requirements

- Modern browser with support for HTML5 Canvas and JS APIs
- No backend or internet connection required to use the core features (external libs are included via CDN)

## Files of interest

- `index.html` — main application UI and scripts

## Notes

- The app uses `JSZip` and `FileSaver.js` to prepare ZIP archives and trigger downloads.
- Because processing happens in the browser, performance depends on the client machine and image sizes.

## Live demo

Try the live deployment: https://image-forge-pro.vercel.app/

---

If you'd like, I can expand the README with screenshots, a quick FAQ, or contribution guidelines.   
