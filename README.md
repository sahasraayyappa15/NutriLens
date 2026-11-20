# NutriLens

NutriLens is a responsive snack-discovery demo that helps you explore snack nutrition, compare alternatives, and track small snack swaps. It is built with HTML, CSS, and vanilla JavaScript; there is no build step or package installation.

> **Demo notice:** Nutrition values and product matches are illustrative sample data, not verified product labels. The barcode page uses a local demo catalog and does not connect to a live product database or use your camera.

## Features

- Browse, search, filter, and sort a catalog of 46 sample snacks.
- View snack nutrition details and compare snack alternatives.
- Try a barcode lookup against the included demo data.
- Track snack swaps, weekly challenges, and progress in your browser.
- Explore hostel-friendly snack ideas and a sugar-cube visualizer.
- Export your swap history as a CSV file.

## Pages

| Page | Description |
| --- | --- |
| `index.html` | Home page and introduction |
| `explore.html` | Searchable and filterable snack catalog |
| `nutrition.html` | Nutrition details for a selected snack |
| `compare.html` | Compare snacks and log a swap |
| `scanner.html` | Look up sample barcodes in the demo catalog |
| `dashboard.html` | Summary of swaps and weekly progress |
| `progress.html` | Swap history, achievements, and CSV export |
| `challenges.html` | Weekly snack challenge |
| `hostel-hacks.html` | Budget-friendly snack ideas |
| `sugar.html` | Visual comparison of sugar in selected drinks |

## Run locally

No dependencies need to be installed. From the project folder, start a local static web server:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000> in your browser. Alternatively, open the folder in Visual Studio Code and use a static-site extension such as Live Server.

The site loads Bootstrap, Bootstrap Icons, Chart.js, AOS, and web fonts from CDNs, so an internet connection is needed for those external assets. Swap and challenge progress is saved in the browser's `localStorage` on the current device.

## Project structure

```text
NutriLens/
├── assets/
│   └── images/       # Snack photos and image source notes
├── css/              # Site styles and responsive layouts
├── js/               # Snack data and page behavior
├── *.html            # Site pages
└── README.md
```

## Publish to GitHub

Create an empty repository on GitHub, then run these commands from this project folder. Replace the URL with your repository's URL:

```bash
git init
git add .
git commit -m "Add NutriLens website"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repository>.git
git push -u origin main
```

To host the static site with GitHub Pages, open the repository's **Settings → Pages**, choose the `main` branch and `/ (root)` folder, then save.

## Image credits

Image source and license information for local photos is listed in [`assets/images/SOURCES.txt`](assets/images/SOURCES.txt). The included photos are illustrative and do not depict a specific packaged brand.
