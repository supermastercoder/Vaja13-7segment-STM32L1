# Vaja13-7segment-STM32L1

2b)
segment A: PA1
segment B: PA2
segment C: PA3
segment D: PA4
segment E: PA5
segment F: PA6
segment G: PA7

2c)
naš prikazovalnik je skupna katoda

2e)
števka|abcdefg|PA7,PA6,PA5,PA4,PA3,PA2,PA1,PA0|HEX
   0   1111110  0   1   1   1   1   1   1   0  0x007E
   1   0110000  0   0   0   0   1   1   0   0  0x000C
   2   1101101  1   0   1   1   0   1   1   0  0x00B6
   3   1111001  1   0   0   1   1   1   1   0  0x009E
   4   0110011  1   1   0   0   1   1   0   0  0x00CC
   5   1011011  1   1   0   1   1   0   1   0  0x00DA
   6   1011111  1   1   1   1   1   0   1   0  0x00FA
   7   1110000  0   0   0   0   1   1   1   0  0x000E
   8   1111111  1   1   1   1   1   1   1   0  0x00FE
   9   1111011  1   1   0   1   1   1   1   0  0x00DE
   
3e)
Ukaz GPIOA -> ODR pomeni, da na portu GPIOx-u nastavljamo ali
preberemo stanje pinov v določenem portu. V našem primeru vstavljamo
šestnajstiško vrednost (ker je GPIOA 16-bitni) za vsako števko, ki
jih STM32CubeIDE nato prebere, pretvori v binarno vrednost in s tem
daje stanje pinov od PA0 do PA15.

4e)
Ko pritisnemo črno tipko (RESET), se koda ustavi in zažene ponovno.

slika pinouta:

<img width="559" height="428" alt="image" src="https://github.com/user-attachments/assets/cb3cdecb-08d4-48a7-ac7d-9eba5b60bd30" />


posnetek delovanja, ko pritisnemo črno tipko:




https://github.com/user-attachments/assets/9b9606ef-5bf2-4d26-9ba2-7f0c19b6fcc9

