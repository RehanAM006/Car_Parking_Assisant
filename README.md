# Car_Parking_Assisant
# Ultrasonic Sensor Parking Assistance System
This project is an Ultrasonic Sensor-based Parking Assistance System that detects distance and alerts the user through LEDs and a buzzer. The system includes three LEDs (Red, Yellow, and Green) to indicate the proximity of an object (such as a vehicle) in front of the sensor. Additionally, a buzzer provides an alert for critical proximity.

## Circuit Diagram

| Component  | Pin   |
|------------|-------|
| Echo Pin   | 2     |
| Trigger Pin| 3     |
| Buzzer     | 4     |
| Red LED    | 8     |
| Yellow LED | 9     |
| Green LED  | 10    |



# How it Works
- The ultrasonic sensor measures the distance between the sensor and an object in front of it. The distance is calculated using the time taken for an ultrasonic wave to bounce back to the sensor.
- Based on the distance, different LEDs are triggered:
    - Red LED: If the object is less than 4 cm away (alert).
    - Yellow LED: If the object is between 4 cm and 12 cm away (ok parking).
    - Green LED: If the object is between 12 cm and 25 cm away (go further).
    - If no object is detected (distance > 25 cm), all LEDs remain off.
- A buzzer will sound when the red LED is lit, indicating a critical alert situation.
- The distance is printed in centimeters on the serial monitor.
