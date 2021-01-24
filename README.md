# Custom-Dev-Board
Getting started with the ESP32 based Custom Dev Board     

![Custom Development Board - Based on ESP32 WROOM ](https://github.com/Jayanth2209/Custom-Dev-Board/blob/main/Images/Custom%20Dev%20Board%20-%20Copy.png)


### Interfacing Custom Dev Board with External CP2102 USB to TTL UART Serial Converter    
#### Connections:        
* VIN of CBD --> External +5V Supply
* GND of CBD --> GND of USB-UART
* TXD of CBD --> RXD of USB-UART
* RXD of CDB --> TXD of USB-UART

##### References:
[ESP32 with FTDI Programmer](https://electronics.stackexchange.com/questions/448187/esp32-with-ftdi-programmer)       
[ESP Flasher Test Procedure](https://github.com/SuperHouse/ESPF/blob/main/Tests/Test-Procedure.md)


