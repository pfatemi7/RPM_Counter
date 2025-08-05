# RPM_Counter
RPM counter using Hall effect sensor

#  Simple RPM Counter with Hall Sensor & LCD (Arduino)

This is a small project that measures the RPM (Revolutions Per Minute) of a rotating object using a Hall effect sensor and displays it on a 16x2 I2C LCD screen.

---

## What It Does

- Counts how many times a magnet passes the Hall sensor (i.e., how many rotations occur).
- Calculates RPM using time intervals.
- Displays:
  - Current RPM
  - Total number of rotations
  - Elapsed time (in seconds)

---

##  How It Works

Every time the magnet passes the Hall sensor, an **interrupt** is triggered. After a few rotations (default = 2), the time taken is used to calculate RPM, and the result is shown on the screen.

The display updates in real time and tracks total revolutions + time since startup.

---

##  Wiring Overview

| Component       | Arduino Pin        |
|----------------|--------------------|
| Hall Sensor D0 | D2 (Digital Pin 2) |
| LCD (I2C)      | Uses A4 (SDA), A5 (SCL) on Uno |

Make sure to connect power (VCC, GND) properly.

---


## 📝 License

This project is open-source under the [MIT License](LICENSE). Feel free to use, remix, or build on it — just give credit!

---
