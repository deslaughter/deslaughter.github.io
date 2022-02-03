---
title: "Electronics"
weight: 2
---

# Electronics

## Gear Motors

Two worm drive gear motors are used to position the sled on the workspace. The motors change the length of the chain supporting the router sled which causes the sled to move. These motors must produce sufficient torque to support the sled at any location on the workspace. Hall effect encoders on the DC motor shaft are used to determine speed and position of the output shaft. A worm-gear based gearbox is used so the weight of the sled cannot back-drive the DC motor.

This [DC 24V 28RPM 50Kg.cm](https://www.amazon.com/uxcell-50Kg-cm-Self-Locking-Encoder-Reduction/dp/B0788CTS4V) gear motor was selected as it provides sufficient torque and speed. The product comes with minimal documentation which is summarized in the following sections. [Mounting brackets](https://www.amazon.com/gp/product/B073NZ81M9/) were also purchased to attach the gear motors to the frame.

{{< figure src="./gear-motors/gearmotor.jpeg" caption="Gear Motor" width="400" >}}


### Specifications

The gear motor product number is GW4058-31ZY 24V 1:280.

| Specification                 | Value         |
|-------------------------------|---------------|
| Voltage                       | 24V DC        |
| Wattage                       | 35W           |
| Reduction Ratio               | 1:280         |
| No-Load Speed - Motor (RPM)   | 8000          |
| No-Load Speed - Output (RPM)  | 28            |
| No-Load Current (A)           | <0.25         |
| Rated Torque (kg-cm)          | 50            |
| Rated Speed (RPM)             | 22            |
| Rated Current (A)             | <1.2          |
| Stall Torque (kg-cm)          | 40 (70)       |
| Stall Current (A)             | 4.4           |
| Output Shaft Diameter         | 8mm D-type    |
| Output Shaft Length           | 15mm          |

{{< figure src="./gear-motors/dimensions.jpeg" caption="Dimensions" width="400" >}}

### Encoder

The Hall effect encoder, connected to the DC motor driveshaft, outputs 11 pulses per revolution (PPR) [^1]. This is equivant to 44 counts per revolution (CPR). The 44 CPR will be used in this application to maximize the control resolution.

| Specification                 | Value           |
|-------------------------------|-----------------|
| Encoder Type                  | Hall Sensor     |
| Encoder Input Voltage         | 3.3V - 5V       |
| Encoder Output                | 11 PPR (44 CPR) |
 
{{< figure src="./gear-motors/encoder.jpeg" caption="Hall Effect Encoder" width="400" >}}

[^1]: [What’s the Difference Between an Incremental Encoder’s PPR, CPR, and LPR?](https://www.cuidevices.com/blog/what-is-encoder-ppr-cpr-and-lpr)

### Wiring

The following table describes the wires connecting to the gear motor plug.

| Pin | Color         | Description                                   |
|-----|-------------- |---------------------------------------------- |
|  1  | Red Wire      | M1 - Positive power supply of motor           |
|  2  | Black Wire    | GND - Encoder negative power supply           |
|  3  | Yellow Wire   | C1 - Signal feedback                          |   
|  4  | Green Wire    | C1 - Signal feedback                          |   
|  5  | Blue Wire     | VCC - Encoder positive power supply (3.3-5V)  |
|  6  | White Wire    | M2 - Negative power supply of motor           |
 
{{< figure src="./gear-motors/wiring.jpeg" caption="Wiring" width="400" >}}


## DC Driver

[160W 2-Channel DC Motor Driver](https://www.droking.com/160W-2-Channel-DC-Motor-Driver-Module-Positive-Negative-PWM-Speed-Regulation-Optocoupler-Isolation-Dual-H-bridge-Motor-Controller)