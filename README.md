## Intro ##
**URLSUCKER** sucks all embedded URLs from a given URI or file.

Ideal to parse strings from CSS or JavaScript files as many or all the web crawlers and spiders do not scan through JavaScript code, missing many interesting resources such as API calls, webservices, etc.

So far **URLSUCKER** is quite useful to pentest Web Applications.

It could be integrated to ZAP or Burp Suite as well. 

## Syntax ##
```
./URLSUCKER [-v] [-t <timeout>] ([-u url] | [-f file])
```

- Give as a parameter a url (```-u```) or a file (```-f```) to scan.
- ```-v``` parameter gives you verbose output, showing the response code and the potential URL found for manual analysis.
- ```-t <timeout>``` parameter establishes a timeout between requests to evade WAF / security systems (in seconds)

## Example ##
```
$ ./URLSUCKER -u http://192.168.1.1/index.php
[ABSOLUTE URL] http://192.168.1.1/help/license.html
[RELATIVE URL] http://192.168.1.1/console.png
[RELATIVE URL] http://192.168.1.1/green.png
[RELATIVE URL] http://192.168.1.1/help.png
[EXTERNAL ABSOLUTE URL] http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd
[RELATIVE URL] http://192.168.1.1/license.png
[RELATIVE URL] http://192.168.1.1/mikrotik_logo.png
[RELATIVE URL] http://192.168.1.1/winbox.png
```


### DISCLAIMER ###
Use at your own risk in an environment that you are allowed to attack.


~
(c) 2018 defensahacker
