*Team Name-* Quasar Tag

*Team Leader-* Aditya Kumar eakadityakumar15@gmail.com

*NasaSpaceApps2024 Challenge-* Create an Orrery Web App that Displays Near-Earth Objects


# orrery
An interactive map of the Solar System created with Three.js and jQuery.

It's definitely better as a desktop web experience than mobile in the current version.

![image](https://github.com/user-attachments/assets/83d9f44e-8de3-4719-b74d-92a6a3767b47)
![Screenshot 2024-10-06 102602](https://github.com/user-attachments/assets/15a9fbba-c9ac-4bbc-b1dc-9eda395a31f6)



## Requirements
- [Three.js](https://github.com/mrdoob/three.js/)
- [jQuery](https://github.com/jquery/jquery) and [jQuery UI](https://github.com/jquery/jquery-ui)
- [Tween.js](https://github.com/tweenjs/tween.js/)

## Features
- Ephemerides for astronomical bodies in the Solar System, searachable for all above 1km in radius 
- Exaggerated orrery view at the solar system scale, zoomable to true scale for planetary systems
- Live data readout for the body's physical and orbital characteristics, right ascension/declination and altitude/azimuth coordinates relative to current location, rise and set times, and magnitude adjusted for atmospheric dispersion
- Links to articles and images from Wikipedia
- Background stars include all above 7th magnitude
- HTTPvars for latitiude/longitude, start time, and reducing particle count

## Setup
- npm init
- npm i three-js

## Usage
### Navigation
- SPACE BAR: Pause/resume time
- LEFT/RIGHT ARROW KEYS: Change speed
- DOWN ARROW KEY: Set to current time
- UP ARROW KEY: Toggle chase mode on focused object
- ESC: Release focus on object
- F2: Hide/show UI panels
- F4: Hide/show celestial sphere
- F8: Hide/show extra time info
- CLICK ON LABELS: Shift focus to object and display info
- CLICK ON INFO HEADER OR IMAGE: Learn more on Wikipedia
- LEFT/MID/RIGHT MOUSE + DRAG: Rotate/zoom/translate around focus
- SCROLL WHEEL: Zoom to focus
### HTTP Variables
- ?x=(decimal degrees): Longitude
- ?y=(decimal degrees): Latitude
- ?t=(YYYYMMDDHHMM): Date (Years can be -9999 to 9999, time in military time format, e.g. 0615)
- ?n=(integer) Small asteroid limit

## Potential Roadmap
- UI scaling for mobile
- Object count throttling from FPS observation
- Non-periodic comets/hyperbolic orbits (`Omuamua, etc.)
- Extended data/add ins for smaller objects
- Planetarium view with sky shader
- Asteroid categorization from orbital elements
- Asteroid 3D shapes
- Ring shadows
- Spacecraft/Two Line Element reader
- NASA SPICE kernels
- Better image compression (Basis)
- THREE.CSS2D renderer or Canvas for tags (if faster)
- Procedural textures
- Exoplanetary systems
- Lagrange points/Hill spheres for planets
- XR
- Hohmann transfer orbits, launch window solver, delta-v requirements
- Gravitational simulations
- Compute shaders
