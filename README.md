# ULP LoRa HAT PCB Design

The ULP LoRa HAT PCB is designed for 5V sensors to integrate with the ULP LoRa board. However, since the ULP LoRa only provides a 3.3V output voltage, 5V sensors cannot be directly integrated. This issue can be resolved by using a buck-boost converter or a boost converter circuit. In this PCB, the voltage is stepped up from 3.3V to 5V using a boost converter circuit with a TPS61202 IC. Level shifter (SN74LV1T34) is added for UART and GPIO peripherals.


# PCB Testing

- Short circuit test using Multimeter; No short ckt in the PCB.
- Provided 3.3V to the input side and Output voltage is noted (Needed output voltage is 5V); The output voltage is 6.5V.
- Varying the input voltage from 1V to 5V and the output voltage is
noted; The output voltage of the boost converter circuit is varying upto
6.5V (from the datasheet TPS61202 IC provides constant 5V.)
 - Varying the inductors and the output voltage is noted; Variable output
voltage is obtained.The PCB was modified using the TPS6120xEVM-179 datasheet. By varying the input voltage from 1V to 5V, the output voltage remains constant at 6.6V.

