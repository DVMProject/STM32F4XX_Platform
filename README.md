# STM32F4XX Platform Library 

This is the STM32F4XX Platform Library with just the needed code for the DVM firmware projects.

The source of this package can be found here:
http://www.st.com/en/embedded-software/stsw-stm32065.html

In order to run the DVM firmware correctly, there are the following modifications already done in this package:

1) STM32F4XX_Platform/Device/startup/startup_stm32f4xx.c :
	- Added C++ global constructors support
	- Changed initial stack pointer

2) STM32F4XX_Platform/Device/system_stm32f4xx.c :
	- Changed PLL_M definition (support "integer" only crystal frequencies: 8, 12, 16 MHz, etc)

3) STM32F4XX_Platform/Device/stm32f4xx_conf.h :
	- Peripheral header file inclusions

