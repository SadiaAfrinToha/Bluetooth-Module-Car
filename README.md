# Bluetooth-Module-Car

## Components:
1.Arduino Uno <br>
2.L298N Motor Driver <br>
3.HC-05 Bluetooth Module <br>
4.2 DC Motors<br>
5.Power source (e.g. battery pack) <br>

## Feature:
1.Full directional control (including diagonal moves) <br>
2.Variable speed (0–9, q for max) <br>
3.Headlight toggle <br>
4.Clean use of a motor() function for abstraction <br>

## Working Guideline:

| Command | Action         |
|---------|----------------|
| `F`     | Forward        |
| `B`     | Backward       |
| `L`     | Turn Left      |
| `R`     | Turn Right     |
| `G`     | Forward-Left   |
| `I`     | Forward-Right  |
| `H`     | Backward-Left  |
| `J`     | Backward-Right |
| `S`     | Stop           |

---

## Headlight Control

| Command | Action   |
|---------|----------|
| `U`     | Light ON |
| `u`     | Light OFF|

---

## Speed Control

| Command | Speed Level |
|---------|-------------|
| `0`     | 0 (stop)    |
| `1`     | 25          |
| `2`     | 50          |
| `3`     | 75          |
| `4`     | 100         |
| `5`     | 125         |
| `6`     | 150         |
| `7`     | 175         |
| `8`     | 200         |
| `9`     | 225         |
| `q`     | 250 (max)   |

## Circuit Connections – Bluetooth Controlled Car with Arduino

## L298N Motor Driver to Arduino

| L298N Pin | Arduino Pin | Description |
|----------|-------------|-------------|
| ENA      | 10          | Left motor speed (PWM) |
| IN1      | 9           | Left motor direction control |
| IN2      | 8           | Left motor direction control |
| IN3      | 7           | Right motor direction control |
| IN4      | 6           | Right motor direction control |
| ENB      | 5           | Right motor speed (PWM) |
| VCC      | 12V Battery | Motor power |
| GND      | GND         | Common ground |
| 5V       | 5V (Arduino) *(Optional)* |

---

## Motors to L298N

| Motor        | L298N Pins |
|--------------|------------|
| Left Motor   | OUT1, OUT2 |
| Right Motor  | OUT3, OUT4 |

---

## Bluetooth Module (HC-05/HC-06) to Arduino

| Bluetooth Pin | Arduino Pin | Note |
|---------------|-------------|------|
| VCC           | 5V          | Power supply |
| GND           | GND         | Ground |
| TX            | RX (Pin 0)  | Receives data from Bluetooth |
| RX            | TX (Pin 1)  | Sends data to Bluetooth *(Use voltage divider!)* |

---

## Headlight (LED) to Arduino

| LED Pin | Arduino Pin | Description |
|---------|-------------|-------------|
| +ve     | 1           | Turn ON/OFF via digitalWrite |
| -ve     | GND         | Ground |

---

## IR Sensors to Arduino (Optional for Line Following)

| IR Sensor | Arduino Pin |
|-----------|-------------|
| Left IR   | A0          |
| Right IR  | A1          |
| Middle IR | A4          |

---

## Power Supply Notes

- Use **9V or 12V battery** to power motors via **L298N VCC**.
- Never power motors directly from
