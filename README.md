# RCM-Hardware

Starting in fall 2023 I started thinking about making a smaller [RCM board](https://github.com/RCMgames/RCM_hardware_documentation_and_user_guide/tree/v1/Robot%20Control%20Module/circuit%20diagram%20and%20fritzing%20design).
I wanted to find a microcontroller board that includes an esp32 chip instead of using an esp32 chip directly, in order to keep the project simpler and more likely to work – I didn’t want to have to design a circuit with an antenna.
I found the Adafruit QT Py esp32 board that’s tiny (about the size of lots of bare esp32 modules) and still has 13 GPIO pins.
That’s a large decrease from the 20 GPIO pins from the ESP32 boards used in the previous design. I didn’t want to reduce the number of motors and servos that can be connected.
The L293D h-bridge chips in the old design take a lot of pins, if I used a motor driver chip with a serial interface, I could save pins for controlling servos.
After looking at a few options I found the Trinamic TMC7300. https://www.analog.com/en/products/tmc7300.html
Each driver can control 2 motors, and up to 4 drivers can be controlled from just two pins from the QT Py.
This means the new design can control 8 servos and 8 motors. Because 8 bits is a byte and the boards are small and bite sized I named these boards RCM BYTE.

![11020293](https://github.com/RCMgames/RCM-Hardware-BYTE/assets/59814881/c987c97d-4fd9-44b2-9f5a-b85f4dfdcac6)
