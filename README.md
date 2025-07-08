# IOT-SECURITY-SYSTEM

*COMPANY*: CODTECH IT SOLUTIONS 

*NAME*: AKEPOGU SATHVIK RAJ 

*INTERN ID*: CT04DH122

*DOMAIN*: INTERNET OF THINGS

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH


# DESCRIPTION

The project involves developing a basic yet efficient IoT-based motion detection security system using Arduino Uno as the controller. The primary objective is to detect the movement of a human through a PIR (Passive Infrared) sensor, notify the users with audio (buzzer) and visual (LED and LCD) signals, and simulate an image capture process through a push button.
The system is real-time and can be implemented in home, office, or small business area protection systems. When the PIR sensor senses motion, it triggers a HIGH signal to the Arduino, and the Arduino automatically activates the buzzer and LED, and displays a visible warning message on a 16x2 LCD display. The real-time feedback replicates the basic action of advanced surveillance systems that warn users of potential intrusions

Components Used:
• Arduino Uno – Microcontroller board that runs the code and controls peripherals
• PIR Motion Sensor (HC-SR501) – Human or animal movement detection
• 16x2 LCD Display – Shows system status and alerts
• 10KΩ Potentiometer – Adjusts LCD contrast
• Buzzer – Beeps when there is motion
• LED – Visual alert for movement detection
• Push Button – Mimics image capture trigger
• 220Ω Resistors – To restrict current for LED and LCD backlight

Working Principle:
It is always watching out for movement with the help of a PIR sensor. Upon detecting movement:
• The buzzer sounds, creating a sound signal.
• The LED glows as a visible signal.
• An LCD screen shows a message: "Motion Detected! Sending alert."
The user can then press the push button, which serves to mimic taking a photo of the intruder. When pressed, the LCD will update to display: "Image Captured".
If no movement is detected, the system enters idle mode and displays: "System Active". Buzzer and LED do not display any indication during this time.
Visibility of the LCD is controlled by a 10K potentiometer, which adjusts its contrast.
This project mimics the main role of commercial IoT security systems in a simplified, beginner-friendly manner.

Overview of the code:
The Arduino code starts off with the inclusion of the LiquidCrystal library and initialization of the LCD using pins 8, 9, 10, 11, 12, 13. Input and output pins are declared for:
• PIR sensor D2
• D6 Buzzer
•LED on D5
•Button on D7
In the setup() function:
•All pins are configured.
•The LCD displays "System Ready" for 2 seconds and then blanks.
Inside the loop() function:
• Whenever motion is detected (PIR == HIGH):
     Buzzer and LED are activated.
     LCD shows the motion alert message.
•If no motion:
    Buzzer and LED are off.
    LCD shows "System Active".
• If push button is pressed:
      LCD briefly states "Image Captured".


Applications:
•Home/Office Security Systems
•Smart Surveillance Setup 
•Shop or Warehouse Entrance Detection 
•Motion-activated Notification Systems


# OUTPUT

When the push button is activated the LCD display shows that "Image captured" 

<img width="1299" height="782" alt="Image" src="https://github.com/user-attachments/assets/97bc6bf7-b950-4ffd-9328-172d0534548f" />

When PIR sensor detects motion , it triggers buzzer & led and LCD display shows that "Motion Detected! Sending alert..."

<img width="1183" height="792" alt="Image" src="https://github.com/user-attachments/assets/ce6f6bf1-01a1-43b1-b045-f7889cba46eb" />
