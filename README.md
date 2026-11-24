# 764 Tremont St · Unit 4 — 3D furnishing planner

An interactive 3D model of a 2-bed, 1-bath corner unit (~752 sq ft) in Boston's South End, for trying out furniture layouts.

The rooms are traced from the listing photos. There's no official floor plan, so the dimensions are estimates.

## Use it
- Pick a piece from the catalog on the left to place it. Furniture comes in standard real-world sizes.
- Drag furniture to move it.
- `Q` / `E` rotate 15°, `R` turns 90°, `D` duplicates, `Delete` removes.
- Drag empty floor to orbit, scroll to zoom, and right-drag to pan.
- Switch between the **3D**, **Plan** and **Eye level** views, and between **Cutaway** and **Full walls**.

Your layout saves in your browser's local storage, so it's per-device.

## Run locally
Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

Everything is in `index.html`: plain HTML, CSS and JS, with three.js loaded from a CDN. To change the floor plan, edit the `WALLS` array, the `floorShape(...)` calls and the fixtures. Coordinates are in feet: the street side is z = 0, and the unit spans x 0–23 and z 0–32.
