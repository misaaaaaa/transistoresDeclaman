# transistoresDeclaman
circuito para instalación sonora basada en compuertas NAND y sistemas imán-bobina caseros

# ruidoRupestre

**Tarjeta de presentación**

Circuito activador de sistema iman-bobina en base a circuito de compuertas NAND y 555 en modo monostable

También utilizada en obra ["Transistores en tránsito"](https://misaa.cc/projects/transistoresentransito.html) (MAC 2025), controlando bobinas suspendidas en la pared

![foto](./front.jpg)

## Esquemático

![sch](./sch.png)

- Control de frecuencia de 3 osciladores por medio de trimpots

- Visualización de estados por medio de LEDS

- Poesía basada en Jussi Parikka

### Issues versión JLC Y44-2398046A 

- Pin 5 de 555 NO debe ir a tierra directamente

- Q1 tiene comportamiento extraño. No ubicar

- D13 es demasiado brillante, se recomienda no instalar. Se podría instalar una resistencia más grande en R14


## BOM

| Referencia  | Valor          | Huella                                        | Cantidad |
|-------------|----------------|-----------------------------------------------|----------|
| R1,R2,R3,R5 | 1k             | Resistencia SMD 0805                          |        4 |
| U1          | Socket         | DIP-8                                         |        1 |
| U2          | L7805          | Regulador de voltaje TO-252                   |        1 |
| R4          | 100k           | Resistencia THT                               |        1 |
| D1,D2       | 1N4148         | Diodo                                         |        2 |
| D4,D5       | 1N4007         | Diodo                                         |        2 |
| C2,C4,C7    | 100n           | Condensador                                   |        3 |
| C1          | 1000uf         | Condensador electrolítico                     |        1 |
| C3          | 100uF          | Condensador electrolítico                     |        1 |
| C5,C6       | 10uF           | Condensador electrolítico                     |        2 |
| D3,D6       | LED            | Led 3mm                                       |        2 |
| J4,J5,J6,J8 | JUMPER         | Pin Header                                    |        4 |
| J1,J2       | Barrel_Jack    | Connector_BarrelJack:BarrelJack_Horizontal    |        2 |
| J3          | TERMINAL_BLOCK | TerminalBlock:TerminalBlock_bornier-3_P5.08mm |        1 |
| J7          | JACK_TS        | Jack SJ-3525N                                 |        1 |
| K1          | LEG-12F        | Relé 12V                                      |        1 |
| Q1          | IRFZ44n        | Transitor MOSFET TO-220                       |        1 |
| RV1,RV2     | 100k           | Trimpot RM-065                                |        2 |
| U1          | NE555P         | DIP-8                                         |        1 |

![layout](layout_front.png)

![layout](layout_back.png)
