# Arduino_i2c_relay
![XL9535 plate](https://github.com/nozloy/Arduino_i2c_relay/blob/b56cb617c20fccbfad817c98cdc4285ad39c2d1a/relay.jpg)

Test-scetch for Arduino IDE for testing relay plates based on PCA9535

Required PCAL9535A Arduino [library](https://github.com/chrissbarr/PCAL9535A-Arduino-Library/tree/master) for XL9535 plate

### Explanation:
1. **Turning on relays sequentially**:
   - Relays turn on one by one with a 1-second delay between each relay.
2. **Delay after turning on**:
   - A 5-second delay after all relays are turned on to observe the state.
3. **Turning off all relays simultaneously**:
   - All relays turn off simultaneously.
4. **Delay after turning off**:
   - A 5-second delay after all relays are turned off.

### Checks:
1. **Connections**: Ensure SDA and SCL are correctly connected to the Arduino Nano.
2. **Power**: Make sure the relays are receiving sufficient power.
3. **Monitoring**: Monitor the serial output for debugging.

This sketch should turn on relays sequentially with a 1-second delay between each, and then turn off all relays simultaneously with a 5-second delay to observe the state.
