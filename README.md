[English version](https://github.com/MeMadao/Secret-Sing-Box_PiHole/blob/main/Docs/README-EN.md)

!!! In develop
На данный момент, не работает с PiHole v6

# Secret-Sing-Box + Pi-hole

### Добавляет Pi-hole для гибкой настройки блокирования рекламы и других нежелательных доменов при использовании [Sing-box](https://github.com/SagerNet/sing-box)

Основано на [https://github.com/MeMadao/Secret-Sing-Box_PiHole](https://github.com/BLUEBL0B/Secret-Sing-Box)

Отличия:
* .by домены исключены для проксирования
* Добавлен [Pi-hole](https://github.com/pi-hole/pi-hole) (работает через Nginx)
* Pi-hole выступает в качестве DNS-сервра для [Sing-box](https://github.com/SagerNet/sing-box):  `"dns": { "servers": [ { "tag": "dns-remote", "address": "127.0.0.1" } ] }`

> На данный момент Pi-hole не различает разных клиентов Sing-box и воспринимает их как одного.

## Установка

```
bash <(curl -Ls https://raw.githubusercontent.com/MeMadao/Secret-Sing-Box_PiHole/refs/heads/main/Scripts/install-server.sh)
```

Для корректной работы, во время установки Pi-hole, необходимо установить UI:

![image](https://github.com/user-attachments/assets/0b1cbbcc-0b0f-4c56-919e-8d285f4d7691)

А так же PHP для корректной работы UI:

![image](https://github.com/user-attachments/assets/1aaada14-5532-472c-88eb-c601f77e1f16)
