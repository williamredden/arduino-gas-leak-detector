# Arduino Gas Leak Detection System
An embedded system using an MQ-5 sensor and Arduino to detect LPG, methane, hydrogen, and natural gas, triggering visual and audio alerts for safety monitoring.

## Demo

▶️ Full system demonstration; Portable Gas Leak Detection System (Arduino): https://youtu.be/uWade8Qd0Jg?si=SRWCj3aXiakNgnTq

The video shows the system's baseline state, then controlled gas exposure via a lighter that causes LED activation and buzzer alert behavior.

## Inputs and Outputs

### Inputs
- MQ-5 gas sensor (digital threshold output indicating gas presence)
- Power input (USB or 9V battery)

### Outputs
- LED indicator (visual alert when gas is detected)
- Buzzer (audible alert when gas exceeds threshold)
- Serial monitor output (real-time sensor readings used for debugging, calibration, and verification)

## Design Notes
- The MQ-5 sensor’s onboard comparator was used to provide a digital threshold signal, simplifying detection logic.
- Threshold sensitivity was tuned to balance responsiveness and false positives.
- System behavior was verified using both physical outputs and serial monitor readings.
Yes 👍 — this is exactly the right place for it, and the flow is correct.

Recommended README flow (what you have + what comes next)

Your current structure:

Project title + overview ✅

Demo (video link + explanation) ✅

Inputs and Outputs ✅

Design Notes ✅

➡️ Next section should be the Images & Documentation section
This is where your schematic, physical layout, and test screenshots belong.

✅ Final recommended order (clean + professional)

Paste the Images & Documentation section directly after ## Design Notes.

Here is the final flow:

## Design Notes
- The MQ-5 sensor’s onboard comparator was used to provide a digital threshold signal, simplifying detection logic.
- Threshold sensitivity was tuned to balance responsiveness and false positives.
- System behavior was verified using both physical outputs and serial monitor readings.

## 📷 Images & Documentation

This repository includes schematic documentation, physical hardware verification, and operational test results to demonstrate correct system design and functionality.

### 🔌 Circuit Design & Hardware

- **`PGLDS Schematic (Fritzing).pdf`**  
  Breadboard schematic created using Fritzing, showing all electrical connections between the Arduino Uno, MQ-5 gas sensor, LED indicator, current-limiting resistors, and buzzer. This schematic serves as the primary circuit reference.

- **`Physical Wiring Layout PGLDS.png`**  
  Photograph of the completed physical prototype assembled on a breadboard. This image verifies real-world implementation and confirms consistency with the schematic design.

---

### 📊 System Operation & Test Results

- **`baseline_no_gas_reading.png`**  
  Serial Monitor output showing baseline sensor readings under normal conditions with no gas present.

- **`baseline_no_gas_outputs.png`**  
  System output state during normal operation, with the LED and buzzer inactive, indicating no gas detection.

- **`gas_detected_reading.png`**  
  Serial Monitor output captured during controlled gas exposure, demonstrating a clear sensor response.

- **`gas_detected_outputs.png`**  
  System output state when gas is detected, showing LED activation and buzzer alert behavior.

---

### 🔋 Power Source

- **Primary Power Source:** Arduino Uno 5V (USB-powered)  
- **Alternative Power Source:** 7.2V battery (not shown in schematic)
