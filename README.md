# IoT26-HW01

## Control Raspberry Pi Digital Outputs with Python

## 1. Objective

The objective of this assignment is to control Raspberry Pi GPIO pins as digital outputs using Python.

In this project, an LED is connected to a Raspberry Pi GPIO pin and controlled using the `gpiozero` library.

## 2. Components

- Raspberry Pi
- LED
- Resistor
- Breadboard
- Jumper wires

## 3. GPIO Pin

| Component | GPIO Pin |
|---|---|
| LED | GPIO14 |

## 4. Source Code

```python
from gpiozero import LED
from time import sleep

led = LED(14)

while True:
    led.on()
    sleep(1)

    led.off()
    sleep(1)
```

## 5. How to Run

```bash
python3 HW1.py
```

## 6. Result

The LED connected to GPIO14 turns on and off repeatedly every second.

This confirms that the Raspberry Pi GPIO pin was successfully controlled as a digital output.

## 7. Screenshots and Evidence

### Source Code Screenshot

![HW1 Code](images/hw1_code.png)

### Running Program Screenshot

![HW1 Run](images/hw1_run.png)

### Raspberry Pi LED Result

![HW1 Result](images/hw1_result.jpg)

## 8. Members

- 장동현 / AI·소프트웨어학부 소프트웨어전공
- 임규민 / AI·소프트웨어학부 인공지능전공
- 이형호 / AI·소프트웨어학부 인공지능전공
