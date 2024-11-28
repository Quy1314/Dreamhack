## [Basic_Forensics_1](https://dreamhack.io/wargame/challenges/518)
The challenge gave me a PNG file of whitebear, my work is trying to discover the flag in there.  
To start, i inspected the file using ```zsteg``` and luckily i obtained the flag.  
```linux
user@LAPTOP-TL39B5OL:/mnt/c/Users/Hoang Quy/Downloads$ zsteg whitebear.png
b1,rgb,lsb,xy       .. text: "DH{Wh!te_Be4r_In_Dream_4ack}W4!teBear"
b2,r,lsb,xy         .. text: "UUUUUEUUUU"
b2,g,lsb,xy         .. text: "UUUUUEUUUU"
b2,b,lsb,xy         .. text: "UUUUUEUUUU"
b2,rgb,lsb,xy       .. text: ["U" repeated 15 times]
b2,rgb,msb,xy       .. text: ["U" repeated 15 times]
b2,bgr,lsb,xy       .. text: ["U" repeated 15 times]
b2,bgr,msb,xy       .. text: ["U" repeated 15 times]
b2,rgba,lsb,xy      .. text: ["W" repeated 20 times]
b2,abgr,msb,xy      .. text: ["W" repeated 20 times]
b3,g,msb,xy         .. file: OpenPGP Secret Key
b3,abgr,msb,xy      .. file: PGP Secret Sub-key -
b4,r,lsb,xy         .. text: "\"#22#322##"
b4,r,msb,xy         .. text: ["f" repeated 10 times]
b4,g,lsb,xy         .. text: "2\"\"323\"\"2#"
b4,g,msb,xy         .. text: ["f" repeated 10 times]
b4,b,lsb,xy         .. text: "#\"#3#\"\"#3\""
b4,b,msb,xy         .. text: ["f" repeated 10 times]
b4,rgb,lsb,xy       .. text: "#\"#\"#\"2\"#323###3#22\"\"2\"##3#\"#2"
b4,rgb,msb,xy       .. text: ["f" repeated 30 times]
b4,bgr,lsb,xy       .. text: "##\"\"\"#\"3\"332####23\"2\"\"3\"3##\"\"3"
b4,bgr,msb,xy       .. text: ["f" repeated 30 times]
b4,rgba,lsb,xy      .. text: "#/\"?\"/2/2/\"?3?#?#/2?3/3/2/\"/2/\"?#?2?\"/3/"
b4,abgr,msb,xy      .. text: "ofofofofofofofofofofofofofofofofofofofof"
```
## Flag: **```DH{Wh!te_Be4r_In_Dream_4ack}```**
