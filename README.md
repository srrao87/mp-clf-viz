# Women's Economic Empowerment Partners' Forum Dashboard

## Dashboard overview

This repository contains a complete static dashboard for the Gates Foundation Women's Economic Empowerment Partners' Forum. It is designed for State Rural Livelihoods Missions, Gates Foundation staff, and Gates Foundation-funded partners, and runs entirely from static HTML, CSS, JavaScript, CSV, and GeoJSON files with no backend or build step.

## Exact repository file structure

```text
/
├── index.html
├── README.md
├── .nojekyll
├── css/
│   └── styles.css
├── js/
│   ├── app.js
│   ├── config.js
│   ├── data-loader.js
│   ├── filters.js
│   ├── maps.js
│   ├── tables.js
│   └── utils.js
└── data/
    ├── state_metadata.csv
    ├── district_name_crosswalk.csv
    ├── clf_lists/
    │   ├── assam.csv
    │   ├── bihar.csv
    │   ├── chhattisgarh.csv
    │   ├── jharkhand.csv
    │   ├── madhya-pradesh.csv
    │   ├── odisha.csv
    │   └── uttar-pradesh.csv
    └── geojson/
        ├── india_states.geojson
        └── districts/
            ├── assam.geojson
            ├── bihar.geojson
            ├── chhattisgarh.geojson
            ├── jharkhand.geojson
            ├── madhya-pradesh.geojson
            ├── odisha.geojson
            └── uttar-pradesh.geojson
```

## Exact step-by-step GitHub Pages deployment instructions

1. Create a new GitHub repository in your GitHub account.
2. Open the new repository and choose the option to upload files.
3. Upload the complete generated folder structure exactly as created: `index.html`, `README.md`, `.nojekyll`, `css/`, `js/`, and `data/`.
4. Confirm that the repository root contains `index.html` directly at the top level.
5. Commit the uploaded files to the `main` branch.
6. Open the repository **Settings** tab.
7. In the left-side settings menu, open **Pages**.
8. Under **Build and deployment**, choose **Deploy from a branch**.
9. Under **Branch**, select `main`.
10. Under **Folder**, select `/ root`.
11. Click **Save**.
12. Wait for GitHub Pages to publish the site.
13. Once publishing is complete, open the published GitHub Pages URL shown in the Pages settings.

## Troubleshooting

- If the page is blank, confirm that `index.html` is in the repository root and that GitHub Pages is publishing from `main` and `/ root`.
- If maps are not loading, confirm that the `data/geojson/` files are present in the deployed repository and that the published site can load CDN assets for Leaflet.
- If CSV data is not loading, confirm that the `data/clf_lists/` files and `data/state_metadata.csv` are present in the deployed repository and that the published site can load PapaParse from its CDN.

## Public access note

Anything uploaded to GitHub Pages is publicly accessible, including the CSV and GeoJSON files used by the dashboard.
