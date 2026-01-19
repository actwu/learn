[/]: #(<title>Dom</title>)
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1, user-scalable=no">
<link rel="preload" as='https://cdn.jsdelivr.net/gh/iselang/iselang.github.io@main/num.min.js'/>

[/]: # (<script src="https://iselang.github.io/num.min.js"></script>)

[/]: #(<style>body{margin:auto;padding:0.4em!important;}*:not(last-child){margin-bottom:var(--mar);}*{border:unset;outline:unset;word-break:break-all;}body{margin:auto;background:var(--b);color:var(--f);font-family:var(--font);display:flex;flex-direction:column;padding:5px;box-sizing:border-box;width:100vw;max-width:540px;text-align:center;justify-content:center;place-content:center;align-content:center;min-height:100svh;}</style>)

[/]: #(<script>app('Site');fav(3)</script>)
<link rel="preload" as='style' href="https://actwu.github.io/md2.css"/>
<link rel="stylesheet" href="https://actwu.github.io/md2.css"/>

# ETHICAL HACKING BASICS 101 - ASCII GUIDE

## WEB STACK
html structure  
css style  
javascript behavior  
frontend runs in browser  
backend runs on server  
browser -> server -> database -> server -> browser  

## HTTP METHODS
get    read  
post   create  
put    update  
delete remove  

## COMMON HTTP STATUS CODES
200  ok  
301  redirect  
400  bad request  
401  unauthorized  
403  forbidden  
404  not found  
500  server error  

## HTTP REQUEST PARTS
method  
path  
headers  
body optional  

## COMMON HTTP HEADERS
Host  
User-Agent  
Accept  
Content-Type  
Authorization  
Cookie  
Set-Cookie  

## WEBSITE FILES
index.html  default page  
404.html    not found page  

common paths  
- /index.html  
- /login.html  
- /admin/  
- /api/  
- /uploads/  
- /assets/  
- /robots.txt  
- /sitemap.xml  

## NETWORKING BASICS
ssh       secure remote access port 22  
http      port 80  
https     port 443  
ftp       port 21  
dns       port 53  

vpn       encrypt traffic hide ip  
proxy     middle server  
endpoint  final server or api url  

tcp = reliable, ordered  
udp = fast, no guarantee  

## COOKIES & SESSIONS
cookie = stored in browser  
session = stored on server  
used for login tracking  

token auth  
jwt = json web token  
bearer token in header  

## CRYPTO BASICS
encryption = reversible (AES, RSA)  
hashing    = one way (SHA256, bcrypt)  

never store plaintext passwords  
always use salted hashes  

## BASIC BASH COMMANDS

pwd ls ls -la cd /var/www cd .. touch test.txt mkdir testdir rm test.txt rm -r testdir cp a.txt b.txt mv a.txt /tmp/ cat file.txt less file.txt grep "admin" file.txt find / -name index.html ps aux netstat -tulnp ip a ip route ping example.com traceroute example.com dig example.com

## SSH COMMANDS

ssh user@192.168.1.10 ssh -i key.pem user@host

## CURL COMMANDS

curl http://example.com curl -v http://example.com curl http://example.com/index.html curl -X POST http://example.com/login -d "user=test&pass=1234" curl -X PUT http://example.com/user/1 -d "name=newname" curl -X DELETE http://example.com/user/1 curl -H "Authorization: Bearer TOKEN" http://example.com/api curl http://example.com -o page.html curl http://example.com http://example.com/admin curl -x http://127.0.0.1:8080 http://example.com

## GITHUB GIST COMMANDS

Gist allows you to share data faster


Make gist 

```
export GH_TOKEN="YOUR_TOKEN_HERE"

curl -X POST https://api.github.com/gists 
-H "Authorization: Bearer $GH_TOKEN" 
-H "Content-Type: application/json" 
-d '{"description":"ethical hacking notes","public":false,"files":{"notes.txt":{"content":"ethical hacking basics plain text 101"}}}'
```

read gist
```
curl -H "Authorization: Bearer $GH_TOKEN" https://api.github.com/gists/GIST_ID
```

add content to gist
```
curl -X PATCH https://api.github.com/gists/GIST_ID 
-H "Authorization: Bearer $GH_TOKEN" 
-H "Content-Type: application/json" 
-d '{"files":{"notes.txt":{"content":"OLD_CONTENT\nNEW_LINES"}}}'
```

bye bye gist
```
curl -X DELETE -H "Authorization: Bearer $GH_TOKEN" https://api.github.com/gists/GIST_ID
```


## OTHER USEFUL TOOLS

nmap 127.0.0.1 nmap -sV 127.0.0.1 nmap -A 127.0.0.1 tcpdump -i eth0 nc -lvnp 4444 nc 127.0.0.1 4444 whois example.com nslookup example.com

## OWASP TOP 10
1. broken access control  
2. cryptographic failures  
3. injection  
4. insecure design  
5. security misconfiguration  
6. vulnerable components  
7. auth failures  
8. data integrity failures  
9. logging failures  
10. ssrf  

## LOGGING & MONITORING

/var/log/auth.log /var/log/syslog /var/log/nginx/access.log /var/log/nginx/error.log top htop journalctl

## DEFENSIVE BEST PRACTICES
update systems  
use firewall  
least privilege  
strong passwords  
2fa  
rate limiting  
input validation  
backup regularly  

## VIRTUALIZATION & LABS
vmware  
virtualbox  
docker  
kali linux  
ubuntu server  

## LEGAL & ETHICS
permission required  
written scope  
no data destruction  
report findings  
respect privacy  

## NOTES
test only authorized systems  
log everything  
keep traffic capture clean  
document steps  
stay ethical
