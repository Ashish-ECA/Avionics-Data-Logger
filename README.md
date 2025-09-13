# Avionics Data Logger (Embedded, Aerospace)

## Overview  
This project is an embedded system designed to log real-time avionics sensor data for diagnostics and flight health monitoring. It captures critical flight parameters with timestamping and stores logs securely for post-mission analysis.

## Features  
- Real-time sensor data acquisition using embedded microcontroller  
- Timestamped logging of sensor values to onboard memory  
- Low power consumption suitable for aerospace environments  
- Reliable data integrity with error checking mechanisms  
- Easy extraction of log files for analysis after flight

## How to Run  
1. Connect avionics sensors (e.g., temperature, pressure) to the microcontroller inputs.  
2. Flash the provided firmware (`logger_firmware.c`) onto the embedded board.  
3. Power the system and start logging automatically on boot.  
4. After operations, retrieve logged data via USB or wireless interface.  
5. Use provided parsing scripts (optional) to analyze collected data.

## File Structure  
- `logger_firmware.c` — Embedded C code for data logging firmware  
- `schematics.pdf` — Hardware connection and sensor wiring diagrams  
- `data_parser.py` — Optional Python script for log file parsing and visualization  
- `README.md` — Project overview and instructions  
- `docs/` — Flight test reports, power consumption analyses, and logs  

## Methodology Summary  
- Continuous sampling of connected sensors at defined intervals  
- Real-time timestamp generation and data structuring for each sample  
- Storage management optimized for limited memory resources  
- Simple error detection to identify corrupted data segments

## Future Work  
- Wireless telemetry integration for live data streaming  
- Implement advanced error correction and compression algorithms  
- Expand sensor suite to include GPS, accelerometers, and gyroscopes  
- Design accompanying ground station software for live monitoring

## References  
- Aerospace embedded system design textbooks and guidelines  
- Relevant avionics data acquisition standards and protocols  
- Research papers on flight data recorders and black box technology  

## Contact  
ashishprajit308@gmail.com
