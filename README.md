# Arduino_i2c_relay
![XL9535 plate](https://github.com/nozloy/Arduino_i2c_relay/blob/b56cb617c20fccbfad817c98cdc4285ad39c2d1a/relay.jpg)

Test-scetch for Arduino IDE for testing relay plates based on PCA9535

## ENG
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

## CIS

Понадобится PCAL9535A Arduino [библиотека](https://github.com/chrissbarr/PCAL9535A-Arduino-Library/tree/master) для платы XL9535

### Пояснения:
1. **Включение реле поочередно**:
   - Реле включаются по очереди с задержкой 1 секунда между включением каждого реле.
2. **Задержка после включения**:
   - После включения всех реле, задержка 5 секунд для наблюдения за состоянием.
3. **Выключение всех реле одновременно**:
   - Все реле выключаются одновременно.
4. **Задержка после выключения**:
   - Задержка 5 секунд после выключения всех реле.

### Проверки:
1. **Подключение**: Проверьте, что SDA и SCL правильно подключены к Arduino Nano.
2. **Питание**: Убедитесь, что реле получает достаточное питание.
3. **Мониторинг**: Следите за серийным монитором для отладки.

Этот скетч должен включать реле по очереди с задержкой в 1 секунду между ними и выключать все реле одновременно с задержкой в 5 секунд для наблюдения за состоянием.
