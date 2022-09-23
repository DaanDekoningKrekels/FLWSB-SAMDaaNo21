# Onderdelen PCB ontwikkeling

- FLWSB bord 
  
  - Arduino Nano vormfactor
  - USB poort
  - Componenten aan weerszijden
  - LoRaWAN radio naar apart bord

- Bord met Maximum Power Point Tracking voor zonne-energie en Litium Ion batterijen
  
  - USB oplader toevoegen

- Bord voor anemometer aan te sluiten

- Bord voor grondvochtigheid te meten

## FLWSB-SAMDaaNo21

Atsamd 21 bord gebaseerd op de Arduino Nano vormfactor. Alle benodigdheden voor de ATSAMD zitten op dit bord. Alsook male headers om op een breadboard te pinnen, female connectoren om dochterbroden aan te sluiten en een USB C poort.

### USB Poort

Ref: https://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-42261-SAM-D21-USB_Application-Note_AT06475.pdf

Ref schematic checklist: https://ww1.microchip.com/downloads/en/DeviceDoc/SAM-D21DA1-Family-Data-Sheet-DS40001882G.pdf#_OPENTOPIC_TOC_PROCESSING_d10240e380866

![Figure 45-15. Protected USB Interface Example Schematic](/home/daan/Documents/SCHOOL/Applied IoT Projects/FLWSB/assets/Screenshot 2022-09-23 at 14-53-28 SAM D21 Family Data Sheet - SAM-D21DA1-Family-Data-Sheet-DS40001882G.pdf-16639376699902.png)

## Power delivery

LD1117 regelaar van 5V naar 3.3V voor wanneer de USB is aangesloten. 

Schakelt over naar de effitientere 3.3V regelaar die op het POWER DELIVERY bord wordt gezet. Op dezelfde manier als de Arduino UNO werkt.

TODO:

- MOSFETSCHAKELING maken
- OPAMP kiezen
