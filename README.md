# stm_32_with_hm_10

This repo contains sample code that runs on an STM32 Nucleo F446RE board which is connected to a DSD-TECH HM_10 BLE module via UART. For this setup, the UART will be in DMA mode. From the HM_10 datasheet, if the DSD-TECH module is powered but not connected, if you send the string "AT" via UART, you should get an "OK" response. This is used to test the UART communication between the board and the HM_10 module.
We will then send a string, "Hello from STM32" every second and use a Raspberry Pi to communicate with this module and read the data thereby demostrating a transmission of data via BLE.
