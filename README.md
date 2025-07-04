# DisasterAware 

**DisasterAware** is a smart disaster relief zone locator built to assist communities in quickly identifying the nearest active relief centers during emergencies such as floods, earthquakes, and urban fires.

##  Objective

India faces several disasters annually, where timely access to aid can save lives. DisasterAware empowers citizens and volunteers by helping them locate nearby relief centers instantly using location data. This initiative not only supports emergency navigation but also promotes community engagement in crisis management.

##  Overview

This web application allows users to:
- Enter their name and PIN code
- View the five closest relief centers near them
- Choose between a map-based view or a detailed list

It uses a `.CSV` file containing a list of relief center locations across a city and leverages geographic routing libraries to determine proximity and shortest paths.

##  How It Works

1. User enters their **Name** and **PIN Code** in a simple form.
2. Application displays:
   -  **Map View:** A visual map with markers for the nearest 5 centers
   -  **List View:** A sortable list of centers with useful details
3. Users can click on a relief center to view the shortest route from their location.

The backend logic uses Dijkstra’s algorithm to calculate the most efficient travel route.

##  Technologies Used

- Python
- Flask
- Folium
- NetworkX
- OSMnx
- Geopy

## Running the Project Locally

Install dependencies:

```bash
pip install flask networkx osmnx geopy folium

