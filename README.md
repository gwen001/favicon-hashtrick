# favicon-hashtrick

Returns the hash of a given favicon file and performs IP search on Shodan.

```
$ python3 favicon-hashtrick.py <url>
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
