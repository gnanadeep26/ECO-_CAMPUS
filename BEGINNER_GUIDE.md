# Beginner Guide — EcoCampus

## Project title
AI-Powered Sustainable Campus: A Digital Twin for Monitoring Waste, Water, and Energy

## Problem
College campuses can waste resources when bins overflow, water systems behave abnormally, or electricity is used unnecessarily. Manual inspection alone may not provide a clear, unified overview.

## Proposed solution
A web dashboard represents a sample campus digitally. It displays simulated sensor values, uses simple thresholds to flag issues, and generates an action-oriented sustainability report.

## Key terms
- **AI (Artificial Intelligence):** Methods that help computers perform tasks such as recognizing patterns or classifying images.
- **Digital Twin:** A digital representation of a physical place or system, updated with data from that system. In this demo, the map and data are simulated.
- **Computer Vision:** AI techniques that interpret images or video. The current version does not run a vision model; this is a future module.
- **Sensor data:** Measurements from devices such as water-flow meters or bin-level sensors. This version simulates the values.
- **GenAI:** Generative AI that creates text, summaries, or other content. The current report is template/rule-based, not a live GenAI API.
- **Sustainability:** Using resources responsibly while reducing environmental impact.
- **Actionable recommendation:** A practical next step someone can take, such as inspecting a pipe after unusual flow is detected.

## Run the project
1. Extract the ZIP file.
2. Open `index.html` in a browser.
3. Use the sliders to change the sample readings.
4. Select campus buildings on the map.
5. Watch the alerts and status colors update.
6. Click **Generate report** to see a summary.
7. Click **Reset demo** to restore the original values.

## How the prototype works
1. Sliders represent simulated sensor readings.
2. JavaScript compares readings with demo thresholds.
3. The campus map changes location colors.
4. Alerts explain the detected condition.
5. A report template summarizes current readings and suggests actions.

## Example thresholds
- Bin fill at or above 80% -> arrange collection.
- Water flow at or above 15 L/min -> inspect for possible leakage.
- Energy at or above 180 kWh -> review use.

These values are for the demonstration only and are not universal engineering limits.

## Suggested presentation/demo script
“Good morning. Our project is EcoCampus, an AI-powered sustainable campus concept. The dashboard shows a digital representation of selected campus locations. In this prototype we use simulated readings because we do not have physical sensors yet. If I increase the canteen bin level above the demo threshold, the map changes status and a waste alert appears. If I change the water flow, the system can recommend inspecting the plumbing. The report summarizes the current readings and suggests next steps. The present report is rule-based; connecting a real GenAI service and validated sensors is future work. Our goal is to help campus teams identify issues earlier and use resources more responsibly.”

## What to say honestly
- Current version: interactive front-end, simulated data, rule-based detection, report template.
- Not yet implemented: real camera-based computer vision, real IoT sensors, persistent database, live GenAI API.
- Do not claim measured savings or real-world accuracy from simulated data.

## Development roadmap
Phase 1: Demonstrate the browser prototype.
Phase 2: Add image upload and a tested computer-vision model.
Phase 3: Connect sensor hardware and a backend.
Phase 4: Save historical readings and generate trends.
Phase 5: Connect a GenAI API with safeguards and source data.
Phase 6: Pilot in one campus area, validate alerts, and measure outcomes.
