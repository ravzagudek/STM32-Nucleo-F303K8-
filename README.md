# STM32 Development Process
This repo includes the works that I did with Nucleo-F303K8 card.

# Blinky LED
## Purpose
To toggle the onboard LED on the STM32F303K8 (PB3) on and off at 2000 ms intervals.
## What I Learned?
-How to use the HAL_GPIO_TogglePin function.
-The convenience of assigning a “Label” in the Pinout settings.
-The logic behind the SysTick timer and HAL_Delay.##
### Pin Configurations (in .ioc file)
#### LED PIN
PB3: GPIO_Output
#### Debug Configauration
System Core -> SYS -> Debug: Serial Wire (If this is not done, you may encounter issues when uploading new code after the initial upload (the processor may enter sleep mode or fail to enter debug mode) )
#### Generating Code
Click the Gear Icon (Device Configuration Tool code generation) in the top menu / Project -> Generate Code
Choose “Yes” when the prompt appears. This process generates the necessary C libraries (HAL) in the background based on the settings you selected.
## Wiring Diagram
The onboard LED was used, no external circuit is required.

# UART-Message
## Purpose

## What I Learned?
### Pin Configurations (in .ioc file)
Connectivity: USART2
Mode: Asynnchronous
Parameters:
-Baud Rete: 115200
-Word Length: 8 Bits (Std)
-Stop Bits: 1 (Std)
### ->Generate Code

### PuTTY
Connection Type: Serial
Serial line: COM Port number can be seen on the Device Manager (Mine is COM9)
Speed: 115200
-> Open 
