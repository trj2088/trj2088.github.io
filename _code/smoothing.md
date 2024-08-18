---
layout: codelayout
category: Data Aquisition
project_name: Simple Smoothing 
project_description: This is a simple script that reads an analog value from an input and prints it to the serial monitor. This is a great starting point for learning how to read analog values from a sensor.
---

<pre><code>
        int sensorPin = A0;    // select the input pin for the potentiometer
        int sensorValue = 0;  // variable to store the value coming from the sensor

        void setup() {
        Serial.begin(9600);
        }

        void loop() {
        // read the value from the sensor:
        sensorValue = analogRead(sensorPin);    
        Serial.println(sensorValue);   
        delay(100);                     
        }
</code></pre>