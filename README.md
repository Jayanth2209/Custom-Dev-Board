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

### Programming ESP32 using an Arduino UNO
#### Connections:
* Arduino 5V --> VIN of CDB       
* Arduino GND --> GND of CDB       
* Arduino RX --> RXD of CDB      
* Arduino TX --> TXD of CDB      
* Arduino RESET --> Arduino GND       
* GND --> D0 of CDB
  
Continue by following this [link](https://technoreview85.com/how-to-program-esp-32-cam-using-arduino-uno-board/)       

#### Code for RGB-LED on Custom Dev Board 
```
int red = D6;
int green = D7;
int blue = D8;
 
// the setup routine runs once when you press reset:
void setup()
{
// initialize the digital pin as an output.
pinMode(red, OUTPUT);
pinMode(green, OUTPUT);
pinMode(blue, OUTPUT);
digitalWrite(red, HIGH);
digitalWrite(green, HIGH);
digitalWrite(blue, HIGH);
}
 
// the loop routine runs over and over again forever:
void loop() {
digitalWrite(red, LOW); // turn the LED on 
delay(1000); // wait for a second
digitalWrite(red, HIGH); // turn the LED off by making the voltage LOW
delay(1000); // wait for a second
digitalWrite(green, LOW); // turn the LED on 
delay(1000); // wait for a second
digitalWrite(green, HIGH); // turn the LED off by making the voltage LOW
delay(1000); // wait for a second
digitalWrite(blue, LOW); // turn the LED on
delay(1000); // wait for a second
digitalWrite(blue, HIGH); // turn the LED off by making the voltage LOW
delay(1000); // wait for a second
}

```    

