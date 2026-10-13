# NOC Network Diagram Studio

A lightweight, customizable network topology diagram editor built with plain HTML, CSS, JavaScript, and SVG. Designed for GitHub Pages; no build tools, backend, or dependencies required.

## Features
- Drag-and-drop network nodes
- Edit node labels, categories, and accent colors
- Connect two nodes and edit connection labels, colors, and line styles
- Add or delete nodes and connections
- Export diagrams to SVG or PNG
- Import/export diagram JSON to save and reuse layouts
- Responsive dark UI inspired by an ISP / Internet Exchange topology diagram

## Run locally
Open `index.html` in a modern browser. For best results, use a local static server or GitHub Pages.

## Publish with GitHub Pages
1. Create a public GitHub repository under your account `ishall21`, named `noc-network-diagram`.
2. Upload the contents of this folder to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then save.
6. Wait for the Pages deployment. Your expected URL is https://ishall21.github.io/noc-network-diagram/.

## Customize the starter topology
- Edit `initial.nodes` and `initial.edges` in `app.js` to change the default diagram.
- Node categories: `network`, `router`, `exchange`, `service`, `server`, `people`.
- Edge properties: `from`, `to`, `label`, `color`, and `style` (`solid`, `dashed`, or `dotted`).

## Project structure
```text
noc-network-diagram/
├── index.html
├── style.css
├── app.js
├── README.md
├── CHANGELOG.md
├── VERSION
├── LICENSE
└── .nojekyll
```

## Notes
This is a client-side editor. Changes are not automatically saved to GitHub; export the JSON file to preserve a layout, or update the starter data in `app.js` and commit it to your repository.
