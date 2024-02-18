# ServerVGA
VGA-Adapter der auf einem Touch-Display via SPI das Bild darstellt. 
Minimal und optimal für Server. 

# VGA-Signal

``` 

BUCHSE
             ____________________________________
    ____     \    ( 5) ( 4) ( 3) ( 2) ( 1)      /     ____
   /  _  \    \                                /     /  _  \
  /  / \  \    \     (10) ( 9) ( 8) ( 7) ( 6) /     /  / \  \
  \  \_/  /     \                            /      \  \_/  /
   \_____/       \ (15) (14) (13) (12) (11) /        \_____/
                  \------------------------/
```

1) R
2) G
3) B 
4) ID2
5) G (DDC)
6) G (R)
7) G (G)
8) G (B)
9) 
10) G (Sync)
11) ID0 
12) ID1 (oder DDC: SDA)
13) H-Sync
14) V-Sync 
15) ID 3 (oder DDC - SDC)

Pegel: 0.7V, 75Ohm

ID0    |  ID1   | ID2    | function              |
---    | ---    | ---    | ---                   |
n.c.   | n.c.   | n.c.   | no monitor connected  | 
&nbsp; | GND    | &nbsp; | monochrome (G)        |
GND    | &nbsp;	| &nbsp; | color 800x640         |
GND    | &nbsp;	| GND    | color, 1024x768       |


