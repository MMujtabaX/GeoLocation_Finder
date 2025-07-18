# 🌍 OpenGeo Location Mapper

This project retrieves geolocation data for a list of addresses using a web API and stores the results in an SQLite database. It then converts that data into a JavaScript file which can be visualized on a map using `where.html`.

![Map Visualization Demo](https://assets.grab.com/wp-content/uploads/sites/4/2023/02/13123441/exploredata.gif) ![](https://i.gifer.com/DD6E.gif)
<!-- Replace this GIF with a screen recording of your actual project if available -->

---

## 📁 Project Structure

- `geoload.py`: Reads addresses from `where.data`, fetches their geolocation from the OpenGeo API, and saves responses into `opengeo.sqlite`.
- `geodump.py`: Extracts geolocation data from `opengeo.sqlite` and creates `where.js` for map visualization.
- `where.html`: Displays the geolocation points on a map (requires internet access for Leaflet or similar libraries).
- `where.data`: A plain text file containing one address per line (sample input).
- `where.js`: Generated output file containing coordinates and location names.

---

## 🛠 How to Run

### 1. Requirements
Make sure you have:
- Python 3.x
- Internet access (for retrieving data via API)

### 2. Install Required Libraries
These are standard libraries; no installation required:
```bash
urllib, sqlite3, json, ssl, codecs, time
