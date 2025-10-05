# HandWind-Sim
A real-time, web-based cloth simulation framework with gesture-driven wind interaction.

<br>

<p align="left">
  <img width="340" alt="Fig2" src="https://github.com/user-attachments/assets/06f71d97-75c4-4ff9-89fc-88e6fe8758d0"> <img width="340" alt="Fig6" src="https://github.com/user-attachments/assets/7fd3cce0-91ab-4736-8d03-aa46c4b8a718">
<br>

<br>

## Overview

HandWind-Sim is an interactive framework that recognizes user hand gestures via a standard webcam to interact with a 3D cloth simulation in real-time, directly in the browser. This project aims to increase the accessibility of complex physics-based interactions for applications in HCI research, interactive art, and virtual prototyping.

<br>

## Features

- **🖥️ Real-time Web Simulation:** Provides a real-time cloth simulation that runs directly in modern web browsers without any installation required.
- **👋 Intuitive Gesture Interaction:** Recognizes user hand movements via a standard webcam and translates them into an intuitive wind vector to control the simulation.
- **📊 Interactive Visual Feedback:** Offers a visual feedback system for the generated wind (direction and strength) and the tracked hand position, providing an immersive and understandable experience.

<br>

## How It Works (Architecture)

HandWind-Sim utilizes a pipeline architecture where modules for gesture input, physics simulation, and rendering are organically connected.

<img width="1191" height="237" alt="Fig0" src="https://github.com/user-attachments/assets/aa262320-f70b-4c73-8200-6ecace3787bc" />

1.  **Gesture Input & Processing:** Extracts hand landmarks from the webcam video stream using MediaPipe and analyzes the movement to generate a wind vector.
2.  **Physics Simulation:** Simulates the deformation of the cloth mesh based on the generated wind vector and physical constraints, using a Position-Based Dynamics (PBD) algorithm.
3.  **Rendering & Visualization:** Renders all 3D elements, including the deformed cloth, tracked hand, and wind effects, using Three.js to provide visual feedback to the user.

<br>

## Requirements

-   A modern web browser with WebGL support (e.g., Chrome, Firefox, Edge).
-   A webcam.

<br>

## Installation

1.  Clone this repository:
2.  Navigate to the project directory:
3.  Open the `index.html` file in your web browser.
    -   For the best experience and to avoid potential browser security issues with local files, it is recommended to use a local server. A simple way is to use an extension like **Live Server** in Visual Studio Code.

<br>

## Demo Video
![Fig1](https://github.com/user-attachments/assets/188855a2-86da-4627-bc87-f12cca555d81)

![HandWind-Sim Demo](https://github.com/user-attachments/assets/4017bba7-7ec9-4588-b225-db669c4f1832)

See HandWind-Sim in action.

<br>

## Acknowledgements

-   The cloth simulation physics is based on the work of Matthias Müller et al. on Position-Based Dynamics.
-   Hand tracking is powered by Google's [MediaPipe](https://google.github.io/mediapipe/).
-   3D rendering is done with the amazing [Three.js](https://threejs.org/) library.
