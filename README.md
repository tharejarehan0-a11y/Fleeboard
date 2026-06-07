# Flipboard

https://github.com/user-attachments/assets/660d7121-47da-4f55-9c74-c2678141ec92

<img width="1920" height="1080" alt="card-Photoroom" src="https://github.com/user-attachments/assets/04146464-0e27-4a6b-9aa1-5cdf27326438" />

# Why did i create this
I wanted a good starter project into a little more hardware and found the rp2040 soc with which i could design my own custom devboard but it's a little different as it has it's pin headers upwards thus is the name **FlipBoard** .The only difference between this and other devboards is the pinheaders . It's not something that could benefit people a lot but is just a experiment of going unconventional and seeing how it affects the board 

# Schematics
I started with the schematics and found out about the four main components of it the soc RP2040 , The memory , The Crystal Oscillator , USB-C Connector and the voltage regulator and the pin headers 

this is how u will be able to create this you add the rp2040 and add all the decoupling capcitors to the +3v3 and the +1v1 pins and then you add the crystal oscillator and attach it to the XIN and XOUT pins and add capcitors for reducing the noise and precise vibrations then you add the memory to it and attach the pins as the SPI Model says and attach the pin to the SPI pins of the memory and then you add the usb c connector and you go with the voltage regulator so as to reduce the current from +5v to +3v3 

<img width="3508" height="2480" alt="image" src="https://github.com/user-attachments/assets/3bef6af1-d218-4f4b-a041-c6e48ef9cd34" />

# PCB <br>

**Footprints** <br>

Then while routing u use the footprints <br>
1. Memory - Winbond_USON-8-1EP_3x2mm_P0.5mm_EP0.2x1.6mm <br>
2. Voltage regulator - SOT-23 <br>
3. SOC - QFN-56-1EP_7x7mm_P0.4mm_EP3.2x3.2mm <br>
4. Crystal Oscillator - Crystal_SMD_3225-4Pin_3.2x2.5mm <br>
5. Capacitors - C_0402_1005Metric <br>
6. Resistors - R_0402_1005Metric <br>
7. Push Button - SW_Push_SPST_NO_Alps_SKRK <br>
8. USB - C - USB_C_Receptacle_HRO_TYPE-C-31-M-12 < br>
9. Pin Header Bottom - PinHeader_1x03_P2.54mm_Vertical <br>
10. Pin Headers ( Sides ) - PinHeader_1x20_P2.54mm_Vertical <br>

<img width="1470" height="956" alt="Screenshot 2026-06-05 at 6 58 44 AM" src="https://github.com/user-attachments/assets/bd05da8d-e7d3-45d1-b2b6-b564f55adcbf" />
<br>
# BOM <br>

