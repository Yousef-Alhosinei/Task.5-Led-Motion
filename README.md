# Task.5-Led-Motion
# ESP32 Motion and Light Controlled LED with Relay

# The components

- ESP32 Development Board
- LED
- Light Dependent Resistor LDR
- PIR Motion Sensor
- Relay Module (5V or 3.3V, depending on your ESP32's capabilities)
- Breadboard
- Jumper Wires
- 220-ohm Resistor
- 10k-ohm Resistor



LDR:
1. Connect one leg of the LDR to the 3.3V pin on the ESP32.
2. Connect the other leg of the LDR to GPIO 14 on the ESP32.
3. Connect one end of a 10k-ohm resistor to the same leg of the LDR that goes to GPIO 14.
4. Connect the other end of the 10k-ohm resistor to GND.



PIR Sensor:
1. Connect the VCC pin of the PIR sensor to the 3.3V pin on the ESP32.
2. Connect the GND pin of the PIR sensor to GND on the ESP32.
3. Connect the OUT pin of the PIR sensor to GPIO 25 on the ESP32.



Relay Module:
1. Connect the VCC pin of the relay module to the 3.3V pin on the ESP32.
2. Connect the GND pin of the relay module to GND on the ESP32.
3. Connect the IN pin of the relay module to GPIO 23 on the ESP32.



LED:
1. Connect the anode (longer leg) of the LED to the NO (Normally Open) terminal of the relay.
2. Connect the cathode (shorter leg) of the LED to one end of a 220-ohm resistor.
3. Connect the other end of the 220-ohm resistor to GND.



# The process:

- LDR : Detects the ambient light level. When light falls on the LDR, its resistance decreases, resulting in a higher voltage drop across it. This change in resistance is read by the ESP32's analog input pin (GPIO 14).

- PIR : Detects motion by measuring changes in infrared radiation in its surroundings. When motion is detected, the PIR sensor outputs a HIGH signal to GPIO 25 of the ESP32.

- Relay Module: Acts as a switch to control the LED. When the relay is activated, it closes the circuit between the NO and COM terminals, allowing current to flow through the LED and turn it on.

![image](https://github.com/user-attachments/assets/d0361ea6-6c74-449d-8555-a56a18440b4f)
