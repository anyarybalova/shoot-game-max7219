## Shooting Game using MAX7219 Dot LED Matrix

### Description
A simple Arduino-based shooting game using the MAX7219 LED matrix. This project helps in learning how to control the LED matrix, handle multiple simultaneous animations, and manage user input with a joystick.

### Components Required
- Arduino
- Breadboard
- MAX7219 Dot Matrix Module (x4)
- Joystick (with a button)
- Passive buzzer (optional)
- 100Ω resistor
- 100µF Capacitor
- Jumper wires

### Circuit Diagram


### Installation & Setup
1. Install the required Arduino libraries: `MD_MAX72xx.h` and `SPI.h`.
2. Upload the provided code to your Arduino board.
3. Connect the components as follows:

#### Joystick
- GND -> GND
- 5V -> 5V
- VRx -> A0 (for horizontal movement)
- VRy -> A1 (optional for vertical movement, not used in this project)
- SW -> PIN 10 (button)

#### MAX7219
- VCC -> 5V
- GND -> GND
- DOUT -> 51
- CS -> 6
- CLK -> 52

#### Reset Button
- Pin 8

#### Buzzer
- Pin 3

### Game Instructions
- The objective is to destroy the enemy base by shooting at it.
- Use the joystick to move the spaceship and the button to shoot.
- To restart the game, press the reset button.

### Lessons Learned
- **MAX7219 LED Matrix Control** – Explored how to interface with the matrix and update animations efficiently.  
- **Joystick Input Handling** – Processed analog input to control movement.  
- **Simultaneous Animation Management** – Updated multiple elements on the display without flickering or performance issues.  

### Notes
This project was designed primarily for learning purposes. While certain values were not made into constants, and the game can be expanded to include more enemies or additional features. 
The focus was on understanding the core concepts of controlling the MAX7219 matrix, handling user input, and animating elements in the game. Fine-tuning and optimization were not the primary goal for this version.

### Code

