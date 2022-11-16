<p align="left">
    <img src="https://img.shields.io/badge/python-v3-blue" alt="python badge">
    <img src="https://img.shields.io/badge/license-MIT-green" alt="MIT license badge">
    <a href="https://twitter.com/intent/tweet?text=https%3a%2f%2fgithub.com%2fgwen001%2fdnspy%2f" target="_blank"><img src="https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fgwen001%2Fdnspy" alt="twitter badge"></a>
</p>

# favicon-hashtrick

Returns the hash of a given favicon file and performs search on Shodan.  
It's a good way to discover IPs and subdomains.

## Install

```
git clone https://github.com/gwen001/favicon-hashtrick
cd favicon-hashtrick
pip3 install -r requirements.txt
```

## Usage

```
$ python3 favicon-hashtrick.py -f <favicon_file>
$ python3 favicon-hashtrick.py -k xxxxxxxxxxxxxxxxxxxxx -v ip_str,hostnames -u <favicon_url>
```

```
usage: favicon-hashtrick.py [-h] [-b FAVFILE64] [-f FAVFILE] [-u FAVURL] [-k SHOKEY] [-v VALUES] [-s]

options:
  -h, --help            show this help message and exit
  -b FAVFILE64, --favfile64 FAVFILE64
                        favicon source file (base64 format)
  -f FAVFILE, --favfile FAVFILE
                        favicon source file
  -u FAVURL, --favurl FAVURL
                        favicon source url
  -k SHOKEY, --shokey SHOKEY
                        Shodan API key
  -v VALUES, --values VALUES
                        values you want separated by comma, default: ip _str, can by: ip_str,http,data,domains,hash,ssl,timestamp,asn,_shodan,transport,os,isp,port,org,ip,tags,hostnames,location
  -s, --silent          silent mode, only results displayed
```

<img src="https://raw.githubusercontent.com/gwen001/favicon-hashtrick/main/preview.png" />

---

Feel free to [open an issue](/../../issues/) if you have any problem with the script.  

