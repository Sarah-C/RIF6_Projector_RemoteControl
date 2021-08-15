# RIF6 - Projector: remote control commands.
This is the mini Rif-6 projectors remote control commands.

Grabbed using an M5Stack-Core2 with the IR Unit, and IRremoteESP8266.

![image](https://user-images.githubusercontent.com/1586332/129451740-ee0874ca-4235-4ab1-bf4c-c8cfb70324d8.png)


/*       
 * IRremoteESP8266: IRrecvDumpV3 - dump details of IR codes with IRrecv       
 * An IR detector/demodulator must be connected to the input kRecvPin.       
 *       
 * Copyright 2009 Ken Shirriff, http://arcfn.com       
 * Copyright 2017-2019 David Conran       
*/       
       

Actual timings from the transmitter:

![image](https://user-images.githubusercontent.com/1586332/129470960-703b4cec-2df7-43c1-ab0f-0048fce54705.png)
https://codepen.io/SarahC/pen/GRmQxJQ?editors=0010
       
RIF6 Remote control.       
       
IRrecvDump is now running and waiting for IR input on Pin 36       
Library   : v2.7.19       
Protocol  : NEC       

Key       : Power       
Code      : 0xFFA25D (32 Bits)       
uint16_t rawData[67] = {9024, 4506,  570, 582,  542, 582,  518, 606,  518, 606,  518, 606,  518, 606,  518, 606,  518, 610,  518, 1698,  548, 1698,  546, 1700,  546, 1700,  546, 1698,  546, 1700,  546, 1696,  548, 1702,  570, 1674,  546, 610,  516, 1698,  546, 606,  542, 582,  542, 582,  544, 1674,  546, 610,  520, 606,  542, 1674,  570, 582,  542, 1676,  546, 1698,  570, 1674,  572, 582,  520, 1698,  546};  // NEC FFA25D       
uint32_t address = 0x0;       
uint32_t command = 0x45;       
uint64_t data = 0xFFA25D;       
       
Key       : Mute       
Code      : 0xFF4AB5 (32 Bits)       
uint16_t rawData[67] = {9044, 4484,  572, 580,  544, 580,  544, 580,  544, 580,  542, 582,  544, 580,  520, 604,  542, 586,  544, 1674,  570, 1674,  570, 1676,  570, 1674,  572, 1672,  570, 1674,  546, 1700,  568, 1678,  570, 582,  542, 1672,  572, 580,  542, 580,  542, 1674,  566, 582,  542, 1672,  570, 584,  538, 1674,  564, 580,  534, 1674,  556, 1674,  556, 580,  530, 1672,  558, 582,  524, 1676,  552};  // NEC FF4AB5       
uint32_t address = 0x0;       
uint32_t command = 0x52;       
uint64_t data = 0xFF4AB5;       
       
Key       : Rewind       
Code      : 0xFF30CF (32 Bits)       
uint16_t rawData[67] = {9040, 4480,  572, 578,  544, 580,  542, 580,  542, 582,  542, 580,  544, 580,  544, 578,  544, 584,  544, 1674,  570, 1672,  572, 1670,  572, 1670,  572, 1672,  570, 1670,  572, 1670,  574, 1674,  572, 578,  544, 580,  544, 1672,  572, 1670,  570, 580,  542, 580,  544, 580,  544, 582,  544, 1672,  570, 1670,  572, 578,  544, 580,  544, 1670,  572, 1672,  572, 1670,  572, 1670,  572};  // NEC FF30CF       
uint32_t address = 0x0;       
uint32_t command = 0xC;       
uint64_t data = 0xFF30CF;       
       
Key       : Fast forward       
Code      : 0xFF7A85 (32 Bits)       
uint16_t rawData[67] = {9040, 4482,  570, 582,  542, 580,  544, 556,  568, 556,  568, 580,  544, 580,  542, 582,  542, 584,  542, 1674,  570, 1674,  568, 1674,  572, 1672,  570, 1672,  572, 1674,  570, 1672,  572, 1676,  570, 582,  542, 1674,  570, 1674,  546, 1696,  570, 1672,  570, 582,  542, 1672,  572, 584,  542, 1674,  572, 578,  544, 580,  544, 580,  544, 580,  518, 1698,  570, 580,  542, 1672,  546};  // NEC FF7A85       
uint32_t address = 0x0;       
uint32_t command = 0x5E;       
uint64_t data = 0xFF7A85;       
       
Key       : Up arrow       
Code      : 0xFF52AD (32 Bits)       
uint16_t rawData[67] = {9022, 4476,  572, 578,  544, 578,  544, 578,  544, 578,  542, 580,  542, 580,  542, 578,  544, 582,  544, 1670,  570, 1672,  570, 1668,  570, 1670,  572, 1670,  572, 1670,  570, 1670,  572, 1672,  570, 578,  544, 1668,  572, 578,  542, 1668,  572, 578,  544, 578,  544, 1666,  574, 582,  544, 1668,  572, 578,  542, 1668,  572, 578,  546, 1668,  570, 1668,  574, 576,  546, 1668,  570};  // NEC FF52AD       
uint32_t address = 0x0;       
uint32_t command = 0x4A;       
uint64_t data = 0xFF52AD;       
       
Key       : Left arrow       
Code      : 0xFFE01F (32 Bits)       
uint16_t rawData[67] = {9040, 4484,  570, 580,  544, 580,  544, 580,  544, 580,  544, 580,  544, 580,  544, 580,  542, 584,  544, 1672,  572, 1672,  570, 1674,  572, 1672,  572, 1672,  572, 1672,  570, 1672,  572, 1676,  570, 1674,  570, 1674,  570, 1672,  572, 580,  544, 580,  544, 578,  546, 578,  544, 584,  544, 580,  546, 578,  544, 580,  544, 1672,  570, 1672,  572, 1670,  572, 1672,  572, 1672,  572};  // NEC FFE01F       
uint32_t address = 0x0;       
uint32_t command = 0x7;       
uint64_t data = 0xFFE01F;       
       
Key       : Play / Pause       
Code      : 0xFF18E7 (32 Bits)       
uint16_t rawData[67] = {9042, 4484,  548, 604,  544, 582,  544, 580,  544, 580,  544, 580,  544, 580,  544, 580,  544, 584,  544, 1676,  570, 1672,  570, 1674,  572, 1672,  570, 1676,  572, 1672,  570, 1674,  572, 1676,  572, 580,  544, 580,  546, 578,  544, 1672,  572, 1672,  570, 582,  544, 580,  544, 584,  544, 1672,  572, 1672,  574, 1672,  572, 580,  544, 580,  544, 1672,  572, 1672,  572, 1672,  570};  // NEC FF18E7       
uint32_t address = 0x0;       
uint32_t command = 0x18;       
uint64_t data = 0xFF18E7;              
       
Key       : Right arrow       
Code      : 0xFF906F (32 Bits)       
uint16_t rawData[67] = {9044, 4476,  578, 574,  548, 576,  548, 576,  546, 578,  546, 576,  548, 550,  572, 574,  548, 580,  548, 1668,  574, 1668,  576, 1666,  574, 1670,  576, 1666,  576, 1666,  576, 1666,  576, 1670,  576, 1666,  576, 574,  548, 574,  548, 1668,  576, 574,  548, 574,  548, 576,  548, 578,  548, 576,  548, 1668,  576, 1666,  574, 576,  546, 1666,  576, 1666,  574, 1668,  576, 1666,  574};  // NEC FF906F       
uint32_t address = 0x0;       
uint32_t command = 0x9;       
uint64_t data = 0xFF906F;       
       
Key       : Down arrow       
Code      : 0xFF42BD (32 Bits)       
uint16_t rawData[67] = {9042, 4486,  558, 580,  532, 580,  534, 580,  536, 582,  536, 580,  532, 580,  530, 582,  540, 584,  546, 1672,  572, 1674,  574, 1672,  574, 1672,  572, 1672,  572, 1672,  574, 1670,  574, 1676,  574, 578,  546, 1672,  572, 578,  546, 580,  546, 578,  546, 580,  546, 1670,  576, 582,  546, 1672,  572, 580,  544, 1672,  572, 1674,  572, 1674,  572, 1672,  572, 580,  546, 1670,  572};  // NEC FF42BD       
uint32_t address = 0x0;       
uint32_t command = 0x42;       
uint64_t data = 0xFF42BD;       
       
Key       : Settings       
Code      : 0xFFA857 (32 Bits)       
uint16_t rawData[67] = {9054, 4484,  572, 580,  544, 580,  546, 580,  546, 580,  544, 582,  544, 580,  546, 580,  544, 584,  546, 1674,  572, 1672,  572, 1674,  572, 1674,  572, 1674,  572, 1674,  572, 1674,  572, 1678,  570, 1674,  572, 580,  544, 1674,  570, 558,  570, 1672,  572, 580,  544, 580,  546, 584,  546, 580,  546, 1672,  574, 580,  546, 1672,  572, 580,  546, 1674,  574, 1672,  572, 1674,  574};  // NEC FFA857       
uint32_t address = 0x0;       
uint32_t command = 0x15;       
uint64_t data = 0xFFA857;       
       
Key       : Back       
Code      : 0xFFE21D (32 Bits)       
uint16_t rawData[67] = {9050, 4484,  574, 578,  544, 580,  546, 580,  542, 582,  546, 580,  546, 554,  572, 578,  546, 584,  546, 1674,  572, 1674,  574, 1674,  572, 1674,  572, 1674,  572, 1674,  572, 1674,  572, 1676,  572, 1674,  572, 1672,  574, 1672,  572, 580,  546, 554,  570, 554,  572, 1672,  572, 584,  544, 580,  544, 580,  544, 580,  546, 1674,  574, 1672,  572, 1672,  574, 580,  546, 1672,  574};  // NEC FFE21D       
uint32_t address = 0x0;       
uint32_t command = 0x47;       
uint64_t data = 0xFFE21D;       


