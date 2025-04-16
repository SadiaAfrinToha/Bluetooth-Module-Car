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
