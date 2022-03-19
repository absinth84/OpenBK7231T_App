MCU command

----------------------------------------------------
| Field     | Lenght (byte) |     Description      |
----------------------------------------------------
| Header    |      2        |  Fixed 0x55aa        |
| Version   |      1        |  For upgrade and ext | 
| Command w |      1        |
| Data lenght      2        |
| Data      |      xxxx     |
| Checksum  |      1        | byte sum from header to 256


init                55aa00000000ff 
product info        55aa0001000000          55aa00080000
allDps              55AA00080000            55 AA 01 07 00 08 03 02 00 04 00 00 00 2C 44
        
wifi working mode   55aa0002000001
wifi smart          55aa0003000002
wifi ap mode        55aa0003000103
wifi 4 conn router  55aa0003000305
wifi 5 conn r&c     55aa0003000406

set hour            55AA001C00080113020F10041205

temperature 

30grades            55aa00060008020200040000001e15

set target temp 22                    55AA00060008020200040000002C41



on      55AA000600050101000101


temp -1C

//Command: Set date and time
    	//                       OK YY MM DD HH MM SS Weekday
    	//DEC:                   01 19 02 15 16 04 18 05
    	//HEX: 55 AA 00 1C 00 08 01 13 02 0F 10 04 12 05
    	//DEC:                   01 19 02 20 17 51 44 03
    	//HEX: 55 AA 00 1C 00 08 01 13 02 14 11 33 2C 03