# 3-LED-for-3-Button
3 LED for 3 Button
# LED Toggle with Push Buttons (Arduino)

This Arduino sketch demonstrates how to control three LEDs using three push buttons. Each button toggles the state (ON/OFF) of its corresponding LED.

## Features

- Toggle LED 1 using Button 1
- Toggle LED 2 using Button 2
- Toggle LED 3 using Button 3
- Debouncing implemented using a simple delay

## Hardware Requirements

- Arduino board (e.g., Uno, Mega)
- 3 x LEDs
- 3 x 220Ω resistors (for LEDs)
- 3 x Push buttons
- Breadboard and jumper wires

## Pin Configuration

| Component | Arduino Pin |
|----------|--------------|
| LED 1    | 13           |
| LED 2    | 12           |
| LED 3    | 11           |
| Button 1 | 2            |
| Button 2 | 3            |
| Button 3 | 4            |

> Buttons are configured with `INPUT_PULLUP`, so connect one side to the pin and the other to **GND**.

## How It Works

Each button is wired to an Arduino input pin configured with `INPUT_PULLUP`, meaning it reads HIGH when not pressed and LOW when pressed.

When a button is pressed (detected as a falling edge), the state of the corresponding LED is toggled (switched ON if OFF, and vice versa).

A 200 ms delay is added after each press to prevent bouncing and accidental multiple toggles.

## Getting Started

1. Connect the LEDs and buttons according to the pin configuration above.
2. Upload the sketch to your Arduino board.
3. Press each button to toggle its respective LED.

## Code

See [`main.ino`](./main.ino) for the full source code.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.




