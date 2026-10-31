# IONVERSE LAB — Phase 3.2 Smart Realistic

Open `index.html` on GitHub Pages (or use `python3 -m http.server`). Online access is required for Three.js imported from jsDelivr. Source modules live in `src/`; tests run with `npm test` (Node 20+).

## Improvements
- Selecting a chemical or changing concentration automatically prepares a fresh 4 mL sample and rinses electrodes. No mandatory rinse button for normal classroom use.
- Diagnostic checklist visibly separates **unready circuit** from **ready circuit with a nonconductive solution**.
- Chemistry interactions remain meaningful: connect circuit, submerge electrodes and turn on power; test red/blue litmus; student chooses their own classification before recording.
- Drag chemical cards onto the 3D viewport to select a sample; clicking 3D rinse station resets electrodes; other 3D equipment and fallback buttons retained.
- Notebook keeps independent repeat records, CSV export, 12 chemicals, molecular view, dual comparison and mystery challenge.

## Limitations and honest scope
The main 3D scene still uses procedural low-to-medium-poly meshes; **not yet fully photorealistic**. Animated liquid has simplified motion. Dragging a reagent card to select is not realistic pouring physics. 3D interactions need browser/device testing, including CDN and WebGL support. Chemistry calculations are qualitative/idealized and signal is relative, not a calibrated conductivity measurement. No teacher accounts or Sheets connection (Phase 4 excluded). Development tests do not validate the model against physical laboratory data.

## GitHub Pages deployment
Upload the **contents** of this folder into a new repo; Settings → Pages → Deploy from branch → main /(root). Do not upload only the ZIP. If updating an older deployment, hard refresh to avoid old cached modules. Deploying to your existing repository changes that public site; preserve backup first.
