# VThash-checker

Python script to check hashes and files at VirusTotal.

Supported python version: 3
####
Supported hashes: MD5, SHA1, SHA256
####
Be aware that the free API provided by VirusTotal is limited to 4 requests / minute

## Dependencies
Python Modules: pip3 install requests , pip3 install simplejson
#### Ubuntu
```
  sudo apt install python3-simplejson
  sudo apt install python-requests python3-requests python3-requests-unixsocket
```
####
API-KEY from www.virustotal.com

## functions and how to use 
```
* Check single hash
* Check multiple hashes from a txt file
* Hash files and check the hash 

usage: vt-check.py [-h] [--apikey APIKEY] [--hash HASH] [--file FILE]
                   [--mass MASS] [--output OUTPUT]

Checks hashes and files at VirusTotal , supported: MD5,SHA1,SHA256 , all kind
of files

optional arguments:
  -h, --help       show this help message and exit
  --apikey APIKEY  specify the API-KEY from www.virustotal.com
  --hash HASH      checks hash at VT
  --file FILE      hashes file and checks hash at VT
  --mass MASS      reads multiple hashes out of a txt file and checks them at
                   VT , needs --output for results
  --output OUTPUT  specify outputpath for mass-check
 ```
  
###

Published under GNU General Public License v3.0
