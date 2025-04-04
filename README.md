# Field Lines Simulation

A visually engaging particle simulation built with Three.js, visualizing abstract field lines emanating from a central source.

**Live Demo:** https://bytetrooper.github.io/Field-Lines-Simulation/

![image](https://github.com/user-attachments/assets/7a9de9b0-06fb-4e23-9bb7-38389c272f58)

## Description

This interactive web experience displays a central glowing sphere surrounded by numerous particles tracing curved paths. These paths visually represent abstract field lines, similar in appearance to magnetic or gravitational fields. Users can manipulate various parameters of the simulation in real-time using a control panel, altering the appearance of the field lines, particles, and visual effects.

## Features

* **Central Source:** A configurable sphere (wireframe or solid color) at the center.
* **Particle Field Lines:** Thousands of particles rendered as points (`THREE.Points`) trace smooth, curved paths around the central sphere.
* **Interactive Controls:** A GUI panel (using `lil-gui`) allows modification of:
    * Number of field lines
    * Density of points per line
    * Overall strength/spread of the field
    * Particle size and color
    * Central sphere color and wireframe toggle
    * Bloom post-processing effect intensity, threshold, and radius
* **3D Navigation:** Uses `OrbitControls` to allow users to rotate, pan, and zoom the scene.
* **Visual Effects:** Implements `UnrealBloomPass` for a glowing, ethereal aesthetic.
* **Responsive:** Adapts to different window sizes.

## Controls

The control panel allows you to adjust the simulation's parameters:

* **Field Lines:**
    * `Number of Lines`: Controls how many distinct field lines are generated.
    * `Points per Line`: Sets the number of particles used to draw each line. Higher values create smoother lines but impact performance.
    * `Field Strength`: Adjusts the overall size and curvature of the field lines.
* **Appearance:**
    * `Particle Size`: Changes the size of the individual particles.
    * `Particle Color`: Sets the color of the field line particles.
    * `Sphere Color`: Sets the color of the central sphere.
    * `Sphere Wireframe`: Toggles the wireframe view for the central sphere.
* **Bloom Effect:**
    * `Bloom Strength`: Controls the intensity of the glow effect.
    * `Bloom Threshold`: Adjusts the brightness threshold for pixels to contribute to the bloom. Lower values make more things glow.
    * `Bloom Radius`: Controls the spread or blurriness of the glow.

## Technology Used

* [Three.js](https://threejs.org/): A comprehensive 3D graphics library for creating and displaying animated 3D computer graphics in a web browser.
* [lil-gui](https://github.com/georgealways/lil-gui): A lightweight graphical user interface library.
* HTML, CSS, JavaScript

