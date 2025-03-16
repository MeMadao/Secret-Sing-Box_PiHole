# Secret-Sing-Box + Pi-hole

!!! In develop

Currentle, doesn't work with PiHole v6

### Adds Pi-hole for flexible configuration of ad blocking and other unwanted domains when using [Sing-box](https://github.com/SagerNet/sing-box)

Based on [https://github.com/MeMadao/Secret-Sing-Box_PiHole](https://github.com/BLUEBL0B/Secret-Sing-Box)

Differences:
* .by domains are excluded from proxying
* Added [Pi-hole](https://github.com/pi-hole/pi-hole) (works via Nginx)
* Pi-hole acts as a DNS server for [Sing-box](https://github.com/SagerNet/sing-box):  `"dns": { "servers": [ { "tag": "dns-remote", "address": "127.0.0.1" } ] }`

> Currently, Pi-hole does not differentiate between different Sing-box clients and perceives them as one.

## Installation

```
bash <(curl -Ls https://raw.githubusercontent.com/MeMadao/Secret-Sing-Box_PiHole/refs/heads/main/Scripts/install-server.sh)
```

For proper functioning, during the installation of Pi-hole, it is necessary to enable the UI:

![image](https://github.com/user-attachments/assets/0b1cbbcc-0b0f-4c56-919e-8d285f4d7691)

As well as PHP for the UI to work correctly:

![image](https://github.com/user-attachments/assets/1aaada14-5532-472c-88eb-c601f77e1f16)
