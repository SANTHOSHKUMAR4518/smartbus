# SmartBus — Transit Safety Simulator

React + TypeScript + Vite starter with an interactive 3D bus, passenger simulation, safety alerts, illustrative route/ETA, sensor inspector, event log, and Render deployment configuration.

## Important scope
- Phase 1 is simulation-only. No physical sensors, GPS, ESP32, buzzer, or vehicle door is connected.
- Route, coordinates, speed and ETA are illustrative, not live transit data.
- No ticketing, QR passes, UPI or payment features.
- Never connect this demo to real vehicle door controls or safety-critical hardware.

## Requirements
Node.js 20.19+ or 22.12+ recommended, npm, and a modern browser with WebGL enabled.

## Run locally
1. Extract the ZIP.
2. Open a terminal in this folder.
3. Run `npm install`
4. Run `npm run dev`
5. Open the localhost URL shown in the terminal.

## Build check
Run `npm run build`. Then `npm run preview` to inspect the production build locally.

## Render deployment
1. Push this project to a GitHub repository.
2. On Render choose **New + → Static Site** and connect the repository.
3. Build command: `npm install && npm run build`
4. Publish directory: `dist`
5. Deploy. The included `render.yaml` shows the same settings.

## Features
- Responsive dark dashboard with cyan accents
- Interactive 3D bus: drag to rotate, scroll to zoom, click sensor components
- Passenger entry/exit controls and occupancy thresholds
- Footboard obstruction alert, GPS loss and network loss simulation
- Illustrative demo route and ETA state
- Auto demo, event log, reset, and system info

## First-version limitations
- Passenger direction counting is represented by simulation controls, not physical ToF signal processing.
- Door animation is visual only and not connected to a real actuator.
- Coordinates, speed and ETA are synthetic.
- Hardware integration is future work; this starter does not connect to an ESP32.
- State resets on refresh because this version is frontend-only.
