# PDF Studio

**A free, browser-based PDF editor. No document uploads, backend, or database.**

## Overview

PDF Studio is a static web application designed to edit PDF files locally in the browser. It uses PDF.js for rendering and PDF-lib for writing documents.

## Quick start

After the source files are uploaded, run from the project root:

```bash
python -m http.server 8000
```

Open `http://localhost:8000`. Do not open `index.html` directly using `file://`.

## Deployment

No build step is required. Serve the project directory using HTTPS or localhost. Supports Apache/cPanel, GitHub Pages, Netlify, Vercel and Cloudflare Pages. The bundled `.htaccess` is intended for Apache. For Nginx, configure MIME types for `.mjs` and `.wasm`.

## Privacy and limitations

Documents are processed in the browser. Fontkit is loaded from jsDelivr when saving PDFs; if unavailable, some accented and Cyrillic characters may be replaced. This is not a fully offline guarantee.

## Project structure

- `index.html` — application and styles
- `vendor/` — bundled PDF libraries and resources
- `fonts/` — Liberation fonts
- `licenses/` — third-party licensing notices
- `.htaccess` — Apache configuration

## Roadmap

- [ ] Upload complete application source and bundled resources
- [ ] Verify deployment and add screenshots
- [ ] Improve offline support and test document editing
- [ ] Confirm project license and contribution guidelines

## License

Project license pending. Preserve all bundled third-party license notices.
