# Circle Movement Using Zumo32U4 Robot

## Description
This project demonstrates a simple program for the Zumo32U4 robot to move in a circular motion using its motors. By adjusting the speeds of the left and right motors, the robot performs a curve-like movement. The robot stops after completing the movement for a predefined time.

---

## Features
- Waits for the user to press the **Button A** to initiate the motion.
- Moves in a circular motion by setting different speeds for the left and right motors.
- Stops after running the motion for approximately 7.5 seconds.

---

## Components Used
- **Zumo32U4 Robot**: A programmable robot platform equipped with motors, sensors, and a button interface.
- **Button A**: Used to start the movement sequence.
- **Zumo32U4 Library**: Provides access to the robot's motors and button controls.

---

## Code Explanation
1. **Libraries**:
   - `Wire.h`: For I2C communication (required for Zumo32U4).
   - `Zumo32U4.h`: Includes the motor and button control functionalities.

2. **Global Variables**:
   - `left_Speed`: Speed of the left motor (320 units).
   - `right_Speed`: Speed of the right motor (400 units).

3. **Setup Function**:
   - Empty in this case, as no initialization is required beyond library defaults.

4. **Loop Function**:
   - Waits for the user to press **Button A**.
   - Starts the motors with predefined speeds for the left and right wheels.
   - Runs the motors for approximately 7.5 seconds (`delay(7493)`).
   - Stops the motors by setting their speeds to zero.

---

## How to Use
1. Connect your Zumo32U4 robot to a compatible microcontroller (e.g., Arduino).
2. Install the required libraries:
   - [Zumo32U4 Library](https://github.com/pololu/zumo-32u4-arduino-library)
3. Upload the code to your Zumo32U4.
4. Press **Button A** on the robot to start the circular motion.

---

## Customization
- **Adjust Speed**: Modify `left_Speed` and `right_Speed` variables to change the size and speed of the circle.
- **Change Duration**: Modify the `delay(7493)` value to adjust how long the robot moves before stopping.

---

## Author
**Ankush Singh**
