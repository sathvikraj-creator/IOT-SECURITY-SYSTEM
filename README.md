# IOT-SECURITY-SYSTEM

COMPANY: CODTECH IT SOLUTIONS

NAME: AKEPOGU SATHVIK RAJ

INTERN ID: CT04DH122

DOMAIN: INTERNET OF THINGS

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH

# DESCRIPTION

This is a simple IoT Security System prototype developed with an Arduino Uno. It uses a PIR sensor for detecting motion, shows alerts on a 16x2 LCD display, activates a buzzer and LED as visual/auditory alarms, and mimics image capture through a push button. It is meant to give a basic understanding of how microcontrollers can be utilized in home security systems with low-cost materials and basic logic.
The project is simulated and tested entirely with Tinkercad Circuits for virtual prototyping. It is a beginner-level introduction to real-time sensing, input/output devices, and embedded system programming in C++ with the Arduino IDE.

Components Used:
•	Arduino Uno R3
•	PIR Motion Sensor (HC-SR501)
•	16x2 LCD Display
•	10K Potentiometer (for LCD contrast)
•	Push Button (to simulate image capture)
•	Buzzer (for audible alert)
•	LED + 220Ω Resistor (for visual alert)

Working Principle:
1. The PIR sensor constantly senses infrared radiation around it. On detecting motion, its digital output becomes HIGH.
2. The Arduino senses the output of PIR and, on detecting motion:
•	Activates the buzzer and LED
•	Sends a message "Motion Detected! Sending alert." to the LCD
3. In the absence of motion, the system remains in idle mode and shows "System Active" on the LCD.
4. A push button is incorporated to mimic a camera trigger. On push:
The LCD shows "Image Captured", mimicking a photo being snapped.
This configuration emulates a fundamental smart surveillance system with no internet integration. Nevertheless, it can be expanded with the use of ESP32 or NodeMCU to send notifications to a mobile application (e.g., Blynk or Telegram) or save data on the cloud (e.g., Firebase).

Overview of Code:
The Arduino program utilizes the LiquidCrystal library to communicate with the LCD. It declares all required pins for PIR sensor, buzzer, LED, and button. The logic involves:
•	digitalRead() for reading from the PIR and button
•	digitalWrite() for writing to buzzer and LED
•	lcd.setCursor() and lcd.print() to display on the LCD in real time
The setup() function configures all pin modes and the LCD display, and the loop() function repeatedly monitors motion and button statuses to manage system operations accordingly.


# OUTPUT

When the push button is activated the LCD display shows that "Image captured" 

<img width="1299" height="782" alt="Image" src="https://github.com/user-attachments/assets/97bc6bf7-b950-4ffd-9328-172d0534548f" />

When PIR sensor detects motion , it triggers buzzer & led and LCD display shows that "Motion Detected! Sending alert..."

<img width="1183" height="792" alt="Image" src="https://github.com/user-attachments/assets/ce6f6bf1-01a1-43b1-b045-f7889cba46eb" />
