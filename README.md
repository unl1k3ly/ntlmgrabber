# NTLMgrabber

**NTLMgrabber** is just a docker build automation. Original work was done by VakdukSS. So all creds goes to https://github.com/ValdikSS/p0f-mtu-script.

The project idea is to collect NetNTLM* hashes and display back to the user. A TCP p0f daemon will be running as well tying to get the Sistem Operation and connection source details based on packages signatures. A live example can be found at: http://witch.valdikss.org.ru/

To build the dock is very simple! On a VPS, just start the dock as:

 ```
 $ sudo mkdir /data
 $ sudo docker run  -v /data:/data -p 80:80 -p 445:445 -p 443:443  unl1k3ly/ntlmgrabber:v7 -s Domain/IP
 ```
 
After that, browse to http://servername:8080.

Happy Hacking !
