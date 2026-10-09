# X-TPL: Dataset Showcase Website

Website for the Tool Demonstration and Data Showcase Track submission:
> **X-TPL: A Ground-Truth Dataset of Cross-Platform Android Apps and their Third-Party Libraries**  
> *Jordi Tim Frederik, Thomas Sutter, Timo Kehrer* — University of Bern

Live site: [https://x-tpl.github.io/](https://x-tpl.github.io/)

---

## Structure & Placeholders

The site is built as a static site hosted on GitHub Pages (`index.html` + `static/`).

### 1. YouTube Data Video Placeholder
In `index.html` (inside `<section id="video-showcase">`):
- Currently references `https://youtu.be/PLACEHOLDER`.
- To embed or link your real video once recorded:
  - Replace `https://youtu.be/PLACEHOLDER` with your YouTube video link.
  - Or embed the standard YouTube iframe:
    ```html
    <iframe src="https://www.youtube.com/embed/<YOUR_VIDEO_ID>" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    ```

### 2. Diagram Placeholders
Placeholders are pre-styled with mock wireframes and descriptive captions:
- **Diagram Placeholder 1 (`#dataset-variations`)**: Number of Compiled Apps & Unique TPLs across Cross-Platform Frameworks (Flutter, React Native, Cordova, .NET MAUI).
  - Place your exported plot SVG/PNG under `static/images/diagram_apps_distribution.svg` and replace the wireframe `div` with `<img src="static/images/diagram_apps_distribution.svg" alt="...">`.
- **Diagram Placeholder 2 (`#dataset-variations`)**: Build Variations (Debug vs. Release with R8 code shrinking vs. native obfuscation) and Target Architectures (ARM, x86).
  - Place your plot at `static/images/diagram_build_variations.svg`.
- **Diagram Placeholder 3 (`#curation-pipeline`)**: Overview of the automated curation pipeline (Crawling &rarr; Analysis &rarr; Containerized Compilation &rarr; Lockfile/APK Extraction).
  - Place your plot at `static/images/diagram_pipeline_overview.svg`.

### 3. Dataset Table & Counts
- In `index.html`, Table 1 contains `XXXX` placeholders matching the paper draft. Once final build counts are finalized, update the numbers in the table and metrics cards.

---

## Local Preview & Hot Reloading

### With Hot Reloading (Auto-refreshes on save)
Run:
```bash
npm run dev
# or directly:
npx live-server
```
This automatically starts a local server at `http://127.0.0.1:8080`, opens it in your default browser, and refreshes the page whenever you edit `index.html` or CSS.

### Simple Static Server (No hot reload)
```bash
python3 -m http.server 8000
```

