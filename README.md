## Sinitsa PCB Layout

Very broadband receiver, designed to pick up any radio signal in the immediate area. Useful for finding sources of interference.

Improved version of the ["Sinitsa" modification to the Amazing Allband Receiver](http://techlib.com/electronics/sinitsa.htm#Sinitsa).

This represents the diode detector section of the [original Sinitsa](https://cryptomuseum.com/df/sinitsa/index.htm). Adding filters and pre-amplifiers is left to the user.

### Ordering

Download the Gerber files from the `gerbers/` directory. Send them to your PCB manufacturer of choice.

### Parts list and assembly

The following parts need to be populated onto the board.

Once the board is populated and tested:

1. Cover the RF input section with some non-conducting tape. Then put copper or aluminum foil over top. Connect the foil to ground. This will shield the quite sensitive input section from unwanted signals in the area (cell phones, etc).
2. Use epoxy to secure the potentiometers against physical shocks. Their pins are fairly fragile.
3. Cover the whole board in heat shrink tubing. Transparent heat shrink is recommended so the power LED is visible.


|Ref                           |Qnty|Value          |Cmp name                             |Footprint                                                   |Description                                                                                           |Vendor|
|------------------------------|----|---------------|-------------------------------------|------------------------------------------------------------|------------------------------------------------------------------------------------------------------|------|
|BAT1,                         |1   |Battery Clip   |Conn_01x02                           |Connector_PinHeader_2.54mm:PinHeader_1x02_P2.54mm_Vertical  | 9V battery clip|      |
|C1,                           |1   |100pF          |C                                    |Capacitor_SMD:C_0402_1005Metric                             |Unpolarized capacitor                                                                                 |      |
|C2, C4, C5, C8, C9, C10, C11, |7   |1nF            |C                                    |Capacitor_SMD:C_0402_1005Metric                             |Unpolarized capacitor                                                                                 |      |
|C3, C12, C100,                |3   |100nF          |C                                    |Capacitor_SMD:C_0402_1005Metric                             |Unpolarized capacitor                                                                                 |      |
|C6,                           |1   |47nF           |C                                    |Capacitor_SMD:C_0603_1608Metric                             |Unpolarized capacitor                                                                                 |      |
|C7,                           |1   |220uF          |C_Polarized-Device-sinitsa-rescue    |Capacitor_SMD:CP_Elec_6.3x7.7                               |                                                                                                      |      |
|C13,                          |1   |1uF            |C                                    |Capacitor_SMD:C_0402_1005Metric                             |Unpolarized capacitor                                                                                 |      |
|D1,                           |1   |BAT17          |D_Schottky                           |Diode_SMD:D_SOT-23_ANK                                      |Schottky diode                                                                                        |      |
|D2, D3, D4,                   |3   |1N914WT        |1N914WT                              |Diode_SMD:D_SOD-523                                         |75V 0.15A Fast switching Diode, SOD-523                                                               |      |
|IC1,                          |1   |LM358          |LM358                                |Package_SO:SOIC-8_3.9x4.9mm_P1.27mm                         |Low-Power, Dual Operational Amplifiers, DIP-8/SOIC-8/TO-99-8                                          |      |
|J2,                           |1   |KLBR_4         |KLBR_4-LUMBERG_3.5-sinitsa-rescue    |Lumberg_3.5:Lumberg-KLBR_4-0                                |                                                                                                      |      |
|L1,                           |1   |10uH           |L                                    |Inductor_SMD:L_0805_2012Metric                              |Inductor                                                                                              |      |
|L2,                           |1   |39n            |L                                    |Inductor_SMD:L_0402_1005Metric                              |Inductor                                                                                              |      |
|LED1,                         |1   |RED LED        |LED                                  |LED_SMD:LED_0805_2012Metric                                 |Light emitting diode                                                                                  |      |
|R1, R8,                       |2   |10K            |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R2, R3,                       |2   |10M            |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R4, R11, R12, R19,            |4   |100K           |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R5,                           |1   |100            |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R6, R9, R22,                  |3   |220K           |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R7,                           |1   |10             |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R10,                          |1   |3k3            |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R13,                          |1   |200K           |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R14,                          |1   |470K           |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R15, R16, R17, R21,           |4   |5.1K           |R                                    |Resistor_SMD:R_0402_1005Metric                              |Resistor                                                                                              |      |
|R18,                          |1   |10K            |R_Potentiometer-Device-sinitsa-rescue|Potentiometer_THT:Potentiometer_Alps_RK097_Single_Horizontal|                                                                                                      |      |
|R20,                          |1   |100K           |R_Potentiometer-Device-sinitsa-rescue|Potentiometer_THT:Potentiometer_Alps_RK097_Single_Horizontal|                                                                                                      |      |
|T1,                           |1   |MMST2222A-7-F  |BC847W                               |Package_TO_SOT_SMD:SOT-323_SC-70                            |0.1A Ic, 45V Vce, NPN Transistor, SOT-323                                                             |      |
|X1,                           |1   |AMPHENOL 132289|Conn_Coaxial                         |Connector_Coaxial:SMA_Amphenol_132289_EdgeMount             |coaxial connector                                                 |      |

