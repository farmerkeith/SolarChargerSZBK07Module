# Solar-charger-SZBK07Module
MPPT Solar charger based on a design by zopinter 
This design uses a commercial DC-DC converter module coded SZBK07, and Arduino Nano for control.
It also has a supplementary input from mains supply controlled from the Nano, and a controlled Load output.
Reverse current flow to the SZBK07 converter module and to the mains supply is prevented by "MOSFET diodes" each consisting of an IRF4905 MOSFET controlled by two BJTs. 
Current flow to and from the battery is monitored, in addition to the solar panel voltage and current and battery voltage essential to the operation of the MPPT algorithm.

# Peripherals
Battery temperature is monitored with a DS18B20 sensor and used to adjust battery set points.
Operational data logging is provided by a micro SD card, with time stamps from a Tiny RTC module using a DS1307 IC. 
An LCD character display provides status information. A push button turns on the backlight of the LCD, saving power when the LCD is not required to be on. 

# Schematic
The schematic circuit diagram has been prepared using KiCad. 
For more information about controlling the output of the SZBK07 module, please see my Instructable on controlling DC converter modules at https://www.instructables.com/id/Controlling-DC-Converter-Modules/ 
