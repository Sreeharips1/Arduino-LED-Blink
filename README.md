Arduino LED Blink Program
--------------------------------------------------------------------------------
This simple Arduino program blinks an LED connected to pin 13. It toggles the LED between ON and OFF states with a delay of 1 second.


int ledPin = 13;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH); // Turn the LED ON
  delay(1000);                // Wait for 1 second
  digitalWrite(ledPin, LOW);  // Turn the LED OFF
  delay(1000);                // Wait for 1 second
}

Explanation:
1. Variable Declaration

int ledPin = 13;
Declares an integer variable ledPin and assigns it to pin 13, which is commonly associated with the built-in LED on Arduino boards.

2. setup() Function

void setup() {
  pinMode(ledPin, OUTPUT);
}
Configures pin 13 as an output pin using pinMode(). This allows the pin to send voltage signals to control the LED.

3. loop() Function

void loop() {
  digitalWrite(ledPin, HIGH); // Turn the LED ON
  delay(1000);                // Wait for 1 second
  digitalWrite(ledPin, LOW);  // Turn the LED OFF
  delay(1000);                // Wait for 1 second
}
Runs continuously after setup() to toggle the LED state:
Turn ON: digitalWrite(ledPin, HIGH) sends a voltage signal to the pin.
Delay: delay(1000) pauses the program for 1 second.
Turn OFF: digitalWrite(ledPin, LOW) stops the voltage signal.
Delay: Another delay(1000) pauses for 1 second before repeating.
Execution Flow:
The Arduino initializes and runs the setup() function to configure pin 13 as an output.
The loop() function begins:
The LED turns ON for 1 second.
The LED turns OFF for 1 second.
This process repeats indefinitely.

How to Use
Connect an Arduino board to your computer.
Open the Arduino IDE and copy-paste the code.
Upload the code to your Arduino board.
Observe the built-in LED on pin 13 blinking at 1-second intervals.
