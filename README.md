# Jarkom-Modul-4-C06-2022

## Anggota Kelompok
1. 5025201050 - Elshe Erviana Angely
2. 5025201051 - Muhammad Fath Mushaffa Azhar
3. 5025201076 - Raul Ilma Rajasa

## VLSM - Cisco Packet Tracer
Untuk membuat VLSM, pertama-tama, kita perlu membuat tabel yang berisi jumlah IP pada setiap subnet beserta totalnya
### Tabel Subnet
| Subnet | Jumlah IP | Netmask |
| --- | --- | --- |
| A1 | 2 | /30 |
| A2 | 251 | /24 |
| A3 | 121 | /25 |
| A4 | 71 | /25 |
| A5 | 2 | /30 |
| A6 | 1001 | /22 |
| A7 | 212 | /24 |
| A8 | 501 | /23 |
| A9 | 2 | /30 |
| A10 | 51 | /26 |
| A11 | 271 | /23 |
| A12 | 2 | /30 |
| A13 | 2 | /30 |
| A14 | 121 | /25 |
| A15 | 2 | /30 |
| A16 | 2 | /30 |
| A17 | 2 | /30 |
| A18 | 2 | /30 |
| Total | 2618 | /20 |

### VLSM Tree
Sehingga proyeksi tree dari VLSM-nya adalah sebagai berikut:
![VLSM-Tree (1).jpg](assets/VLSM-Tree_(1).jpg)

### Pembagian IP
| Subnet | Network ID | Netmask | Broadcast |
| --- | --- | --- | --- |
| A1 | 192.182.0.0 | 255.255.255.252 | 192.182.0.3 |
| A2 | 192.182.1.0 | 255.255.255.0 | 192.182.1.255 |
| A3 | 192.182.0.128 | 255.255.255.128 | 192.182.0.255 |
| A4 | 192.182.4.128 | 255.255.255.128 | 192.182.4.255 |
| A5 | 192.182.0.4 | 255.255.255.252 | 192.182.0.7 |
| A6 | 192.182.8.0 | 255.255.252.0 | 192.182.11.255 |
| A7 | 192.182.5.0 | 255.255.255.0 | 192.182.5.255 |
| A8 | 192.182.2.0 | 255.255.254.0 | 192.182.3.255 |
| A9 | 192.182.0.16 | 255.255.255.252 | 192.182.0.19 |
| A10 | 192.182.0.64 | 255.255.255.192 | 192.182.0.127 |
| A11 | 192.182.6.0 | 255.255.254.0 | 192.182.7.255 |
| A12 | 192.182.0.8 | 255.255.255.252 | 192.182.0.11 |
| A13 | 192.182.0.12 | 255.255.255.252 | 192.182.0.15 |
| A14 | 192.182.4.0 | 255.255.255.128 | 192.182.4.127 |
| A15 | 192.182.0.20 | 255.255.255.252 | 192.182.0.23 |
| A16 | 192.182.0.24 | 255.255.255.252 | 192.182.0.27 |
| A17 | 192.182.0.28 | 255.255.255.252 | 192.182.0.31 |
| A18 | 192.182.0.32 | 255.255.255.252 | 192.182.0.35 |

## Topologi - Cisco Packet Tracer
Dalam CPT, topologi dibuat seperti pada modul Jarkom 4, setelah itu setiap node (router, host) dikonfigurasi sesuai dengan subnet IP, sehingga node dan gateway IP berada dalam rentang IP yang dapat digunakan dari setiap subnet. Kemudian melakukan routing langsung dan routing statis untuk setiap router di topologi. Pengujian file .pkt dapat dilakukan dengan mengirimkan pesan dari satu node ke node lainnya
![Topologi-Cisco Packet Tracer.jpg](assets/TopologiCPT.jpg)

## CIDR - GNS 3

### Perhitungan Subnet

******************Langkah 1******************

![Langkah 1.png](assets/Langkah_1.png)

Penggabungan

Dari langkah 1 di atas, didapatkan penggabungan sebagai berikut: 

![messageImage_1669396522966.jpg](assets/messageImage_1669396522966.jpg)

******************Langkah 2******************

![Langkah 2.png](assets/Langkah_2.png)

