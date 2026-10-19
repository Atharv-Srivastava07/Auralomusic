AURALO PWA DEPLOYMENT

1. Upload these files to the ROOT of your existing GitHub repository, replacing the old HTML file with index.html:
   - index.html
   - manifest.json
   - service-worker.js
   - icon.svg
2. Commit the changes. Vercel should redeploy automatically.
3. Open the deployed HTTPS URL and refresh once.
4. Install from your browser's install option (Chrome/Edge: install icon/menu; iPhone/iPad Safari: Share > Add to Home Screen).

IMPORTANT LIMITATIONS
- This caches the app shell and same-origin files for basic offline startup. It does NOT make online music streams available offline.
- Songs saved by the existing app are stored in that browser's local IndexedDB; they are not automatically synced across devices.
- SVG icon support varies across install surfaces. If a platform requires PNG icons, create 192x192 and 512x512 PNGs and add them to manifest.json.
- Keep all four files at the repository root, not inside a subfolder.
