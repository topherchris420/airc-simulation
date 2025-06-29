# AIRC System Simulation

An interactive, browser-based simulation of an Adaptive Ionospheric Resonance Control (AIRC) system designed to optimize plasma coherence against environmental disturbances.

[![GitHub Pages Deploy](https://img.shields.io/github/deployments/YOUR-USERNAME/YOUR-REPO-NAME/github-pages?label=Live%20Demo&style=for-the-badge)](https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

---

**➡️ [View the Live Demo](https://topherchris420.github.io/airc-simulation/) ⬅️**

*(Replace the links above with your actual GitHub username and repository name)*

![AIRC Simulation Screenshot](https://i.imgur.com/rL4z1Qk.png)
*(Pro-tip: Run the simulation, take a screenshot, and replace the image link above to show off your project!)*

## About The Simulation

This project simulates a sophisticated control system tasked with maintaining a stable and coherent ionospheric plasma region. The simulation is built entirely in vanilla JavaScript and rendered using the HTML5 Canvas API.

The core objective of the AIRC system is to maximize the **Coherence Index (J)** across the spatial grid. It achieves this by continuously adjusting a **Control Vector Field (u)** using a gradient ascent optimization algorithm.

The simulation introduces a challenge at T=5.00 minutes: a **Traveling Ionospheric Disturbance (TID)**, which the AIRC system must actively counteract to restore coherence. The system's performance and key metrics are visualized in real-time.

## Features

-   **Real-time Visualizations:** Four distinct canvas plots show the Electron Density, Coherence Index, Control Vector Field, and Convergence of the optimization algorithm.
-   **Interactive Controls:** Start, pause, resume, and reset the simulation state.
-   **Dynamic Event Modeling:** A Traveling Ionospheric Disturbance (TID) is introduced mid-simulation to test the adaptive controls.
-   **Complex System Metrics:** Track the overall coherence, control magnitude, gradient norm, and active cyclotron resonance harmonics.
-   **Data Export:** Download the final simulation metrics and history as a JSON file at any time.
-   **Event Log:** See a running log of key system events, warnings, and successes.
-   **Modern UI:** A clean, responsive interface with a "glassmorphism" aesthetic.

## Technologies Used

-   **HTML5:** Provides the structure for the simulation dashboard.
-   **CSS3:** Powers the modern, responsive layout using Flexbox, Grid, and custom properties for styling.
-   **Vanilla JavaScript (ES6+):** All simulation logic, physics modeling, and rendering are handled with plain JavaScript, organized into an `AIRCSimulation` class. The HTML Canvas API is used for all visualizations.

## How to Use the Live Demo

1.  **Start Simulation:** Begins the AIRC optimization process.
2.  **Pause / Resume:** Freezes the simulation at its current state for inspection.
3.  **Reset:** Returns the simulation to its initial baseline conditions.
4.  **Export Data:** Downloads a `.json` file containing the complete simulation history.
5.  **Observe:** Watch how the control system responds to the introduction of the TID and works to maximize the coherence index `J`.

## Running Locally for Development

To run this project on your local machine:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git)
    ```

2.  **Navigate to the directory:**
    ```bash
    cd YOUR-REPO-NAME
    ```

3.  **Open the file:**
    Simply open the `index.html` file in your web browser. For the best experience, use a local web server. If you use Visual Studio Code, the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension is an excellent choice.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments

-   The simulation initializes with a simplified electron density profile inspired by the **International Reference Ionosphere (IRI) model**.
-   The project serves as a practical example of implementing a model-based control system and real-time data visualization in a web environment.
