# STM32 Development Process
This repo includes the works that I did with Nucleo-F303K8 card.

# Pin Configurations (in .ioc file)
## LED PIN
PB3: GPIO_Output
## Debug Configauration
System Core -> SYS -> Debug: Serial Wire (If this is not done, you may encounter issues when uploading new code after the initial upload (the processor may enter sleep mode or fail to enter debug mode) )
## Generating Code
Click the Gear Icon (Device Configuration Tool code generation) in the top menu / Project -> Generate Code
Choose “Yes” when the prompt appears. This process generates the necessary C libraries (HAL) in the background based on the settings you selected.

