# W25QXX SPI FLASH Library for STM32
<br />
I hope use it and enjoy.
<br />
MCU used on tests was STM32L476RG.
The toolchain used was provided by Atollic IDE and STM32CubeMX wizard.
<br />
Tests were done with FreeRTOS and BareMetal.
 <br />
Please Do This ...
<br />
<br />
1) Enable SPI and a Gpio as output(CS pin).Connect WP and HOLD to VCC.
<br />
2) Select "General peripheral Initalizion as a pair of '.c/.h' file per peripheral" on project settings.
<br />
3) Config "w25qxxConfig.h".
<br />
4) Call W25qxx_Init(). 
<br />
5) After init, you can watch w25qxx struct.(Chip ID,page size,sector size and ...)
<br />
6) In Read/Write Function, you can put 0 to "NumByteToRead/NumByteToWrite" parameter to maximum.
<br />
7) Dont forget to erase page/sector/block before write.

