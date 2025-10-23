# Obstracle_avoiding_robot

## 📌 Overview
An autonomous obstacle-avoiding robot built using:
- Arduino Uno
- Ultrasonic sensor for distance detection
- Servo motor for sensor rotation
- DC motors for movement
- L298N motor driver for control

The robot detects obstacles and navigates around them without manual input.

---

## ⚙️ Components
- Arduino Uno
- HC-SR04 Ultrasonic Sensor
- SG90 Servo Motor
- L298N Motor Driver
- 2 × DC Motors with Wheels
- Chassis
- Battery Pack
- Jumper Wires
- Bread Board


---
## 🛠 Circuit Diagram
![WhatsApp Image 2025-08-09 at 15 49 08_b54f61cd](https://github.com/user-attachments/assets/2865a47f-10a6-432a-95d4-8ed1a3c48018)


---

## 🛠 Working Process
1. Power On – When switched on, the Arduino initializes the servo to its center position.
2. Initial Scan – The ultrasonic sensor, mounted on the servo, checks the distance directly ahead.
3. Decision Making – If the distance is greater than the threshold, motors run forward.
4. Obstacle Detection – When an obstacle is detected within the threshold distance:
   - The motors stop.
   - The servo rotates left and right to scan for available paths.
   - The Arduino compares left and right distances.
5. Path Selection – The robot turns towards the direction with the most clearance.
6. Repeat Cycle – The process repeats continuously to avoid collisions.

---

## ⚠️ Precautions & Safety Notes
- Avoid using the robot on wet or uneven surfaces.
- Ensure all connections are secure before powering on.
- Do not power the Arduino and motors from the same USB port.
- Keep battery terminals insulated to prevent short circuits.
- Avoid running the motors for long periods without cooling.

---
---

## ⚙️ Images
![WhatsApp Image 2025-08-07 at 17 25 19_e662fa38](https://github.com/user-attachments/assets/820e619e-2573-4c55-9afd-473a6691de0f)

![WhatsApp Image 2025-08-07 at 17 25 22_535aa755](https://github.com/user-attachments/assets/51fd058d-4200-49cb-acc3-247060f4bcbb)

![WhatsApp Image 2025-08-07 at 17 25 29_1de5f041](https://github.com/user-attachments/assets/9642b21f-bfd3-4e5d-aacf-a95fe347691a)



---
## 🛠 Working Principle
1. The ultrasonic sensor scans the surroundings.
2. Measures distances to detect nearby obstacles.
3. If an obstacle is within a set threshold, the robot stops and changes direction.
4. Selects the path with the most clearance.


---



## 💻 Code Description
- Initializes the ultrasonic sensor and servo motor.
- Continuously reads distance values.
- Controls motor movement based on detected distances.
- Implements obstacle avoidance logic.

---

## 🚀 How to Run

1. Open .ino file in Arduino IDE.
2. Connect the components as shown in the circuit diagram.
3. Upload the code and power the robot.

---

## 🛠 Tools Used
- Arduino IDE
- Embedded C/C++

---

## ✨ Future Improvements
- Integrate IR sensors for edge detection.
- Add PWM-based speed control.
- Implement Bluetooth remote control.

---

## 📜 License
MIT License
