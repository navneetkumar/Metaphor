# Metaphor (Metasploit Exploit)
Metaphor - Stagefright with ASLR bypass
By Hanan Be'er from NorthBit Ltd.
Converted by Timothy Higinbottom

Link to whitepaper:
https://raw.githubusercontent.com/NorthBit/Public/master/NorthBit-Metaphor.pdf

Twitter:
https://twitter.com/High_Byte

Metaphor's source code is now released!
The source include a PoC that generates MP4 exploits in real-time and bypassing ASLR.
The PoC includes lookup tables for Nexus 5 Build LRX22C with Android 5.0.1. Server-side of the PoC include simple PHP scripts that run the exploit generator - I'm using XAMPP to serve gzipped MP4 files. The attack page is index.php.

Eventually we will add more data to the lookup table.

The exploit generator is written in Python and used by the PHP code.

##Note:
Conversion is in progress. This is not stable for use yet.


```sh
usage: metaphor.py [-h] [-c CONFIG] -o OUTPUT {leak,rce,suicide} ...

positional arguments:
  {leak,rce,suicide}    Type of exploit to generate

optional arguments:
  -h, --help            show this help message and exit
  -c CONFIG, --config CONFIG
                        Override exploit configuration
  -o OUTPUT, --output OUTPUT
```

Credits:
To the NorthBit team
E.P. - My shining paladin, for assisting in boosting this project to achieve all the goals.
