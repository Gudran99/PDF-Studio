# PDF Studio

**A free, browser-based PDF editor. No document uploads, backend, or database.**

[**Launch PDF Studio**](https://gudran99.github.io/PDF-Studio/) · [Report an issue](https://github.com/Gudran99/PDF-Studio/issues)

## Overview

PDF Studio is a static web application designed to edit PDF files locally in the browser. It uses PDF.js for rendering and PDF-lib for writing documents.

## Features

- Edit existing text in text-based PDFs and add new text.
- Insert and crop images, highlight, draw and add shapes.
- Create fillable text fields.
- Merge, rotate, reorder, duplicate and delete pages.
- Export edited documents without an account or watermark.

## Quick start

To run locally, execute from the project root:

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

- [x] Upload application source and bundled resources
- [x] Publish GitHub Pages deployment
- [ ] Test live application and add screenshots
- [ ] Improve offline support and test document editing
- [x] Add MIT license for original project code
- [x] Add contribution guidelines and issue templates
- [ ] Verify third-party license compliance

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for development and contribution instructions, and [CHANGELOG.md](CHANGELOG.md) for project changes.

## License

Original project code is released under the [MIT License](LICENSE). Bundled third-party libraries, fonts and other assets remain subject to their respective licenses and notices in `licenses/` and accompanying files.
