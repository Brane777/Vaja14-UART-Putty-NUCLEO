# Vaja14-UART-Putty-NUCLEO
Katere dva mostička bi morali odspajkati in kateri dve povezavi pospajkati, da bi lahko uporabili pina Tx/D1 in Rx/D0? SB62 in SB63, SB13 in SB14

V področju Connectivity aktivirajte protokol USART2 kot asinhroni. Katera dva pina sta se pobarvala zeleno oz. se aktivirala? PA2 in PA3. 

V polju Configuration izbranega serijskega vmesnika pustimo privzeto hitrost (Baud Rate), ki znaša 115200 Bits/s.  

Za to funkcijo zapišite ukaz za vklop/izklop zelene LED (pomagajte si z metodo toggle, glej vaja0a): HAL_GPIO_TogglePin(GPIOA, GPIO_PIN_5);

Dodajte še ukaz za zakasnitev s funkcijo Delay iz knjižnice HAL, in sicer 2 sekunde (glej vaja0a): HAL_Delay(1000);

Program dopolnite tako, da boste SAMO ob pritisku na tipko USER poslali vaši imeni preko USART protokola na terminal odjemalca Putty. Napišite tudi spremembo kode v vaš komentar githuba! 

Komentar:
