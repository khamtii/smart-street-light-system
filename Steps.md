### Steps Taken

1. Connect the IR sensors:
   - Insert the IR sensors into the breadboard.
   - Connect the VCC (power) pin of each IR sensor to the 5V pin on the Arduino.
   - Connect the GND (ground) pin of each IR sensor to the GND pin on the Arduino.
   - Connect the OUT pin of each IR sensor to any digital input pins on the Arduino (e.g., pins 11,12 and 13).
2. Connect the LDR:
   - Insert the LDR into the breadboard.
   - Connect one leg of the LDR to the 5V pin on the Arduino.
   - Connect the other leg of the LDR to one end of a resistor (e.g., 220 ohms). 
  - Connect the free end of the resistor to the GND pin on the Arduino.  
 - Connect a jumper wire from the junction between the LDR and the resistor to an analog input pin on the Arduino (e.g., A0).
3. Connect the LED:
- Insert the LED to the breadboard
- make a common ground for the negative terminal of the LEDs
- Connect all the negative pins of the LEDs to the common ground
- Connect the positive terminal of the LEDs to digital input pins on the Arduino board (e.g, pins 3,5 and 6).


4. Upload the code:
   - Open the Arduino IDE on your computer.
   - write the code to control the street light based on the sensor inputs.
   - Connect the Arduino board to your computer if not already connected.
   - Select the appropriate board and port in the Arduino IDE and Upload the code to the Arduino board.
5. Test the circuit:
   - Make sure the street light is properly wired and the code is uploaded.
   - Adjust the sensitivity of the IR sensors and the LDR based on your requirements.
   - Observe the behavior of the street light as you block the IR sensors or change the ambient light    conditions.

