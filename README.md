DHT11-ESP32-UBIDOTS

To read temperature and humidity data using a DHT11 sensor with an ESP32 board and upload the data to Ubidots, you can follow these step-by-step instructions. 
This project will require some hardware components, including the ESP32, DHT11 sensor, and a computer to program the ESP32.

Hardware Components:
1. ESP32 board.
2. DHT11 temperature and humidity sensor.
3. Micro-USB cable for programming the ESP32.
4. Breadboard and jumper wires.

Software Requirements:
1. Arduino IDE.
2. Arduino libraries:
  i.   <DHT.h> 
  ii.  <UbidotsESP32Mqtt.h> - https://github.com/ubidots/esp32/archive/main.zip


Step 1: Set up the Arduino IDE
- Install the Arduino IDE on your computer if you haven't already.
- Open the Arduino IDE and go to "File" > "Preferences."
- In the "Additional Boards Manager URLs" field, add the ESP32 board manager URL: `https://dl.espressif.com/dl/package_esp32_index.json`
- Go to "Tools" > "Board" > "Boards Manager" and search for "esp32." Install the "ESP32 by Espressif Systems" package.

Step 2: Install Required Libraries
- In the Arduino IDE, go to "Sketch" > "Include Library" > "Manage Libraries."
- Search for and install the following libraries:
  - DHT.h
  - UbidotsESP32Mqtt.h

Step 3: Wiring the Components
- Connect the DHT11 sensor to your ESP32 as follows:
  - DHT11 VCC to Vin on ESP32.
  - DHT11 GND to GND on ESP32.
  - DHT11 Data to GPIO pin (e.g., D26) on ESP32.

Step 4: Create a Ubidots Account
- If you don't have a Ubidots account, sign up for one at Ubidots (https://ubidots.com/).

Step 5: Code for ESP32
- Open the Arduino IDE and create a new sketch.
- Copy and paste the following code into the sketch. Replace `*******` with your Ubidots API token, WiFi name, Wifi password accordingly.

Step 6: Upload the Code
- Select your ESP32 board from "Tools" > "Board."
- Select the appropriate COM port from "Tools" > "Port."
- Click the "Upload" button to upload the code to the ESP32.

Step 7: Monitor Data in Ubidots
- Once the code is uploaded, open the Serial Monitor to view temperature and humidity readings.
- Visit your Ubidots account to see the data displayed in your Ubidots dashboard.



That's it! You've successfully created a project to read temperature and humidity using a DHT11 sensor with an ESP32 board and upload the data to the Ubidots website.

