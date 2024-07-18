#include <Wire.h>
#include "PCAL9535A.h"

// Create a PCAL9535A object using hardware I2C
PCAL9535A::PCAL9535A<TwoWire> gpio(Wire);

void setup() {
  Wire.begin();
  Serial.begin(9600);

  // Initialize PCAL9535A with address 0x20
  gpio.begin();

  // Set all pins as outputs and turn off all relays
  for (uint8_t i = 0; i < 16; i++) {
    gpio.pinMode(i, OUTPUT);
    gpio.digitalWrite(i, LOW);
  }

  Serial.println("PCAL9535A initialized.");
}

void loop() {
  // Turn on relays sequentially
  for (uint8_t i = 0; i < 16; i++) {
    gpio.digitalWrite(i, HIGH);
    delay(1000);  // 1 second delay between turning on each relay
  }

  delay(5000);  // 5 second delay after all relays are turned on

  // Turn off all relays simultaneously
  for (uint8_t i = 0; i < 16; i++) {
    gpio.digitalWrite(i, LOW);
  }

  delay(5000);  // 5 second delay after turning off all relays
}
