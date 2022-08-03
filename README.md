# চলুন বাংলায় জেনে আসি nmap টুলের কমান্ড গুলোর কাজ


![nmap](images/nmap.png)

nmap টুল ইনস্টল কমান্ড:

    sudo apt install nmap -y
<br/>

যদি পুর্বেই ইনস্টল করা থাকে তাহলে এমন দেখাবে:
```
sudo apt install nmap -y
[sudo] password for hunter: 
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
nmap is already the newest version (7.91+dfsg1+really7.80+dfsg1-2).
0 upgraded, 0 newly installed, 0 to remove and 24 not upgraded.

```
<br/>

ভার্শন চেক করার কমান্ড:

    nmap --version

<br/>

nmap এর help মেনু দেখার কমান্ড: এছাড়াও রয়েছে `nmap`, `nmap --help`, `man nmap`.

    nmap -h

<br/>

টার্গেট আইপি চেক: এখানে আইপি এর জায়গায় টার্গেট হোস্ট `scanme.nmap.org` দিতে পারবেন

    nmap 45.33.32.156