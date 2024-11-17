# Consumption Display - ESP32

## Overview
The Consumption Display is an ESP32-based solution designed to show real-time information about energy consumption, electricity prices, and solar energy. The display provides users with a simple overview of their energy usage by showing consumption, current electricity price, costs, and solar energy directly on a TFT display. The project is integrated with Home Assistant to fetch live data and display it on a 2.8" CYD (Cheap Yellow Display) TFT screen.

## Features
- **Consumption**: Displays the current energy consumption in watts.
- **Electricity Price**: Shows the current electricity price per kWh in SEK.
- **Cost**: Calculates and shows the current cost based on consumption and electricity price.
- **Solar Energy**: Displays the current solar energy being generated, if available.
- **Display**: 2.8” CYD TFT display with ILI9342, displaying data with graphic icons for easy reading.
- **Web Server**: Simple web-based configuration and system updates through ESPHome.

# Configuration Instructions

Before using the system, you need to customize the following values in your configuration:

### Substitution Parameters
```yaml
substitutions:
  current_consumption_sensor: sensor.consumption
  current_export_sensor: sensor.export
  nordpool_sensor: sensor.nordpool_kwh