Dari langkah 2 di atas, didapatkan penggabungan sebagai berikut:

![messageImage_1669393625734.jpg](assets/messageImage_1669393625734.jpg)

******************Langkah 3******************

![Langkah 3.png](assets/Langkah_3.png)

Dari langkah 3 di atas, didapatkan penggabungan sebagai berikut:

![messageImage_1669393632275.jpg](assets/messageImage_1669393632275.jpg)

**************Langkah 4**************

![Langkah 4.png](assets/Langkah_4.png)

Dari langkah 4 di atas, didapatkan penggabungan sebagai berikut:

![messageImage_1669393639889.jpg](assets/messageImage_1669393639889.jpg)

******************Langkah 5******************

![Langkah 5.png](assets/Langkah_5.png)

Dari langkah 5 di atas, didapatkan penggabungan sebagai berikut:

![messageImage_1669393646576.jpg](assets/messageImage_1669393646576.jpg)

******************Langkah 6******************

![Langkah 6.png](assets/Langkah_6.png)

Dari langkah 6 di atas, didapatkan penggabungan sebagai berikut:

![messageImage_1669393652783.jpg](assets/messageImage_1669393652783.jpg)

******************Langkah 7******************

![Langkah 7.png](assets/Langkah_7.png)

Dari langkah 7 di atas, didapatkan penggabungan sebagai berikut:

![messageImage_1669393660785.jpg](assets/messageImage_1669393660785.jpg)

### Tree

![CIDR-Tree.jpg](assets/CIDR-Tree.jpg)

### Pembagian IP

| Subnet | Network ID | Netmask | Broadcast |
| --- | --- | --- | --- |
| A1 | 192.182.1.0 | 255.255.255.252 | 192.182.1.3 |
| A2 | 192.182.64.0 | 255.255.255.0 | 192.182.64.255 |
| A3 | 192.182.8.0 | 255.255.255.128 | 192.182.8.127 |
| A4 | 192.182.8.128 | 255.255.255.128 | 192.182.8.255 |
| A5 | 192.182.65.0 | 255.255.255.252 | 192.182.65.3 |
| A6 | 192.182.64.0 | 255.255.252.0 | 192.182.67.255 |
| A7 | 192.182.0.0 | 255.255.255.0 | 192.182.0.255 |
| A8 | 192.182.2.0 | 255.255.254.0 | 192.182.3.255 |
| A9 | 192.182.72.0 | 255.255.255.252 | 192.182.72.3 |
| A10 | 192.182.80.0 | 255.255.255.192 | 192.182.80.63 |
| A11 | 192.182.32.0 | 255.255.254.0 | 192.182.33.255 |
| A12 | 192.182.9.0 | 255.255.255.252 | 192.182.9.3 |
| A13 | 192.182.4.0 | 255.255.255.252 | 192.182.4.3 |
| A14 | 192.182.12.0 | 255.255.255.128 | 192.182.12.127 |
| A15 | 192.182.16.0 | 255.255.255.252 | 192.182.16.3 |
| A16 | 192.182.96.0 | 255.255.255.252 | 192.182.96.3 |
| A17 | 192.182.34.0 | 255.255.255.252 | 192.182.34.3 |
| A18 | 192.182.36.0 | 255.255.255.252 | 192.182.36.3 |

### Konfigurasi GNS
#### The Resonance
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
        address 192.182.64.1
        netmask 255.255.255.252

auto eth2
iface eth2 inet static
         address 192.182.192.1
         netmask 255.255.255.252

auto eth3
iface eth3 inet static
        address 192.182.1.1
        netmask 255.255.255.252

auto eth4
iface eth4 inet static
        address 192.182.32.1
        netmask 255.255.255.252
```
#### The Magical
```
auto eth0
iface eth0 inet static
	address 192.182.100.2
	netmask 255.255.255.252
	gateway 192.182.100.1

auto eth1
iface eth1 inet static
	address 192.182.96.1
	netmask 255.255.254.0
```
#### The Magical
```
iface eth0 inet static
	address 192.182.32.2
	netmask 255.255.255.252
	gateway 192.182.32.1

auto eth1
iface eth1 inet static
	address 192.182.16.1
	netmask 255.255.255.192

