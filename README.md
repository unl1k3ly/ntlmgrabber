# NTLMgrabber

**NTLMgrabber** is just a docker build automation. Original word was done by https://github.com/ValdikSS/p0f-mtu-script. So all creds goes to VakdukSS.

The project will collect NetNTLM* hashses and display back to the user. A TCP p0f daemon will be running tying to get your SO based on packages signatures. A live example can be found at: http://witch.valdikss.org.ru/

To build the dock is very simple! On a VPS, just start the dock as:

`docker run -it -p 8080:8080 -p 80:80 -p 445:445 -p 443:443 unl1k3ly/ntlmgrabber:v2 -s servername/IP -i eth0` 

After that, browse to http://servername:8080.

Happy Hacking !
