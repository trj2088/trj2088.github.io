---
layout: codelayout
category: Data Aquisition
project_name: Button Box 
project_description: This is a bare bones sketch to create a button box similar to a stream deck. Using the keyboard.h library and an Arduino micro, you can connect multiple momentary switch buttons and program custom commands to each putton push. 
---
<div class="codeblock">
    <pre><code>
    #include <Keyboard.h>

    void setup() {
    // make pin 2 an input and turn on the
    // pullup resistor so it goes high unless
    // connected to ground:
    pinMode(2, INPUT_PULLUP);
    Keyboard.begin();
    }

    void loop() {
     //if the button is pressed
     if (digitalRead(2) == LOW) {
     //Send an ASCII 'A', replace with proper ASCII for desired   character
     Keyboard.write(65);
     }
}
    </code></pre>
</div>