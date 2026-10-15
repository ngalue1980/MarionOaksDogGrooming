# Marion Oaks Dog Grooming — Browser Pricing Manager

A free, static, GitHub Pages-ready pricing manager. Add/edit/delete grooming services, hide services, edit promotions, preview a branded menu, and export a printable PDF using the browser's **Print → Save as PDF** option. No Python or server required.

## Publish to GitHub Pages

1. Create a **public** GitHub repository (e.g. `MarionOaksDogGrooming-Pricing`).
2. Upload **index.html**, **style.css**, **app.js**, and this README.md to the repository root (not inside a subfolder).
3. In the repository, open **Settings → Pages → Build and deployment**.
4. Select **Deploy from a branch**, choose **main**, folder **/(root)**, and save.
5. Visit `https://YOUR-USERNAME.github.io/MarionOaksDogGrooming-Pricing/` after publishing completes.

## Using the app

- Add a service using the editor; click **Edit** on any row to change its price or visibility.
- Change business details and click **Save business details**.
- Click **Export PDF menu**, choose **Save as PDF** in the browser print destination, select Letter paper, and enable **Background graphics** if your browser offers that setting. The printed menu can flow across multiple pages for long service lists.
- Click **Download database backup** to save your services and settings as JSON. Use **Restore JSON backup** to import it on another browser/device.

## Important storage and security limitations

This version uses the browser's **IndexedDB** database. It is **not** an online/shared database. Each browser/device has its own independent data; clearing site data or using private browsing can delete it. GitHub stores and hosts only the application code, not your price changes. Export backups regularly. No admin login is provided; anyone visiting your public URL can edit **their own local copy**, but cannot edit your data on your browser or change your GitHub files. Do not store customer personal information here.

For shared prices across multiple devices, add an authenticated hosted database (such as Supabase with Row Level Security) as a future upgrade.

## Run locally

Open `index.html` in a modern browser. If your browser blocks local-file storage, use a local server (for example `python -m http.server 8000`) and visit `http://localhost:8000`.

## License

For Marion Oaks Dog Grooming business use.
