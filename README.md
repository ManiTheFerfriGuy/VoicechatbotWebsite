# VoiceChatBot Shop Landing Page

A modern Persian landing page for promoting and selling the VoiceChatBot assistant. The page is lightweight, responsive, and designed to work as a single static site on shared hosting (including cPanel).

## Features

- Persian copy with modern dark/minimal styling
- Smooth scrolling navigation with active-section highlighting
- Responsive layout for desktop and mobile
- Automatic current-year update in the footer via JavaScript

## Project Structure

- `index.html` — Page markup and content (Persian).
- `styles.css` — Minimal dark theme, typography, and responsive layout.
- `script.js` — Smooth scrolling, menu highlighting, and footer year injection.

## Local Development

1. Clone the repository and switch to the project folder.
2. Start a simple HTTP server (for example with Python):

   ```bash
   python -m http.server 8000
   ```

3. Open `http://localhost:8000` in your browser to preview `index.html`.

## Deploying on cPanel

1. Zip the project files (`index.html`, `styles.css`, `script.js`, and any assets) on your machine.
2. Log in to cPanel and open **File Manager**.
3. Navigate to your web root (commonly `public_html/`).
4. Upload the zip archive and extract it inside the web root.
5. Ensure the main page is named `index.html` in the root. If you placed files in a subfolder, access it via `https://your-domain.com/subfolder/`.
6. Clear any caching (browser or CDN) and reload the site.

### Fixing 404 errors on cPanel

- Verify that `index.html` exists in `public_html/` (or the subdirectory you are visiting).
- Remove default `index.php`/`default.html` files if they conflict with your `index.html`.
- Check that the domain or subdomain points to the correct document root in **Domains** → **Document Root**.
- If you uploaded to a subfolder, include that path in the URL (e.g., `https://your-domain.com/voicechatbot/`).

## Customization Tips

- Update copy and prices directly in `index.html` (content is in Persian).
- Adjust colors, spacing, or typography in `styles.css` to match your brand.
- Extend `script.js` if you need analytics events or additional UI behaviors.

## License

This project is released under the MIT License. Feel free to use, modify, and deploy it for your own shop.
