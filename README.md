زن  زندگی آزادی
# مقدمه
از اونجایی که  سرعت آپلود داره روز به روز بدتر میشه 
وظیفه خودمون دونستیم که آموزش افزایش سرعت سرور رو با استفاده ازBBR
 داخل گیتهاب بزاریم و ویدیوی آموزشیش رو هم داخل یوتیوب بزاریم.
 

#روش اول

```sh
bash <(curl -fsSL https://raw.githubusercontent.com/69learn/fastbbr/main/bbr.sh)
```
#روش دوم

```sh
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh
```

#روش سوم

```sh
echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf
sysctl -p
lsmod | grep bbr
```

#روش آخر
```sh
bash <(curl -fsSL https://raw.githubusercontent.com/69learn/fastbbr/main/hybla.sh)
```




اینترنت یا برای همه یا برای هیچکس!

به امید آزادی

