

**Solar-Panel-Tracking**

This repository contains the code for a simple solar panel tracking system using an Arduino and a servo motor. 

**Features:**

* **Basic Tracking:** 
    * Continuously adjusts the servo motor's position to maximize sunlight exposure on the solar panel.
    * Utilizes two photoresistors (connected to analog pins A0 and A1) to measure light intensity.
* **Manual Calibration:** 
    * Includes initial calibration to find the maximum sunlight position.

**Hardware:**

* **Arduino Board:** (e.g., Arduino Uno, Nano)
* **Servo Motor:** Standard RC servo motor
* **Photoresistors:** Two or more 
* **Jumper Wires:** To connect components
* **Breadboard:** (Optional)
* **Solar Panel:** (For testing purposes)
* **Power Supply:** (To power the Arduino and servo)

**Software:**

* **Arduino IDE:** For code development and uploading

**Wiring:**

* **Servo:** Connect the servo motor's signal wire to digital pin 3 on the Arduino.
* **Photoresistors:** Connect each photoresistor to an analog pin (A0 and A1) and ground.
* **Power:** Connect the Arduino and servo motor to a suitable power source.

**Usage:**

1. **Upload the code:**
   * Open the `servo.ino` file in the Arduino IDE.
   * Upload the code to the Arduino board.

2. **Calibration:**
   * **Manual Calibration:** 
      * During the initial `setup()` phase, the servo will sweep from 0 to 90 degrees. 
      * Observe the solar panel's output or the readings from the photoresistors.
      * Adjust the servo's starting position (if necessary) to ensure it aligns with the maximum sunlight.

3. **Tracking:**
   * The Arduino will continuously read the values from the photoresistors.
   * It will adjust the servo position based on the relative light intensity on each photoresistor, maximizing solar panel output.

**Note:**

* This is a basic implementation and may require further refinement for optimal performance.
* Consider adding features like:
    * **Automatic Calibration:** Implement algorithms for automatic calibration.
    * **Weather Considerations:** Incorporate weather data (e.g., cloud cover) to adjust tracking behavior.
    * **PID Control:** Implement more sophisticated control algorithms (like PID control) for smoother and more accurate tracking.

**Disclaimer:**

This code and project are provided for educational and experimental purposes only. The author is not responsible for any damage or injury resulting from the use of this system.



