# PLC-seven-segment-display
This is a project developed for the Siemens SIMATIC S7-1500, controlling a seven-segment display.
Input 1.0 selects progam 1, input 1.1 selects program 2. The display is connected to outputs 4.0 - 4.7.

## Program 1:
The program turns input from the ports 0.0 - 0.7 into a ascii character and outputs it to the display.
```
"printChar"(input := "BCDToChar"(v1 := "i1", v2 := "i2", v3 := "i3", v4 := "i4", v5 := "i5", v6 := "i6", v7 := "i7", v8 := "i8"));
```

## Program 2:
The program writes a String to the display. The characters are displayed with a delay of 1 second between each character.
```
"printString"(input := 'Hello World.');
```
