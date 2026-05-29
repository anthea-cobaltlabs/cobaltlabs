# Cobalt Labs — website

Static marketing site. No build step, no server — just HTML, CSS, and a little JavaScript.

## Files

| File | What it is |
|------|------------|
| `index.html` | The whole site |
| `styles.css`, `home.css` | Styles |
| `image-slot.js` | Renders the photos in the case-study cards + team headshots |
| `image-slots.state.json` | The actual uploaded images (do not delete) |
| `assets/` | Other images (Womaness case photo, "senior operators" photo) |
| `.nojekyll` | Tells GitHub Pages to serve every file as-is |

## Before you launch: turn on the contact form (one-time, ~2 min)

The form emails submissions straight to your inbox via a free service called **Web3Forms** — no server required.

1. Go to **https://web3forms.com**
2. Enter your email (**anthea@cobaltlabs.co**) — they email you an **access key**
3. Open `index.html`, find this line near the bottom:
   ```js
   const WEB3FORMS_ACCESS_KEY = "YOUR_ACCESS_KEY_HERE";
   ```
4. Paste your key between the quotes and save.

Until you do this, the form shows an error when someone hits submit.

## Publish with GitHub Pages

1. Upload **all** of these files to your repo (keep the folder structure — `assets/` stays a folder).
2. In your repo: **Settings → Pages**.
3. Under "Build and deployment", set **Source = Deploy from a branch**, branch = `main`, folder = `/ (root)`.
4. Save. Your site goes live at `https://<your-username>.github.io/<repo>/` in a minute or two.

### Custom domain (optional)
In **Settings → Pages → Custom domain**, enter your domain (e.g. `cobaltlabs.co`) and follow the DNS instructions GitHub shows.

## Editing later
Everything is plain HTML — open `index.html` in any editor to change copy. To swap a case-study or headshot photo, the simplest path is to come back here and ask, then re-export.
