# Embedded LED Animation System (PIC18F4520)

## Overview
Development of a real-time embedded system to control multiple LED animations using a PIC18F4520 microcontroller.

## Features
- 6 LED animations: running light, wave, alternation, blinking
- Adjustable speed via potentiometer (ADC)
- Time base: 10 ms using Timer0
- User interface:
  - Matrix keypad
  - Push buttons
- Display:
  - 3 multiplexed 7-segment displays (000–999 counter)

## Architecture
- Modular firmware:
  - Timer module
  - ADC module
  - Animation control
  - I/O handling

## Technical Details
- Language: C (XC8)
- Microcontroller: PIC18F4520
- Real-time control using interrupts and timer scheduling

## Challenges
- Timing accuracy for smooth animations
- Synchronization between display multiplexing and LED control

## Possible Improvements
- Use RTOS for better task management
- Add communication interface (UART / I2C)
