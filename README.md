# 🤖 Obstacle-Avoiding Robot using Arduino

An autonomous robot built with **Arduino** that navigates its environment by detecting and avoiding obstacles using an **ultrasonic sensor** and motor control logic. When an object is detected within a threshold distance, the robot automatically stops, reverses, and makes a random turn to continue safely.

---

## 🧠 How It Works

- The **ultrasonic sensor (HC-SR04)** continuously measures distance.
- If an object is detected within **20 cm**, the robot:
  - Stops
  - Moves backward briefly
  - Makes a random turn (left or right)
- If the path is clear, it keeps moving forward.

---

## 🏗️ Hardware Components

- Arduino Uno or compatible board
- HC-SR04 Ultrasonic Sensor
- L298N Motor Driver
- 2 DC Motors with wheels
- Power supply (e.g., 9V battery or Li-ion pack)
- Jumper wires
- Chassis

---

## 🔌 Pin Connections

| Component         | Arduino Pin |
|------------------|-------------|
| Ultrasonic Trig  | A1          |
| Ultrasonic Echo  | A0          |
| Motor A EN       | 10          |
| Motor A IN1      | 9           |
| Motor A IN2      | 8           |
| Motor B IN1      | 7           |
| Motor B IN2      | 6           |
| Motor B EN       | 5           |

---

## 📁 File Info

Save your Arduino code in a file named:  
`ObstacleAvoidanceRobot.ino`  
It should be placed inside a folder named:  
`ObstacleAvoidanceRobot/`

---

## ▶️ Upload Instructions

1. Open the `.ino` file using the **Arduino IDE**.
2. Connect your Arduino board via USB.
3. Select the correct **board** and **port** from the Tools menu.
4. Click **Upload**.

---

## 🚀 Demo Behavior

- 🟢 Moves forward by default
- 🟥 On obstacle detection:
  - Stops
  - Reverses
  - Randomly turns left or right
- 🔁 Repeats the cycle autonomously

---

## 📌 Notes

- Distance threshold is set to `20 cm` by default.
- Motor speed is adjustable via the `speed` variable.
- Random turn logic ensures varied pathfinding.

---

## 📷 (Optional) Add Images / Videos

_Showcase your robot in action!_

---

## 🤝 Contribution

Pull requests are welcome! Improve the logic, add features, or optimize sensor handling.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

