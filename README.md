# Fleeboard
<p align="center">
  <img width="420" height="595" alt="image" src="https://github.com/user-attachments/assets/c97c900b-bddb-4bbb-9ac9-b35d8af7d2cf" />
</p>

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
**Sidenote for reviewers**
_(There is a chance that ktron.in does not accept the hcb money if it happens then i will pay my self)_

# Bill of Materials (BOM)

| Component | Footprint | Qty | Value | Price | Supplier | Link |
|------------|-----------|-----|--------|--------|----------|------|
| Capacitors | 0402 | 13 | 100nF | ₹34.84 | Robu | [GRM155R71C104JA88D](https://robu.in/product/grm155r71c104ja88d-murata-electronics-16v-100nf-x7r-%c2%b15-0402-multilayer-ceramic-capacitors-mlcc-smd-smt-rohs/) |
| Capacitors | 0402 | 2 | 10µF | ₹27.00 | Robu | [CC0402MRX5R5BB106](https://robu.in/product/cc0402mrx5r5bb106-yageo-cap-smd-mlcc-10-%c2%b5f-6-3-v-0402-1005-metric-20-x5r-cc-series/) |
| Capacitors | 0402 | 2 | 33pF | ₹12.00 | Robu | [GRM1555C2A330JA01D](https://robu.in/product/grm1555c2a330ja01d-murata-electronics-100v-33pf-null-%c2%b15-0402-multilayer-ceramic-capacitors-mlcc-smd-smt-rohs/) |
| USB-C port | USB_C_Receptacle_HRO_TYPE-C-31-M-12 | 1 | USB_C_Receptacle_USB2.0_14P | ₹54.00 | Robu | [TYPE-C-31-M-22](https://robu.in/product/type-c-31-m-22-hroparts-5a-1-surface-mount-right-angle-16p-female-30%e2%84%8385%e2%84%83-type-c-smd-usb-connectors-rohs/) |
| Pin headers | PinHeader_1x20_P2.54mm_Vertical | 2 | Conn_01x20 | ₹28.00 | Robu | [Pin Header](https://robu.in/product/1-month-warranty-898/) |
| Pin headers | PinHeader_1x03_P2.54mm_Vertical | 1 | Conn_01x03 | ₹11.97 | Robu | [Pin Header](https://robu.in/product/ph2-54-01-08pzd-xunpu-straight-policy-2-5mm-8p-6mm-40%e2%84%83105%e2%84%83-3mm-2-54mm-black-brass-single-row-1x8p-pluginp2-54mm-pin-headers-rohs/) |
| Resistors | 0402 | 2 | 27Ω | ₹10.26 | Robu | [AC0402JR-0727RL](https://robu.in/product/ac0402jr-0727rl-yageo-res-thick-film-0402-27-ohm-5-0-063w1-16w-%c2%b1100ppm-c-pad-smd-t-r-automotive-aec-q200/) |
| Resistors | 0402 | 2 | 5.1kΩ | ₹11.52 | Robu | [CRCW04025K10FKEDC](https://robu.in/product/crcw04025k10fkedc-vishay-smd-chip-resistor-5-1-kohm-%c2%b1-1-63-mw-0402-1005-metric-thick-film-general-purpose/) |
| Resistors | 0402 | 2 | 1kΩ | ₹11.67 | Robu | [RT1206FRE071KL](https://robu.in/product/rt1206fre071kl-yageo-smd-chip-resistor1-kohm%c2%b1-1250-mw1206-3216-metricthin-film/) |
| Resistors | 0402 | 1 | 10kΩ | ₹10.14 | Robu | [AC0402FR-0710KL](https://robu.in/product/ac0402fr-0710kl-yageo-res-thick-film-0402-10k-ohm-1-0-063w1-16w-%c2%b1100ppm-c-pad-smd-t-r-automotive-aec-q200/) |
| SW_push button | SW_Push_SPST_NO_Alps_SKRK | 2 | Push Button | ₹354.00 | LionCircuits | [SKRKAHE020](https://www.lioncircuits.com/parts/SKRKAHE020) |
| SCU Brain | QFN-56-1EP_7x7mm_P0.4mm_EP3.2x3.2mm | 1 | RP2040 | ₹68.00 | Robocraze | [RP2040](https://robocraze.com/products/raspberry-pi-rp2040-microcontroller-ic-chip?variant=40531158040729) |
| voltage regulator | SOT-23 | 1 | MCP1700-3302E/TT | ₹78.00 | Robu | [MCP1700T-3302E/TT](https://robu.in/product/mcp1700t-3302e-tt-microchip-technology-3-3v-250ma-fixed-output-ldo-linear-voltage-regulator-3-pin-sot-23/) |
| Memory | Winbond_USON-8-1EP_3x2mm_P0.5mm_EP0.2x1.6mm | 1 | W25Q128JVS | ₹294.00 | Robu | [W25Q128JVSIQ](https://robu.in/product/w25q128jvsiq-winbond-electronics-serial-nor-flash-memory-dual-quad-spi-3v-128mbit-133mhz-8pin-soic/) |
| crystal oscillator | Crystal_SMD_3225-4Pin_3.2x2.5mm | 1 | 12MHz Crystal | ₹48.00 | Robu | [OT2JI-111-12M](https://robu.in/product/ot2ji-111-12m/) |
| N/A | Shipping&Taxes | N/A | N/A                                    | ₹700+39$ | N/A | N/A |

## Estimated Total Cost

**≈ ₹1,900.00**

> Prices may vary over time and based on stock availability.


# Problems I Faced
I faced a lot of problems in this project i started with some differnt idea in my mind of building my own thing like a desktop companion and made the project to complicated for me and i tried to work it out a lot made it through the pcb but then it was js out of my league then i asked sam liu if i can change up my mind and do something about it or change the project completely so what i did i took the knowledge for the hardware fromt the blueprint guide credits to team that built that and did a little bit of changes to it and this fleeboard was invented




