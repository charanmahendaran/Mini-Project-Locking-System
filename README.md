# Locking System Using ESP32 Embedded Controller

#### In today's fast-paced world, the demand for smart security systems has surged, leading to the development of more efficient and reliable solutions for home and office security. One such system is the ESP32-based Locking System, which offers a modern, internet-connected approach to controlling access. The ESP32, a versatile and powerful embedded controller, serves as the core component for this project, enabling remote management of locks via the Telegram app.

#### The ESP32 microcontroller is equipped with Wi-Fi and Bluetooth capabilities, making it ideal for IoT (Internet of Things) applications. By leveraging its Wi-Fi connectivity, the system can be controlled remotely through a Telegram bot, offering users a convenient and secure way to lock or unlock doors from anywhere in the world. This system not only adds a layer of convenience but also provides the ability to track and control access in real-time.

#### This project offers a blend of embedded systems, IoT, and user-friendly app control, creating an innovative solution to traditional security systems. The use of Telegram as the interface enhances the system's usability, as it leverages an app that is already widely used and familiar to many. Moreover, it enhances security by enabling access control via a secure communication channel.

## IMPLEMENTATION
The implementation of the ESP32-based Locking System using the Telegram app involves both hardware and software components. The project will consist of the following key stages:
-  Hardware Setup
-  Software Development
-  Telegram Bot Configuration
-  Integration and Testing

### Hardware Setup

<h4>(a) Components Needed:</h4>

-  ESP32 Microcontroller : This will be the central unit controlling the locking system, and it will handle communication with the Telegram bot and the lock hardware.
-  Servo Motor or Electronic Lock : This will be the actuator for locking and unlocking. A servo motor can be used to physically lock/unlock a door, while an electronic solenoid lock can also be used for this purpose.
-  Power Supply : The ESP32 and lock need a power supply. Depending on the components, this could range from a 5V to a 12V supply.
-  Jumper Wires and Breadboard : For wiring the components together.
-  Relay Module (if needed) : If you're using a solenoid lock or any high-power electronic locking system, a relay module may be required to safely control the power to the lock from the ESP32.
-  Resistors and Capacitors : These may be needed for additional components or to stabilize power to the ESP32 or locking mechanism.

<h4>(b) Basic Circuit Diagram:</h4>

-  The ESP32 will be connected to the relay or servo motor to control the locking mechanism.
-  The GPIO pins of the ESP32 will be used to send signals to the servo motor or relay.
-  A button or magnetic sensor can be added for local manual control of the locking system (optional).

### Software Development
<h4>(a) Programming Environment:</h4>

Arduino IDE: The ESP32 can be programmed using the Arduino IDE. The IDE allows you to write, compile, and upload the code to the ESP32 board.

<h4>(b) Libraries Required:</h4>

- WiFi.h: For connecting the ESP32 to Wi-Fi.
- UniversalTelegramBot.h: A library for communicating with the Telegram Bot API.
- Servo.h (if using a servo motor): For controlling the servo motor.
- ArduinoJson.h: For parsing JSON data from the Telegram bot.

### Telegram Bot Configuration
To control the lock via the Telegram app, you'll need to set up a Telegram Bot :

<h4>(a) Create a new Telegram Bot:</h4>

-  Open the Telegram app and search for the “BotFather.”
-  Use the command /newbot to create a new bot.
-  You’ll receive an API token for your bot. Save this token as you will need it in your code.

<h4>(b) Obtain Your Chat ID:</h4>

-  Start a conversation with your bot in Telegram.
-  Use a bot like [@userinfobot] (https://t.me/userinfobot) to find your Chat ID. You’ll need this ID to send messages to your specific user.

### Integration and Testing
Once the hardware is assembled and the software is loaded onto the ESP32, the system needs to be tested to ensure functionality:
-  Connect the ESP32 to Wi-Fi : Verify the ESP32 can connect to your network.
-  Test the Lock/Unlock Mechanism : Ensure the servo motor or relay activates correctly in response to commands sent from the Telegram bot.
-  Test Telegram Commands : Send /lock and /unlock commands to the Telegram bot to verify the ESP32 responds appropriately, locking and unlocking the door.

## RESULTS
The implementation of the ESP32-based Locking System controlled through the Telegram app results in several key outcomes, which demonstrate the effectiveness and practicality of the solution. Below are the key outcomes of the system:

<h4>(a) Remote Access Control:</h4>

One of the primary outcomes of this system is the ability to control the locking mechanism remotely, from anywhere with an internet connection. By leveraging the ESP32’s Wi-Fi capabilities and the Telegram messaging app, users can lock or unlock doors without being physically present. This outcome is especially beneficial for:
-  Homeowners : Granting access to family members, friends, or service personnel without the need to provide physical keys.
-  Businesses/Offices : Granting temporary access to employees or visitors without being physically on-site, improving the flexibility and security of office premises.

<h4>(b) Improved Security and Convenience:</h4>

The system eliminates the need for traditional keys, which can be lost, duplicated, or stolen. Instead, digital communication via the Telegram bot ensures secure access management. This outcome significantly enhances security by:

-  Providing a traceable record of access (e.g., who locked/unlocked the door and when).
-  Enabling instant notifications when the door is locked/unlocked, improving monitoring.
-  Password-less authentication : The Telegram app acts as the authentication layer, with only authorized users able to control the lock via their Telegram credentials.

Additionally, the convenience of controlling access via a familiar mobile app (Telegram) enhances the user experience, ensuring the system is easy to use and doesn’t require additional hardware or software.








