# Generative Digital Twins: Vision-Language Simulation Models for Executable Industrial Systems

Project page for the CVPR 2026 submission  
**“Generative Digital Twins: Vision-Language Simulation Models for Executable Industrial Systems”** (under review).

> **Status:** Authors and affiliations are kept anonymous to comply with double-blind review.

---

## Project Page

The static project page is hosted via GitHub Pages:

**Live page:**  
https://danielhsu2014.github.io/GDT-VLSM-project/

This page provides a high-level overview of:

- The GDT-120K dataset construction pipeline  
- Vision-Language Simulation Models (VLSM) architecture  
- Prototype interface for layout-and-prompt → FlexScript generation  
- Qualitative results on held-out industrial layouts and LLM backbones

For training code, checkpoints, and data configuration, please refer to the main `GDT-VLSM` repository (separate from this project-page repo).

---

## Repository Structure

This repository only contains the **static website** for the paper project page.

```text
GDT-VLSM-project/
├── index.html              # Main project page (single HTML entry point)
└── static/
    ├── css/
    │   ├── bulma.min.css   # Bulma CSS framework
    │   └── index.css       # Custom styling for this project
    ├── js/
    │   ├── bulma-carousel.min.js
    │   ├── bulma-slider.min.js
    │   └── index.js        # Minimal JS for scroll-to-top, etc.
    └── images/
        ├── first_pic.png       # Teaser / overview figure
        ├── dataset_pipeline.png
        ├── VLSM_Pipeline.png
        ├── UI.png              # Prototype interface screenshot
        ├── Fig5_3.png          # Main qualitative examples
        ├── 5.2Quant.png        # LLM backbone comparison
        ├── suppl_2.png         # Additional qualitative example
        ├── suppl_3.png         # Additional qualitative example
        └── favicon.ico         # (Optional) browser tab icon
```

There is **no backend** and no build step; everything is plain HTML/CSS/JS.

---

## How to Edit the Page

Most content lives in a single file:

- **`index.html`**  
  - Title, meta tags  
  - Abstract  
  - Section texts (Dataset, VLSM, Prototype Interface, Qualitative Results)  
  - `<img src="static/images/....png">` for all figures

Typical edits you may want to make:

1. **Update text (e.g., after acceptance)**
   - Open `index.html`
   - Search for the relevant section headers:
     - `Abstract`
     - `Dataset Construction and Timing Distributions`
     - `Vision-Language Simulation Models`
     - `Prototype Interface`
     - `Qualitative Results`
   - Modify the paragraphs under each section.

2. **Replace figures**
   - Put new image files into `static/images/`.
   - Keep the same filenames (easiest), or:
   - Update the corresponding `src` attributes in `index.html`, for example:
     ```html
     <img src="static/images/first_pic.png" alt="..." />
     ```

3. **Favicon (optional)**
   - To customize the browser tab icon, replace `static/images/favicon.ico`
   - Or remove the favicon lines in `<head>` if you prefer not to use one.

---

## Local Preview

You can test the page locally before pushing changes.

From the repository root:

```bash
# Option 1: Python simple HTTP server (Python 3)
python -m http.server 8000

# Then open in your browser:
# http://localhost:8000
```

Any edits to `index.html` or files in `static/` can be reloaded by refreshing the page.

---

## Deploying via GitHub Pages

This repository is set up to use **GitHub Pages**:

- Source: `main` branch  
- Publishing folder: root of this repo

On each push to `main`, GitHub Pages will automatically rebuild and publish the updated version to:

> `https://<github-username>.github.io/GDT-VLSM-project/`

You can verify or change the settings under:  
**Repository → Settings → Pages**

---

## License & Template Acknowledgment

This project page is based on:

- **Academic Project Page Template**  
  https://github.com/eliahuhorwitz/Academic-project-page-template  
- Originally adapted from the **Nerfies** project page:  
  https://nerfies.github.io

Please keep the attribution in the footer, as required by the template.

Unless otherwise noted, the website content in this repository follows the same license as the main paper/code (to be finalized after the review process).
