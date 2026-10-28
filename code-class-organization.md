

# Code Class Orgaanization



## Method Order

Methods should appear in the following order

- Constructor 
-  periodic()
- idle() Command
- Other  Commands
- Getters and Setters
- Public functions
- Private functions
- simulationInt()
- simulationPeriodic()

## Class Level Variables
- Each class should containt a variable named `table` with the name of the table being the name of the class. \
`private final TelemetryTable table = Telemetry.getTable("name-of-class");`

## Logging
- Logging should be done in the periodic() function
- For all mecahanisms the following should be logged
    - motor voltage
    - stator current
    - supply current
- For mechanisms using PID or MagicMotion control, the following should be additionally logged
    - position or felocity (depending on control type)
    - closed loop reference