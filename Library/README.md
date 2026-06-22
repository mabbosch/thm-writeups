# Library (TryHackme)

### Reconocimiento

### Nmap

Empezamos esta máquina vulnerable nivel Easy de Tryhackme con un escaneo de puertos abiertos y versiones con nmap.

```bash
──(root㉿kali)-[/home/kali/THM/library]

└─# nmap -p- --open -sVC --min-rate 3000 -n -Pn 10.10.208.114

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-11-25 18:32 EST

Nmap scan report for 10.10.208.114

Host is up (0.077s latency).

Not shown: 65368 closed tcp ports (reset), 165 filtered tcp ports (no-response)

Some closed ports may be reported as filtered due to --defeat-rst-ratelimit

PORT STATE SERVICE VERSION

22/tcp open ssh OpenSSH 7.2p2 Ubuntu 4ubuntu2.8 (Ubuntu Linux; protocol 2.0)

| ssh-hostkey:

| 2048 c4:2f:c3:47:67:06:32:04:ef:92:91:8e:05:87:d5:dc (RSA)

| 256 68:92:13:ec:94:79:dc:bb:77:02:da:99:bf:b6:9d:b0 (ECDSA)

|_ 256 43:e8:24:fc:d8:b8:d3:aa:c2:48:08:97:51:dc:5b:7d (ED25519)

80/tcp open http Apache httpd 2.4.18 ((Ubuntu))

|_http-title: Welcome to Blog - Library Machine

| http-robots.txt: 1 disallowed entry

|_/

|_http-server-header: Apache/2.4.18 (Ubuntu)

Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .

Nmap done: 1 IP address (1 host up) scanned in 26.78 seconds
