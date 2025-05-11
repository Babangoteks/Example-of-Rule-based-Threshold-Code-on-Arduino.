# Example-of-Rule-based-Threshold-Code-on-Arduino.
This project is an Arduino-based air quality monitoring system designed to detect smoke and carbon monoxide (CO) gas levels using analog sensors. This system provides an indication of the level of air hazards via an I2C LCD, indicator LED, buzzer, and a PWM-controlled cooling fan based on the detected gas levels.
Key Features
📟 16x2 LCD display with I2C to display sensor values ​​and air safety status.

🔴 Red LED as danger indicator.

🟢 Green LED as safe indicator.

🔊 Buzzer for warning if gas level is dangerous.

🌬️ Automatic fan control based on gas level for ventilation.

📊 Serial log for debugging and monitoring sensor values.

🎯 System Logic
The system uses threshold-based rule logic to determine conditions:

SAFE if smoke and CO are low.

ALERT if any of the parameters start to increase.

ALERT for medium conditions.

DANGER if smoke or CO approaches the upper limit.

CAUTION!!! for extreme conditions.

PWM fan is controlled according to risk level:

Off when safe

Low–Mid–Fast depending on gas detection level

🧠 Technical Notes
Currently the system does not use fuzzy logic methods. All decisions are based on analog sensor readings against threshold values. To improve system accuracy and intelligence, fuzzy logic or machine learning can be integrated in the future.

📦 Components Used
Arduino Uno / Nano / Mega

Gas Sensor (eg MQ-2, MQ-7)

16x2 I2C LCD

Motor Driver (for fan control)

LED (Red, Green)

Buzzer

DC Fan
