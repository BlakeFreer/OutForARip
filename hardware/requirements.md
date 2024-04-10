# Hardware & Electronics

- [Hardware \& Electronics](#hardware--electronics)
  - [Requirements](#requirements)
    - [Functional](#functional)
    - [Mechanical / Electrical](#mechanical--electrical)

## Requirements

### Functional

- Data Logging
  - All data must be timestamped.
  - Must log CAN messages.
    - Firmware should allow configuration of messages of interest to avoid flooding the storage.
  - Must allow data to be stored without power and transferred to another device.
    - Data must be stored in a useful format.
  - Should record global position (ex GPS) frequently.
    - If GPS is available, then use its clock for timestamps.
  - Should record 9dof IMU data (acceleromter, gyroscope, magnetometer) frequently.
- Should indicate several statuses.
  - Power, error, storage full

### Mechanical / Electrical

- Rigidly attach to any OBD-II port.
- Receive power from the port.
  - Require no additional power cables (ex. cannot use the cigarette lighter for 12V)
- Small enough to leave in place permanently without interfering with driving.
  - Cannot have a cable that hangs down.
  - The whole device should be "small" and unnoticeable when mounted.
- The device should consume negligible power when the vehicle is off.
  - Must not cause the battery to drain.
- Must be strong enough to withstand dozens of insertions and removals.
