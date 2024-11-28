# [Snowing!](https://dreamhack.io/wargame/challenges/241)
This challenge gave me a zip file contains ```flag.txt``` and ```Snow.jpeg```. First, i thought the flag maybe hide inside the picture so i inspected this file using ```EXIF Thumnnail Extractor```, ```xxd``` and ```exiftool``` but nothing in there.  
After that, i focus on the hint which is mentions about whitespace so i decoded txt file using white space decoder named ```stegsnow``` and obtained the flag.  
```linux  
user@LAPTOP-TL39B5OL:/mnt/c/Users/Hoang Quy/Downloads$ stegsnow -C flag.txt
SnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowDH{w0w_1t_Sn0w5}SnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnowSnow  
```  
## FLAG: **```DH{w0w_1t_Sn0w5}```**
