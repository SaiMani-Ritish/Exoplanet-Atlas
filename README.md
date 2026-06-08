# Exoplanet Atlas 🌌

An interactive visualization of confirmed exoplanets from NASA's Exoplanet Archive, arranged by estimated atmospheric hue and rendered as a cosmic atlas of worlds.

## Overview

Exoplanet Atlas transforms thousands of discovered exoplanets into a visually explorable universe. Each planet is represented as a stylized globe whose:

* **Color (Hue)** reflects estimated atmospheric or equilibrium temperature
* **Size** reflects planetary radius
* **Position** groups planets along a temperature-based color spectrum
* **Tooltip** reveals scientific properties and discovery information

The project combines astronomy data with generative visualization techniques to create an engaging way to explore exoplanet discoveries.

## Features

### Interactive Visualization

* Canvas-based rendering for thousands of planets
* Animated starfield background
* Hover tooltips with planet details
* Responsive layout

### NASA Data Integration

* Live data from NASA Exoplanet Archive
* Automatically loads confirmed exoplanets
* Displays:

  * Planet name
  * Host star
  * Radius
  * Mass
  * Orbital period
  * Distance from Earth
  * Discovery year
  * Discovery method

### Filtering & Search

Filter planets by discovery method:

* Transit
* Radial Velocity
* Direct Imaging
* Microlensing
* Astrometry

Search planets by name using the built-in search box.

### Visual Encoding

| Attribute               | Visualization          |
| ----------------------- | ---------------------- |
| Equilibrium Temperature | Planet Hue             |
| Planet Radius           | Planet Size            |
| Planet Type             | Tooltip Classification |
| Discovery Method        | Filter Controls        |

### Automatic Planet Classification

The visualization categorizes planets into:

* Rocky / Earth-like
* Super-Earth
* Sub-Neptune
* Neptune-class
* Gas Giant
* Unknown

## Technology Stack

* HTML5
* CSS3
* Vanilla JavaScript
* Canvas API
* NASA Exoplanet Archive API

No external frameworks are required.

## Data Source

Data is retrieved from:

**NASA Exoplanet Archive**
[https://exoplanetarchive.ipac.caltech.edu](https://exoplanetarchive.ipac.caltech.edu)

Fields used include:

* Planet Name
* Host Star
* Discovery Year
* Discovery Method
* Radius
* Mass
* Orbital Period
* Distance
* Stellar Temperature
* Equilibrium Temperature

## How Planet Colors Are Generated

The atlas estimates atmospheric appearance using equilibrium temperature:

* Blue → Cold / Ice worlds
* Cyan → Temperate worlds
* Green → Mild atmospheres
* Yellow → Warm worlds
* Orange → Hot planets
* Red → Extreme lava worlds

These colors are artistic approximations intended for exploration and visual storytelling rather than scientific atmospheric modeling.

## Fallback Mode

If the NASA API is unavailable:

* A synthetic demo dataset is generated
* Core visualization remains functional
* User experience is preserved

## Running the Project

### Option 1: Open Directly

Simply open:

```bash
exoplanet_atlas_hue_universe.html
```

in a modern browser.

### Option 2: Serve Locally

```bash
python -m http.server 8000
```

Then navigate to:

```text
http://localhost:8000
```

## Browser Support

Recommended browsers:

* Google Chrome
* Microsoft Edge
* Firefox
* Safari

Requires support for:

* ES6 JavaScript
* Fetch API
* HTML5 Canvas

## Future Enhancements

Potential improvements:

* Zoom and pan navigation
* Planetary system grouping
* 3D WebGL rendering
* Habitability indicators
* Distance scaling modes
* Discovery timeline animation
* Exportable screenshots
* Additional NASA datasets

## License

This project is intended for educational, visualization, and astronomy exploration purposes.

Exoplanet data is provided by NASA's Exoplanet Archive.

---

**Author:** Mani Ritish
**Project:** Exoplanet Atlas – Hue Universe Visualization
**Version:** 1.0.0
