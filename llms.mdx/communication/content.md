# Communication (/communication)









The four PYNQ boards sit in the cradle backbone and exchange heartbeat, crying, decision, and command signals. Two topologies are under evaluation.

## Full system [#full-system]

<img alt="Full system block diagram" src="__img0" />

The cradle sensors (photo detector, mic) feed S1 and S2; S1 and S2 send SIG_HR and SIG_CR to S3; S3 sends SIG_CMD to S4; S4 drives the cradle motors with two 1 kHz PWM signals.

## Option 1: shared UART line [#option-1-shared-uart-line]

<img alt="Option 1: shared UART line" src="__img1" />

Every board has its own TX and RX on the backbone, plus a common ground. UART is point-to-point, so addressing and turn-taking are built on top of it: each board gets a 4-bit address and every frame carries a destination.

## Option 2: I2C link [#option-2-i2c-link]

<img alt="Option 2: I2C link" src="__img2" />

One shared data wire (SDA) and one clock wire (SCL) with a common ground. S3 acts as the master, S1, S2 and S4 as slaves. Addressing is built into the protocol, so no frame header is needed.
