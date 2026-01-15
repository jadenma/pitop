## Robotic Catapult Project
### Project Overview

For my final project, I decided to create a robotic catapult using the Pi-top kits. When you run the code, a green LED light will indicate that the system is on. Then, the screen will display the strength of the catapult, which can be adjusted between weak, medium, and strong using a potentiometer. If the potentiometer reading is in the lowest ⅓ (0-333) of values, the launch strength is weak. If the reading is in the middle ⅓ (333-665) of values, the launch strength is medium. And if reading is in the top ⅓ (666-999) of values, the launch strength is strong. When a button that is attached to the catapult is pressed, a red LED shows that the launcher is about to launch. A robotic arm controlled by a servo then launches a ping pong ball and returns to initial position for next run. Weak strength = <5 inches. Medium strength = 5-7 inches. Strong strength = >7 inches. This catapult can be used by athletes such as baseball players to consistently launch a ball at the same speed and angle each time. Humans often lack the precision and repeatability of a robot. This launcher can also be used by STEM teachers on topics such as projectile motion. The overall strength of the catapult was limited by the maximum speed of the servo.

![IMG_5368](https://github.com/user-attachments/assets/a59a9a71-f318-497c-b649-ec3ab12e18ff)

### Design Process

1. Problem Identification

Many educational and testing environments require a consistent and controllable method of launching projectiles. Human-powered launching introduces variability in force, accuracy, and safety, limiting repeatability and data reliability. The goal was to design a system that could launch a ball with adjustable power and precise control.

2. Criteria, Constraints, and Materials

* Criteria: Adjustable launch power, Consistent and repeatable launches, Simple and intuitive user control, Safe operation
* Constraints: Limited voltage and current from microcontroller, Servo torque and speed limitations, Available components and project timeline, Safety considerations for users and surroundings
* Materials: Computer (Python), Pi-top [4], 1x green LED, 1x red LED, 1x potentiometer, 1x button, 1x servo motor, 5x connecting wires, robot building metal components

#### Project Artifacts

Pi-top [4] (Base pre-built raspberry pi that behaves like a mini computer - used in step 7, Prototyping and Testing): 

<img width="475" height="174" alt="Screenshot 2026-01-15 at 12 05 32 AM" src="https://github.com/user-attachments/assets/fabd7029-9c43-4cb6-85ed-6a3d78aafe02" />

Servo (Controls mechanical arm that can rotate and swing the ping pong ball forward - used in step 6 and 7, programming/prototyping): 

<img width="230" height="242" alt="Screenshot 2026-01-15 at 12 02 03 AM" src="https://github.com/user-attachments/assets/24c041b2-9c99-4303-8b3c-8ecbfa5e05f7" />

LEDs (lights up as a signal for an event happening such as the ball being launched or the system running - used in step 6 and 7, programming/prototyping): 

<img width="455" height="245" alt="Screenshot 2026-01-15 at 12 07 38 AM" src="https://github.com/user-attachments/assets/d347ec67-5261-4158-897c-ff34e3947206" />

Potentiometer (Rotatable knob with values that range from 0-999 and creates a continuous range which can be used to adjust the power level - used in step 6 and 7, programming/prototyping): 

<img width="321" height="308" alt="Screenshot 2026-01-15 at 12 12 25 AM" src="https://github.com/user-attachments/assets/bb20062f-67f3-41ee-a617-32a3a0695217" />

3. Background Research

Research was conducted on Servo motor operation and torque characteristics, Potentiometers as analog input devices, and Basic projectile motion principles

4. Concept Generation

Multiple launch mechanisms were considered, including flywheel systems and linear actuators. A servo-driven catapult was selected due to its mechanical simplicity, precise angular control, and compatibility with available electronics. Artifacts included initial sketches and concept comparisons.

5. Circuit Generation

A circuit was designed to safely integrate analog and digital inputs with the servo motor: Potentiometer wired as a voltage divider, Button configured with appropriate pull-down logic, Servo powered and controlled via PWM signal. Pin assignments and voltage limits were documented to prevent component damage.
<img width="832" height="483" alt="Screenshot 2026-01-15 at 12 29 27 AM" src="https://github.com/user-attachments/assets/d1b1347b-3bd2-4e0f-b537-84fb5e34a3f3" />

6. Programming and Control Logic

Initial prototypes were built on a Pi-top and tested incrementally. Tests measured: Servo responsiveness, Consistency of launch distance at different power levels, Reliability of button activation. Issues such as inconsistent motion and timing errors were identified.

7. Prototyping and Testing

Initial prototypes of the catapult were built and tested incrementally. Tests measured: Servo responsiveness, Consistency of launch distance at different power levels, Reliability of button activation. Issues such as inconsistent motion, timing errors, and launch power were identified.

8. Final Solution

The final design is a servo-driven ball launcher with adjustable power controlled by a potentiometer and a push-button launch mechanism. The system meets all design criteria by providing safe, repeatable, and user-controlled launches suitable for educational demonstrations and experimental testing.

### Reflection and Connection

Designing and building the robotic ball launcher challenged me to think beyond making a device work and instead focus on making it reliable, repeatable, and safe. The most difficult aspect of the project was integrating the electronic controls with the mechanical system. Small changes in servo position or timing had a significant impact on launch consistency, which required systematic testing and iteration rather than trial-and-error.

This project strengthened my understanding of control systems, signal mapping, and system integration, particularly how analog inputs can be translated into precise mechanical motion. I also learned the importance of documenting design decisions and using data from testing to guide improvements, which is central to the engineering design process.

The skills and mindset developed through this project directly connect to real-world engineering work, where systems must operate predictably under constraints. This experience has reinforced my interest in engineering fields that combine electronics, mechanics, and programming, and it has prepared me to approach future projects with a structured, analytical, and iterative design approach.
