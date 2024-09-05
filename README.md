# TempSense - DHT11 Temperature and Humidity Sensor with ESP8266

TempSense is a simple Arduino project designed to read temperature and humidity data from a DHT11 sensor using an ESP8266 microcontroller. The project includes a single `.ino` file, `tempsense.ino`, which contains the code to initialize the sensor, read data, and print it to the Serial Monitor.

## Project Files

- `tempsense.ino`: The main Arduino sketch for reading and displaying temperature and humidity data from the DHT11 sensor.

## Prerequisites

Before running the project, ensure you have the following:

1. **Arduino IDE**: Install the [Arduino IDE](https://www.arduino.cc/en/software) if you haven't already.

2. **ESP8266 Board Support**: Add ESP8266 board support to the Arduino IDE. You can do this by going to **File** > **Preferences** and adding the following URL to the **Additional Boards Manager URLs** field:
Then, go to **Tools** > **Board** > **Boards Manager**, search for **ESP8266** and install it.

3. **Required Libraries**:
- **Adafruit Sensor Library**: Install it via the Library Manager in the Arduino IDE (**Sketch** > **Include Library** > **Manage Libraries**), or download it from [Adafruit's GitHub](https://github.com/adafruit/Adafruit_Sensor).
- **DHT Sensor Library**: Install it from the Library Manager or download it from [Adafruit's GitHub](https://github.com/adafruit/Adafruit_DHT).

## Hardware Setup

1. **ESP8266 Microcontroller**: Use any ESP8266-based board such as the NodeMCU or Wemos D1 Mini.
2. **DHT11 Sensor**: Connect the sensor to the ESP8266 as follows:
- **VCC** to **3.3V** (or **5V** if your board supports it)
- **GND** to **GND**
- **DATA** to **D4** (GPIO2 on many boards)

## Uploading the Code

1. Open the `tempsense.ino` file in the Arduino IDE.
2. Select your ESP8266 board and port from the **Tools** menu.
3. Click the **Upload** button to compile and upload the code to your ESP8266.

## Usage

1. Open the Serial Monitor from the Arduino IDE (**Tools** > **Serial Monitor**).
2. Set the baud rate to **115200**.
3. After uploading, you should see temperature and humidity readings printed to the Serial Monitor every 2 seconds.

## Code Overview

- **Setup Function**: Initializes serial communication and the DHT sensor.
- **Loop Function**: Reads the temperature and humidity from the DHT sensor, checks for errors, and prints the data to the Serial Monitor.

## Troubleshooting

- **No Data Displayed**: Ensure the DHT sensor is properly connected and powered. Check the connections and ensure the correct GPIO pin is used.
- **Error Messages**: Verify that all required libraries are installed and up-to-date.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or support, please open an issue on this repository or contact [mail@shan.is-a.dev](mailto:mail@shan.is-a.dev).
