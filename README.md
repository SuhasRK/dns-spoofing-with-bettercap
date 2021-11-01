
# DNS spoofing with Bettercap

DNS works like a Phone book of Internet. All servers in the internet will be hosted with its IP address. As we humans cannot remmember IP address of all servers we connect , we remember its Domain names. Thats where DNS comes in. DNS stands for Domain Name System. It maps all the domain names which we surf in the internet to its corresponding IP address. Can we imagine a world without DNS ??\
__So what is DNS spoofing then??__\
If victim surfs google.com in his web-browser and we as a attacker grabs all the packets sent from victim's PC and redirect him to spoofed webpage which look alike google. Since we are using bettercap for this purpose we can also grab all the credentials entere by victim on our spoofed webpage.

## Installation

Install bettercap with apt.I recommend to use version bettercap v2.23.
[click here to download bettercap v2.23](https://ufile.io/joxjzflg)

```bash
  bettercap
```





## Execution Steps

Download the files required to display a spoofed website from this [Link](https://drive.google.com/file/d/1L3aqTSRq6UJWBMoJK7VvyJezn0F0332T/view?usp=sharing) and replace it with files in /var/www/html\
And caplet file from this [Link](https://www.mediafire.com/file/fxg6x889a6k2nvr/dns_spoof.cap/file) , open it and add victim's IP address and domain name you want to spoof. And store it in root directory.


```bash
  bettercap -iface <name-of-wifi-adapter> -caplet /root/dns_spoof.cap
```

Open another terminal

```bash
  service apache2 restart
```

Now browser the website in victim's PC and wait for results.
## Demo

If you are stuck at any step, do watch my video for assistance.\
[Click on this Link](https://drive.google.com/file/d/1L3aqTSRq6UJWBMoJK7VvyJezn0F0332T/view?usp=sharing)



## 🚀 About Me
__Myself Suhas RK__ \
__I am currently persuing CSE at PES university Bangalore.__ \
__My fields of interest are Ethical Hacking and Cyber Security__


## 🔗 Links
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/suhas-rk-a23734207/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://mobile.twitter.com/SuhasRK2)