auto eth2
auto eth0
iface eth0 inet static
	address 192.182.32.2
	netmask 255.255.255.252
	gateway 192.182.32.1

auto eth1
iface eth1 inet static
	address 192.182.16.1
	netmask 255.255.255.192

auto eth2
iface eth2 inet static
	address 192.182.8.1
	netmask 255.255.255.252
```
#### The Minister
```
auto eth0
iface eth0 inet static
	address 192.182.8.2
	netmask 255.255.255.252
	gateway 192.182.8.1

auto eth1
iface eth1 inet static
	address 192.182.4.1
	netmask 255.255.252.0

auto eth2
iface eth2 inet static
	address 192.182.1.1
	netmask 255.255.255.252
```
#### The Dauntless
```
auto eth0
iface eth0 inet static
	address 192.182.1.2
	netmask 255.255.255.252
	gateway 192.182.1.1

auto eth1
iface eth1 inet static
	address 192.182.0.1
	netmask 255.255.255.0
```
#### The Queen
```
auto eth0
iface eth0 inet static
	address 192.182.64.2
	netmask 255.255.255.0
	gateway 192.182.64.1

auto eth1
iface eth1 inet static
	address 192.182.65.1
	netmask 255.255.255.252
```
#### The Instrument
```
auto eth0
iface eth0 inet static
	address 192.182.80.2
	netmask 255.255.255.252
	gateway 192.182.80.1

auto eth1
iface eth1 inet static
	address 192.182.74.1
	netmask 255.255.255.128

auto eth2
iface eth2 inet static
	address 192.182.68.1
	netmask 255.255.255.252

auto eth3
iface eth3 inet static
	address 192.182.73.1
	netmask 255.255.255.252
```
#### The Profound
```
auto eth0
iface eth0 inet static
	address 192.182.73.2
	netmask 255.255.255.252
	gateway 192.182.73.1

auto eth1
iface eth1 inet static
	address 192.182.72.129
	netmask 255.255.255.128

auto eth2
iface eth2 inet static
	address 192.182.72.1
	netmask 255.255.255.128
```
#### Ashaf
```
auto eth0
iface eth0 inet static
	address 192.182.16.2
	netmask 255.255.255.192
	gateway 192.182.16.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
  ```
#### The Beast
```
auto eth0
iface eth0 inet static
	address 192.182.98.2
	netmask 255.255.255.252
	gateway 192.182.98.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Haines
```
auto eth0
iface eth0 inet static
	address 192.182.96.3
	netmask 255.255.254.0
	gateway 192.182.96.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Corvekt
```
auto eth0
iface eth0 inet static
	address 192.182.96.2
	netmask 255.255.254.0
	gateway 192.182.96.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Spendrow
```
auto eth0
iface eth0 inet static
	address 192.182.72.2
	netmask 255.255.255.128
	gateway 192.182.72.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Helga
```
auto eth0
iface eth0 inet static
	address 192.182.72.130
	netmask 255.255.255.128
	gateway 192.182.72.129
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Oakleave
```
auto eth0
iface eth0 inet static
	address 192.182.66.2
	netmask 255.255.254.0
	gateway 192.182.66.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### The Witch
```
auto eth0
iface eth0 inet static
	address 192.182.65.2
	netmask 255.255.255.252
	gateway 192.182.65.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Keith
```
auto eth0
iface eth0 inet static
	address 192.182.64.3
	netmask 255.255.255.0
	gateway 192.182.64.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Johan
```
auto eth0
iface eth0 inet static
	address 192.182.0.2
	netmask 255.255.255.0
	gateway 192.182.0.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Phanora
```
auto eth0
iface eth0 inet static
	address 192.182.0.3
	netmask 255.255.255.0
	gateway 192.182.0.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Guideau
```
auto eth0
iface eth0 inet static
	address 192.182.4.2
	netmask 255.255.252.0
	gateway 192.182.4.1
	up echo nameserver 192.168.122.1 > /etc/resolv.conf
```
#### Setup Static dan Direct Routing
Di setiap router statis dan perutean langsung dilakukan seperti di GNS, skrip router dapat dijalankan dengan `bash /root/script.sh`.

## Kendala
Tidak ada
## Revisi
Tidak ada