# Denton Bonsai Lady Tracker

![GIS](https://img.shields.io/badge/GIS-ArcGIS%20Online-blue)
![Data Collection](https://img.shields.io/badge/Data-Crowdsourced-green)
![Mapping](https://img.shields.io/badge/Web%20Map-Interactive-orange)
![Status](https://img.shields.io/badge/status-prototype-yellow)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

A crowdsourced geospatial reporting system that allows residents of Denton, Texas to report the last known location of a mobile bonsai tree seller.

The application uses ArcGIS Online tools to collect, moderate, and visualize sightings on an interactive map.


## Purpose

This project demonstrates how cloud GIS platforms can be used to build lightweight community reporting tools with real-time spatial visualization.

## Technologies Used

- ArcGIS Online
- Survey123
- Hosted Feature Layers
- ArcGIS Web Maps
- ArcGIS Dashboards
- ArcGIS Experience Builder (optional)

## System Architecture

User reports a sighting through Survey123.  
Submissions are stored in a hosted feature layer and reviewed by a moderator.  
Approved sightings are displayed on a public web map and dashboard.

See architecture diagram below.

![Architecture](docs/architecture_diagram.png)

## Workflow

1. User submits a sighting using Survey123
2. Submission enters the feature layer as **pending**
3. Moderator reviews the submission
4. Approved sightings appear on the public map
5. Dashboard updates with the latest location

## Feature Layer Schema

| Field | Type | Description |
|------|------|-------------|
| sighting_date | Date | Date/time bonsai seller was seen |
| location_name | Text | Description of location |
| notes | Text | Additional information |
| approved | Integer | Moderation flag |
| submitted_time | Date | Time report was submitted |

## Key GIS Concepts Demonstrated

- Crowdsourced spatial data collection
- Moderated public data submission
- Real-time geospatial dashboards
- Hosted feature layer design
- Spatial filtering and visualization

## Future Improvements

- Reddit posting integration
- Heatmap of common selling locations
- Confidence scoring from multiple reports
- Mobile-first ArcGIS Experience Builder interface
- Automated expiration of old sightings

## Project Status

Active prototype.
