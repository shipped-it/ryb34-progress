# Submodules (/submodules)





## S1 Heartbeat [#s1-heartbeat]

Extracts heart rate from the LED signal; conditions its own signal before sending.

Status: In design

## S2 Crying [#s2-crying]

Detects and filters cry level from the microphone signal.

Status: In design

## S3 Decision [#s3-decision]

Fuses the two processed values into a (frequency, amplitude) decision; timestamps both inputs so misalignment shows on the LCD.

Status: In design

<Callout type="info">
  TODO: circuit will be added
</Callout>

## S4 Motor drivers [#s4-motor-drivers]

Converts the (F, A) decision into two 1 kHz PWM signals on the motor-control connections; cradle supplies motor power.

Status: In design
