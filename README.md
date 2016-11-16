## Intro ##
**URLSUCKER** sucks all embedded URLs from a given URI or file.

Ideal to parse strings from CSS or JavaScript files as many or all the web crawlers and spiders do not scan through JavaScript code, missing many interesting resources such as API calls, webservices, etc.

So far URLSUCKER is quite useful to pentest Web Applications.

It could be integrated to ZAP or Burp Suite as well. 

## Syntax ##
```
./URLSUCKER ([-u url] | [-f file]) [-v]
```

- Give as a parameter a url (-u) or a file (-f) to scan.
- -v parameter gives you verbose output, showing the response code and the potential URL found

## Example ##
```
./URLSUCKER -u http://localhost/login.js
```


### DISCLAMER ###
Use at your own risk in an environment that you are allowed to attack.

~
spinfoo

