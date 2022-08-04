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

### টার্গেট আইপির ক্ষেত্রে:

Single টার্গেট আইপি চেক: এখানে আইপি এর জায়গায় টার্গেট হোস্ট `scanme.nmap.org` দিতে পারবেন

    nmap 45.33.32.156

<br/>

একাধিক টার্গেট আইপি চেক: একাধিক আইপির ক্ষেত্রে প্রতিটা আইপি এর পরে একটি করে `space` দিতে হবে

    nmap 45.33.32.156 48.33.32.126 50.33.31.156

<br/>

নির্দিষ্ট রেঞ্জ `range` এর আইপি চেক: এখানে `১৫৬` থেকে `১৬০` পর্যন্ত মোট `৫` টি আইপি চেক করবে.

    nmap 45.33.32.156-160

<br/>

অনেক গুলো আইপি যদি  ফাইল আকারে save করা থাকে তাহলে ফাইলের ভোতরের আইপি গুলো চেক করার কমান্ড: সেক্ষে আইপি যুক্ত ফাইল এর লোকেশন টি সঠিক ভাবে দিতে হবে.

    nmap -iL /home/hunter/Desktop/multiple-ip.txt

<br/>

আইপি গুলো `file_name.txt` ফাইলের ভেতরে প্রতিটি লাইনে একেক টি করে থাকতে হবে.

```
45.33.32.157
45.33.32.158
45.33.32.159
45.33.32.160
```