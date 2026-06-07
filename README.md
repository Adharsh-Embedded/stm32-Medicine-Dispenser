# Smart Medicine Dispenser with GSM Alert

## Overview

The Smart Medicine Dispenser is an embedded systems project built using the STM32 Nucleo-F446RE. The user can set a medicine time using push buttons. When the scheduled time is reached, the system automatically dispenses a pill, activates a buzzer, and places a missed call through a GSM module to notify both the patient or caretaker.

## Features

* User-configurable medicine schedule
* STM32 Internal RTC for time keeping
* Automatic pill dispensing using a servo motor
* GSM missed-call notification
* Audible alert using a buzzer
* LCD display for time and system status
* Simple button-based interface

## Hardware Used

* STM32 Nucleo-F446RE
* 16×2 LCD with I2C Module
* MG995 Servo Motor
* SIM900A GSM Module
* Buzzer
* 3 Push Buttons

## Working

1. The user sets the medicine time using the Hour and Minute buttons.
2. The Set button confirms the selected time.
3. The STM32 Internal RTC continuously monitors the current time.
4. When the current time matches the scheduled time:

   * The servo motor dispenses the pill.
   * The buzzer alerts the user.
   * The GSM module places a missed call to the registered phone number.

## Button Functions

| Button | Function              |
| ------ | --------------------- |
| Hour   | Increase hour value   |
| Minute | Increase minute value |
| Set    | Confirm medicine time |

## Applications

* Medication reminder systems
* Elderly patient care
* Home healthcare assistance
* Smart healthcare devices

## Future Improvements

* SMS notifications
* Mobile application integration
* IoT-based monitoring

## Author

Adharsh
