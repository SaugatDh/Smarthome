# Smarthome Project

This repository contains Arduino sketches and related code for a smart home automation system, primarily targeting ESP32 microcontrollers. The project aims to integrate various sensors and actuators to create an intelligent and responsive home environment.

## Features

- **Temperature and Humidity Monitoring:** Utilizes the AHT10 sensor for accurate environmental data collection.
- **Web Server Interface:** Implements a simple web server on ESP32 for remote monitoring and control of smart home devices.
- **Light Intensity Detection:** Integrates an LDR (Light Dependent Resistor) to measure ambient light levels.
- **Modular Design:** Individual sensor and module functionalities are encapsulated in separate sketches, allowing for flexible integration into the main `SmartHomeV1.ino` project.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Arduino IDE
- ESP32 Board Support Package for Arduino IDE
- Necessary libraries for AHT10 sensor and web server (e.g., `Adafruit AHT10`, `WiFi`, `WebServer`)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/Smarthome.git
    ```
2.  **Open in Arduino IDE:**
    Open the `.ino` files (e.g., `SmartHomeV1.ino`) in the Arduino IDE.
3.  **Install Libraries:**
    Go to `Sketch > Include Library > Manage Libraries...` and search for and install the required libraries (e.g., "Adafruit AHT10").
4.  **Configure WiFi (for ESP32 projects):**
    In `esp32simpleserver.ino` or `SmartHomeV1.ino`, update your WiFi credentials:
    ```cpp
    const char* ssid = "YOUR_WIFI_SSID";
    const char* password = "YOUR_WIFI_PASSWORD";
    ```
5.  **Select Board and Port:**
    Go to `Tools > Board` and select your ESP32 board (e.g., "ESP32 Dev Module"). Then, select the correct COM port under `Tools > Port`.
6.  **Upload:**
    Click the "Upload" button in the Arduino IDE to flash the code to your ESP32.

## Usage

Once uploaded, the ESP32 will connect to your WiFi network and start its functions.
- Access the web server by navigating to the ESP32's assigned IP address in your web browser.
- Monitor serial output for sensor readings and debug information.

## Contributing

Contributions are welcome! Please feel free to open issues or submit pull requests.

## Team Members

This project was developed as a fourth-semester project by the following team members:

*   Suman Basnet
*   Saurav Adhikari
*   Saugat Dhungana
*   Nikesh Dhakal

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.