# :mag: IP-Finder :earth_americas:
<p align="center">
  <img src="https://i.ibb.co/1Mx2r6R/hgffZbb.png"> <br>
  <i>Open Source Intelligence (OSINT) tool</i>
</p>

## Intro
IP-Finder is an Open Source Intelligence (OSINT) tool that helps collect IPs of Enterprise Servers, Operating Systems, and more.
It also reports all the CVEs (with the associated Metasploit module ready-for-run) for which different endpoints are affected.
This tool uses some of the best search engines (Shodan.io, ZoomEye.org, and Censys.io).

## What makes it better?
IP-Finder reduces the number of false positives(often present in Shodan results).
In short, the optimization algorithm on the search calculates the minimum distance between parameters in the search, if that distance is below a certain threshold then that result can be considered valid otherwise it will not be considered.

## Requirements
```
[*] Metasploit Framework
[*] Python version 3

[*] Successfully tested on Kali Linux OS
```

## Install
```
$ git clone https://github.com/Bl4ckM1rror/IP-Finder.git
$ pip3 install -r requirements.txt
```

## Setup
```
[+] SHODAN & ZOOMEYE
Copy your <API_KEY> in config_api.py file

[+] CENSYS
$ censys config
Copy your <Censys_API_ID> and <Censys_API_Secret>
```

## Run
```
$ python3 IP-Finder.py --search (your search) 

Example: $ python3 IP-Finder.py --search "apache 2.4.1"
```
