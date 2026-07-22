# WingGrove Tree Care — Landing Page

Single-file, responsive landing page. No build step, no dependencies (fonts load from Google Fonts CDN). Works on GitHub Pages as-is.

## Folder structure

```
winggrove-site/
├── index.html          ← the whole site
├── README.md           ← this file
└── images/             ← drop your photos + logo here (names must match exactly)
    ├── logo.png                    (your WingGrove logo — dark text, for the light header)
    ├── logo-white.png              (white-text version of the logo, for the dark footer)
    ├── isa-certified-arborist.png
    ├── hero.jpg
    ├── service-pruning.jpg
    ├── service-removal.jpg
    ├── service-hedge.jpg
    └── service-garden.jpg
```

## Add your images

The page references the filenames below. Drop each file into the `images/` folder using the **exact** name. The page still looks clean if a file is missing (it falls back to a green gradient / a text ISA chip), so you can add them one at a time.

| Filename | What to use | Suggested photo from the ones you sent |
|---|---|---|
| `logo.png` | Your WingGrove logo for the **light header** — needs **dark/green text** so it's readable on white. Transparent PNG. | Your logo (dark-text version) |
| `logo-white.png` | Your WingGrove logo for the **dark footer** — the **white-text version** you sent. Transparent PNG. | Your logo (white-text version) |
| `isa-certified-arborist.png` | The ISA Certified Arborist logo (ICA-400), transparent PNG | The green ISA badge |
| `hero.jpg` | Big background behind the headline. Wide, bright, safety gear visible | Arborist rappelling next to the house roof (green helmet, aerial view) |
| `service-pruning.jpg` | Pruning card | Climber on a branch cutting against blue sky (red shirt) |
| `service-removal.jpg` | Removal card | Chainsaw felling the pine with sawdust spray |
| `service-hedge.jpg` | Hedge card | Chainsaw cutting the log / any green foliage shot |
| `service-garden.jpg` | Garden Maintenance card | Climbing harness close-up, or any tidy-yard shot |

Landscape (wide) JPEGs around 1600×1000px look best. Keep each file under ~400 KB for fast loading (compress at [squoosh.app](https://squoosh.app) if needed).

## Where the contact form goes

By default the **Get My Free Quote** button opens the visitor's email app with all their details pre-filled, addressed to `wing@winggrovetreecare.ca`. No backend needed — perfect for a static site, and it fits your hand-quotation workflow.

If you'd rather receive form submissions as clean emails/notifications without relying on the visitor's mail app, create a free form endpoint (e.g. [Formspree](https://formspree.io)) and paste the URL into one line near the bottom of `index.html`:

```js
var FORM_ENDPOINT = "https://formspree.io/f/your-id";
```

## Publish on GitHub Pages

1. Create a new repository (e.g. `winggrove-treecare`).
2. Upload the contents of this `winggrove-site` folder (so `index.html` is at the repo root).
3. Repo **Settings → Pages → Source: Deploy from a branch → `main` / root → Save**.
4. Your site goes live at `https://<your-username>.github.io/winggrove-treecare/` within a minute.
5. To use a custom domain (e.g. `winggrovetreecare.ca`), add it under Settings → Pages → Custom domain.

## Still to confirm before going fully live

- **Price ranges** in the Services section are illustrative CAD placeholders — swap in your real "starting from" numbers.
- **Insurance wording** ("Fully Insured · WorkSafeBC Compliant") — confirm it's accurate.
- **Social links** — Facebook / Instagram aren't linked yet; add them in the footer if you want them.

## Notes on your edits (applied)

- The **5% first-service discount and the WELCOME5 code were removed entirely** — pricing stays hand-quotation only, as you asked.
- Phone set to **(672) 866-4653**, email **wing@winggrovetreecare.ca**, Google Reviews button links to your shared review URL.
- ISA logo placed in three spots: hero, contact section, footer.
