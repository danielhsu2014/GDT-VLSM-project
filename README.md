# Generative Digital Twins: Vision-Language Simulation Models for Executable Industrial Systems

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
---

## License

This repository is released under the MIT License (see LICENSE).

## Model Usage Notice

The models, model weights, checkpoints, and any generated outputs
associated with this project are released for academic research
and educational purposes only.

Commercial use, including but not limited to use in for-profit
products, services, internal industrial deployment, or technology
transfer, is strictly prohibited without prior written permission
from the authors.

Please contact the authors for commercial licensing inquiries.

## License & Template Acknowledgment

This project page is based on:

- **Academic Project Page Template**  
  https://github.com/eliahuhorwitz/Academic-project-page-template  
- Originally adapted from the **Nerfies** project page:  
  https://nerfies.github.io

Please keep the attribution in the footer, as required by the template.

Unless otherwise noted, the website content in this repository follows the same license as the main paper/code (to be finalized after the review process).
