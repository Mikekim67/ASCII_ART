# ASCII_ART


http://busyducks.com/ascii-art-arduinos
for original Arduino UNO ascii art 

=====================Arduino ZERO========================     

                        +-----+     +-----+     
                        | nat |     | prg |   
         +--[PWR]-------| USB |-----| USB |----+
         |              +-----+     +-----+    |
         |         10-pin JTAG                 |
         |         TCK [1][2] GND    A5/SCL[ ] |   C5 
         |         TDO [ ][ ] 3V3    A4/SDA[ ] |   C4 
         |         TMS [ ][ ] RST      AREF[ ] |
         |         N/C [ ][ ] N/C       GND[ ] |
         | [ ]N/C  TDI [9][ ] GND    SCK/13[ ]~|   B5
         | [ ]IOREF                 MISO/12[ ]~|   .
         | [ ]RST                   MOSI/11[ ]~|   .
         | [ ]3V3                        10[ ]~|   .
         | [ ]5v                          9[ ]~|   .
         | [ ]GND                         8[ ]~|   B0
         | [ ]GND                              |
         | [ ]Vin           ++++          7[ ] |   D7
         |                 + ZE +         6[ ]~|   .
         | [ ]A0           + RO +         5[ ]~|   .
         | [ ]A1            ++++          4[ ]~|   .
         | [ ]A2                     INT1/3[ ]~|   .
         | [ ]A3                     INT0/2[ ] |   .
         | [ ]A4      RST SCK MISO     TX>1[ ] |   .
         | [ ]A5      [ ] [ ] [ ]      RX<0[ ] |   D0
         |            [ ] [ ] [ ]              |
         |  ZERO      GND MOSI 5V  ____________/
          \_______________________/
		  

          10-pin JTAG interface 
          TCK [1][2] GND
          TDO [ ][ ] 3V3
          TMS [ ][ ] RST
          N/C [ ][ ] N/C
          TDI [9][ ] GND
         

=====================BP6A Arduino Shield========================     



                                    +-----+     
                                    | USB |   
         +--------------------------|  C  |----+
         |[@]              [@]  [@] +-----+ [@]|
         |BPRST            BTM  [ ]         RST|
         |                      UART    SCL[ ] |   C5 
         |[ ]5V                         SDA[ ] |   C4 
         |[@]3V3                           [ ] |
         |                              GND[ ] |
         | [ ]N/C                  SPI_CLK [ ] |   B5
         | [ ]IOREF                SPI_MISO[ ] |   .
         | [ ]RST                  SPI_MOSI[ ] |   .
         | [ ]3V3                  SPI_CSN [ ] |   .
         | [ ]5v         .             GP_1[ ] |   .
         | [ ]GND    ===== jtag        GP_2[ ] |   B0
         | [ ]GND    =====                     |
         | [ ]                          RX2[ ] |   D7
         |         ++++                 TX2[ ] |   .
         | [ ]    + BP +             BTMODE[ ] |   .
         | [ ]    + 6A +               GP_3[ ] |   .
         | [ ]     ++++              TX_INT[ ] |   .
         | [ ]                       BP_RST[ ] |   .
         | [ ]                          RX0[ ] |   .
         | [ ]                          TX0[ ] |   D0
         | BP6A Arduino Shield                 |
         |     PPG        .  BIA/ECG/GSR  .    |
         |     ()()()()()[]  ()()()()()()[]    |
         |     ()()()()()()  ()()()()()()()    |
         +-------------------------------------+

          10-pin JTAG interface
                           .
          TDI N/C TMS TDO TCK
          [9] [ ] [ ] [ ] [1]
          [ ] [ ] [ ] [ ] [2]
          GND N/C RST 3V3 GND

	              PPG
             VDD_3P3 [1](2) PPG_LED0
            PPG_LED1 (3)(4) PPG_LED2
            PPG_LED3 (5)(6) PPG_INN0
            PPG_INP0 (7)(8) VDD_3P3
                AGND (9)(A) PPG_SHIELD
            PPG_INN1 (B)(C) PPG_INP1


                  BIA/ECG/GSR
            GSR_POUT [1](2) GPA0_INP
            GSR_NOUT (3)(4) GPA0_INN
              GPIO1E (5)(6) GPIO18
              GPIO1F (7)(8)GPIO19
                AGND (9)(A) VDD_3P3
                 El1 (B)(C) EL3
                 EL2 (D)(E) EL4
