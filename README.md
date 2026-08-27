# LightBridge Frame Scanner

Private/internal barcode price lookup tool for eyewear inventory.

## Current pricing rules

- Eyeglass Frames: Unit Price × 3.00
- Sunglasses: Unit Price × 2.75

## Run with GitHub Pages

1. Create a new GitHub repository named `lightbridge-frame-scanner`.
2. Upload all files in this folder to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose the `main` branch and `/ (root)`, then save.
6. GitHub will provide an HTTPS Pages link.

The phone camera only works reliably when the page is served over HTTPS.

## Important barcode test

The app currently looks up the scanned value against the `Code` field from the Safilo packing-list inventory.

If the physical Safilo barcode encodes a UPC/SKU instead of this Code, add a barcode/UPC mapping column and update the app database accordingly.

## Files

- `index.html` — scanner web app
- `inventory.csv` — current 75-item inventory
- `.nojekyll` — keeps GitHub Pages deployment simple

## Privacy

This tool is intended for inventory data only. Do not store patient information in this repository.
