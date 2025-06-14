# CPI Bangladesh Mission Map

Interactive web map displaying administrative boundaries and placemarks for CPI Bangladesh Mission.
Setup Instructions

Clone the Repository (optional for local testing):
git clone https://github.com/your-username/cpi-bangladesh-map.git
cd cpi-bangladesh-map


## Verify Files:

Ensure all GeoJSON files (level0.geojson to level7.geojson), JSON metadata files (level0.json to level7.json), and placemark files (camps.json, cpi_office.json) are in assets/data/.
Confirm logo PNG files (cpi_logo.png, health.png, sustainable.png, research.png, emergency.png, logo1.png to logo12.png) are in assets/logos/.
Confirm icon ICO files (icon1.ico to icon15.ico) are in assets/icons/.


## Install Dependencies:

No local dependencies are required as the project uses CDN-hosted libraries (Vue 3, MapLibre GL JS, Bootstrap 5).



## Deployment

Local Testing:

Start a local server:python -m http.server 8000


Open http://localhost:8000 in a browser.


## GitHub Pages Deployment:

Go to Settings > Pages in the repository.
Under Branch, select main and / (root), then click Save.
Access the deployed map at https://your-username.github.io/cpi-bangladesh-map/.



## Features

Interactive map with zoom/pan controls
3D terrain visualization
OSM/Satellite/Topography basemap switching
Multi-select filters for District (level2), Upazila (level3), and CPI Office
Layer toggle panel for admin levels (0-7)
Custom placemarks with ICO icons
Metadata popups with logos
Mobile-responsive design
Reset button to restore initial view

## Notes

Ensure GeoJSON files are valid and contain feature_id and parent_id properties.
Metadata JSON files (level0.json to level7.json) should include feature_id, name, thematics_program, description, and logo_id.
Placemark JSON files (camps.json, cpi_office.json) should include name, place_id, type, and icon_id.
The map initializes with Level 0 and Level 1 visible.
Logos auto-size within popups.
If any file exceeds GitHub's 25 MB upload limit, use Git CLI or GitHub Desktop to upload.

## Project Structure
```plaintext
cpi-bangladesh-map/
├── assets/
│   ├── data/
│   │   ├── level0.geojson
│   │   ├── level0.json
│   │   ├── level1.geojson
│   │   ├── level1.json
│   │   ├── level2.geojson
│   │   ├── level2.json
│   │   ├── level3.geojson
│   │   ├── level3.json
│   │   ├── level4.geojson
│   │   ├── level4.json
│   │   ├── level5.geojson
│   │   ├── level5.json
│   │   ├── level6.geojson
│   │   ├── level6.json
│   │   ├── level7.geojson
│   │   ├── level7.json
│   │   ├── camps.json
│   │   └── cpi_office.json
│   ├── logos/
│   │   ├── cpi_logo.png
│   │   ├── health.png
│   │   ├── sustainable.png
│   │   ├── research.png
│   │   ├── emergency.png
│   │   ├── logo1.png
│   │   ├── logo2.png
│   │   ├── logo3.png
│   │   ├── logo4.png
│   │   ├── logo5.png
│   │   ├── logo6.png
│   │   ├── logo7.png
│   │   ├── logo8.png
│   │   ├── logo9.png
│   │   ├── logo10.png
│   │   ├── logo11.png
│   │   └── logo12.png
│   └── icons/
│       ├── icon1.ico
│       ├── icon2.ico
│       ├── icon3.ico
│       ├── icon4.ico
│       ├── icon5.ico
│       ├── icon6.ico
│       ├── icon7.ico
│       ├── icon8.ico
│       ├── icon9.ico
│       ├── icon10.ico
│       ├── icon11.ico
│       ├── icon12.ico
│       ├── icon13.ico
│       ├── icon14.ico
│       └── icon15.ico
├── index.html
└── README.md





