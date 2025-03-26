# EthicalHacking
Cybersecuirty Ethical Hacking Oeson Learning 

Life cycle:
Reconnaissance and foot-printing --> scanning --> enumeration --> vulnerability analysis -> system hacking  
Gaining Access -> Maintaining Access -> Clearing logs

*Target for learning*
```
target for learning:
https://www.hackthissite.org/
http://testphp.vulnweb.com/
http://testfire.net/index.jsp
```
*Gather information*
```
https://www.stationx.net/google-dorks-cheat-sheet/
https://gist.github.com/sundowndev/283efaddbcf896ab405488330d1bbc06
cache:testphp.vulnweb.com
allintext: hacking tools
Google Hacking Data Base (GHDB) --> https://www.exploit-db.com/google-hacking-database
```
```
| Operador   | Descripción                                                                             | Ejemplo                                |
|------------|-----------------------------------------------------------------------------------------|----------------------------------------|
| `allinurl` | Encuentra páginas que contienen todas las palabras clave especificadas en la URL.       | `allinurl:hackthissite admin login`    |
| `filetype` | Busca archivos de un tipo específico en el sitio web.                                   | `site:hackthissite.org filetype:pdf`   |
| `inurl`    | Encuentra páginas que contienen la palabra clave especificada en la URL.                | `inurl:"email.xls"          |
| `intitle`  | Busca páginas que contienen la palabra clave especificada en el título de la página.    | `intitle:"Index of" pwd.db |
| `inanchor` | Encuentra páginas que contienen la palabra clave especificada en el texto de un enlace. | `inanchor:hackthissite forum`          |
| `intext`   | Busca páginas que contienen la palabra clave especificada en el contenido de la página. | `intext:hackthissite confidential`     |
| `site`     | Restringe los resultados de búsqueda a un sitio web específico.                         | `site:hackthissite.org`                |
| `related`  | Encuentra sitios web relacionados con un sitio web específico.                          | `related:hackthissite.org`             |
```
```
intitle:"index of" password.
inurl:admin.php.
site:yeahhub.com "Steganography"
filetype:pdf "Advanced Network Security"
intext:"about" contact.
link:"example.com".
yahoo.com.cache:https://www.yahoo.com
related:yahoo.com
allintext:username filetype:log
*.log files.

inurl:/proc/self/cwd
filetype:xls inurl:"email.xls"
```
*Scanning day*
```
Port scanning:
20 -> UDP  FTP
22 -> TCP  SSH / FTP
23 -> TCP  Telnet
53 -> UDP  DNS 
80 -> UDP  HTTP
```
```
Types scanning --> port, network, vulnerability
> netcraft.com
> shodan.io
> target used --> https://www.hackthissite.org/    http://altoro.testfire.net

ping facebook.com
host testphp.vulnweb.com
nmap testphp.vulnweb.com
nmap 192.168.116.50-150

list.txt ___________ nmap cheat sheet
testphp.vulnweb.com
192.168.116.50
yahoo.com
192.168.116.150
____________________
nmap -iL list.txt

# Técnicas de escaneo Nmap

| SWITCH | EJEMPLO                | DESCRIPCIÓN                                               |
| ------ | ---------------------- | --------------------------------------------------------- |
| -sS    | nmap 192.168.1.1 -sS   | Escaneo de puerto TCP SYN (Predeterminado)                 |
| -sT    | nmap 192.168.1.1 -sT   | Escaneo de puerto TCP connect (Predeterminado sin privilegios de root) |
| -sU    | nmap 192.168.1.1 -sU   | Escaneo de puerto UDP                                      |
| -sA    | nmap 192.168.1.1 -sA   | Escaneo de puerto TCP ACK                                    |
| -sW    | nmap 192.168.1.1 -sW   | Escaneo de puerto TCP Window                                 |
| -sM    | nmap 192.168.1.1 -sM   | Escaneo de puerto TCP Maimon                                 |

-sL
nmap -sV 192.168.116.150
nmap -A 192.168.116.150
nmap -T3 
hpin3 --scan 55-125 -S 192.168.116.11
hpin3 --scan 55-125 -S -V 192.168.116.11

resources->  https://www.stationx.net/wireshark-cheat-sheet/
```
*Evasion IDS / Firewall*
```
nmap -D RND:5 192.168.116.119
nmap -D RND:10 [objetivo] (Genera un número aleatorio de señuelos)
nmap -D señuelo1, señuelo2, señuelo3, etc. (Especifica manualmente las direcciones IP de los señuelos)

nmap -sT -Pn --spoof-mac 0 192.168.116.119
nmap --badsum 192.168.116.119

Proxy sqiitcher standar --> https://www-proxyswitcher-com.translate.goog/?_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=tc


```

**NFS**
```
man rpcinfo

```













