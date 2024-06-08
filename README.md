# Jarkom-Modul-4-IT20-2024

**Kelompok IT20**
| Nama | NRP |
|-----------------------|--------------|
| Clara Valentina | 5027221016 |
| Muhammad Arsy Athallah| 5027221048 |

## GNS3 VLSM
### Topologi dan subnetting

<img width="952" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/539efe00-62dd-4209-b948-a7b26f04bee0">

### Tree VLSM

<img width="1096" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/d1259b11-b42c-4b37-95de-1c94e7d37a99">
Tree lebih detail : (https://drive.google.com/file/d/1lXM2dagMoluTJhxWGsED0R034WWuOEiG/view?usp=sharing)

### Konfigurasi Router
#### JAWA (A1 - A8 - A16) 
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
    address 192.243.21.177
    netmask 255.255.255.252

auto eth2
iface eth2 inet static
    address 192.243.21.189
    netmask 255.255.255.252

auto eth3
iface eth3 inet static
    address 192.243.21.205
    netmask 255.255.255.252
```
#### SUMATERA ( A1 - A2 - A4 )
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.178
    netmask 255.255.255.252
    gateway 192.243.21.177

auto eth1
iface eth1 inet static
    address 192.243.21.181
    netmask 255.255.255.252

auto eth2
iface eth2 inet static
    address 192.243.21.65
    netmask 255.255.255.224
```
#### LAMPUNG ( A2 - A3 )
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.182
    netmask 255.255.255.252
    gateway 192.243.21.181

auto eth1
iface eth1 inet static
    address 192.243.19.1
    netmask 255.255.255.0

```
#### Sebuku (A3)
```
auto eth0
iface eth0 inet static
    address 192.243.19.2
    netmask 255.255.255.0
    gateway 192.243.19.1
```
#### Sebesi (A3)
```
auto eth0
iface eth0 inet static
    address 192.243.19.3
    netmask 255.255.255.0
    gateway 192.243.19.1
```
#### Sibandang (A4)
```
auto eth0
iface eth0 inet static
    address 192.243.21.66
    netmask 255.255.255.224
    gateway 192.243.21.65
```
#### Samosir (A4)
```
auto eth0
iface eth0 inet static
    address 192.243.21.67
    netmask 255.255.255.224
    gateway 192.243.21.65
```
#### SUMATERA-UTARA (A4 - A5)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.68
    netmask 255.255.255.224
    gateway 192.243.21.65

auto eth1
iface eth1 inet static
    address 192.243.21.185
    netmask 255.255.255.252
```
#### ACEH ( A5 - A6 - A7 )
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.186
    netmask 255.255.255.252
    gateway 192.243.21.185

auto eth1
iface eth1 inet static
    address 192.243.20.1
    netmask 255.255.255.128

auto eth2
iface eth2 inet static
    address 192.243.21.129
```
#### Berawang-Tampu (A6)
```
auto eth0
iface eth0 inet static
    address 192.243.20.2
    netmask 255.255.255.128
    gateway 192.243.20.1
```
#### Enang-Enang (A6)
```
auto eth0
iface eth0 inet static
    address 192.243.20.3
    netmask 255.255.255.128
    gateway 192.243.20.1
```
#### Starland (A6)
```
auto eth0
iface eth0 inet static
    address 192.243.20.4
    netmask 255.255.255.128
    gateway 192.243.20.1
```
#### Sabang (A7)
```
auto eth0
iface eth0 inet static
    address 192.243.21.130
    netmask 255.255.255.224
    gateway 192.243.21.129
```
#### Lambaro (A7)
```
auto eth0
iface eth0 inet static
    address 192.243.21.131
    netmask 255.255.255.224
    gateway 192.243.21.129
```
#### KALIMANTAN ( A8 - A9 )
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.190
    netmask 255.255.255.252
    gateway 192.243.21.189

auto eth1
iface eth1 inet static
    address 192.243.21.193
    netmask 255.255.255.252
```
#### KALIMANTAN-UTARA ( A9- A10 - A11)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.194
    netmask 255.255.255.252
    gateway 192.243.21.193

auto eth1
iface eth1 inet static
    address 192.243.18.1
    netmask 255.255.255.0

auto eth2
iface eth2 inet static
    address 192.243.21.197
    netmask 255.255.255.252
```
#### Selimau (A10)
```
auto eth0
iface eth0 inet static
    address 192.243.18.2
    netmask 255.255.255.0
    gateway 192.243.18.1
```
#### KALIMANTAN-TIMUR (A11-A12-A13)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.198
    netmask 255.255.255.252
    gateway 192.243.21.197

auto eth1
iface eth1 inet static
    address 192.243.16.1
    netmask 255.255.254.0

auto eth2
iface eth2 inet static
    address 192.243.21.201
    netmask 255.255.255.252
```
#### Bangkirai (A12)
```
auto eth0
iface eth0 inet static
    address 192.243.16.2
    netmask 255.255.254.0
    gateway 192.243.16.1
```
#### Lamaru (A12)
```
auto eth0
iface eth0 inet static
    address 192.243.16.3
    netmask 255.255.254.0
    gateway 192.243.16.1
```
#### KALIMANTAN-SELATAN (A13-A14-A15)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.202
    netmask 255.255.255.252
    gateway 192.243.21.201

auto eth1
iface eth1 inet static
    address 192.243.21.97
    netmask 255.255.255.224

auto eth2
iface eth2 inet static
    address 192.243.0.1
    netmask 255.255.248.0
```
#### Angsana (A14)
```
auto eth0
iface eth0 inet static
    address 192.243.21.98
    netmask 255.255.255.224
    gateway 192.243.21.97
```
#### Bajuin (A15)
```
auto eth0
iface eth0 inet static
    address 192.243.0.2
    netmask 255.255.248.0
    gateway 192.243.0.1
```
#### Takisung (A15)
```
auto eth0
iface eth0 inet static
    address 192.243.0.3
    netmask 255.255.248.0
    gateway 192.243.0.1
```
#### Batakan (A15)
```
auto eth0
iface eth0 inet static
    address 192.243.0.4
    netmask 255.255.248.0
    gateway 192.243.0.1
```
#### SULAWESI (A16-A17-A20)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.206
    netmask 255.255.255.252
    gateway 192.243.21.205

auto eth1
iface eth1 inet static
    address 192.243.21.161
    netmask 255.255.255.248

auto eth2
iface eth2 inet static
    address 192.243.20.129
    netmask 255.255.255.128
```
#### MAKASAR (A17-A18)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.162
    netmask 255.255.255.248
    gateway 192.243.21.161

auto eth1
iface eth1 inet static
    address 192.243.21.169
    netmask 255.255.255.248
```
#### Topejawa-Takalar (A18)
```
auto eth0
iface eth0 inet static
    address 192.243.21.170
    netmask 255.255.255.248
    gateway 192.243.21.169
```
#### Galesong (A18)
```
auto eth0
iface eth0 inet static
    address 192.243.21.170
    netmask 255.255.255.248
    gateway 192.243.21.169
```
#### BELAWA (A17-A19)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.21.163
    netmask 255.255.255.248
    gateway 192.243.21.161

auto eth1
iface eth1 inet static
    address 192.243.21.1
    netmask 255.255.255.192
```
#### Baru (A19)
```
auto eth0
iface eth0 inet static
    address 192.243.21.2
    netmask 255.255.255.192
    gateway 192.243.21.1
```
#### Madini (A19)
```
auto eth0
iface eth0 inet static
    address 192.243.21.3
    netmask 255.255.255.192
    gateway 192.243.21.1
```
#### Marisa (A20)
```
auto eth0
iface eth0 inet static
    address 192.243.20.132
    netmask 255.255.255.128
    gateway 192.243.20.129
```
#### Gorontalo (A20)
```
#A20 > SULAWESI
auto eth0
iface eth0 inet static
    address 192.243.20.131
    netmask 255.255.255.128
    gateway 192.243.20.129
```
#### MALUKU-UTARA (A20-A21)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
    address 192.243.20.130
    netmask 255.255.255.128
    gateway 192.243.20.129

auto eth1
iface eth1 inet static
    address 192.243.8.1
    netmask 255.255.248.0
``` 
#### Ternate (A21)
```
auto eth0
iface eth0 inet static
    address 192.243.8.2
    netmask 255.255.248.0
    gateway 192.243.8.1
```
#### Morotai (A21)
```
auto eth0
iface eth0 inet static
    address 192.243.8.3
    netmask 255.255.248.0
    gateway 192.243.8.1
```
#### Tobeto (A21)
```
auto eth0
iface eth0 inet static
    address 192.243.8.4
    netmask 255.255.248.0
    gateway 192.243.8.1
```

### Script Node
####
```
#SUMATERA
route add -net 192.243.21.180 netmask 255.255.255.252 gw 192.243.21.178
route add -net 192.243.19.0 netmask 255.255.255.0 gw 192.243.21.178
route add -net 192.243.21.64 netmask 255.255.255.224 gw 192.243.21.178
route add -net 192.243.21.184 netmask 255.255.255.252 gw 192.243.21.178
route add -net 192.243.20.0 netmask 255.255.255.128 gw 192.243.21.178
route add -net 192.243.21.128 netmask 255.255.255.224 gw 192.243.21.178

#KALIMANTAN
route add -net 192.243.21.192 netmask 255.255.255.252 gw 192.243.21.190
route add -net 192.243.18.0 netmask 255.255.255.0 gw 192.243.21.190
route add -net 192.243.21.196 netmask 255.255.255.252 gw 192.243.21.190
route add -net 192.243.16.0 netmask 255.255.254.0 gw 192.243.21.190
route add -net 192.243.21.200 netmask 255.255.255.252 gw 192.243.21.190
route add -net 192.243.21.96 netmask 255.255.255.224 gw 192.243.21.190
route add -net 192.243.0.0 netmask 255.255.248.0 gw 192.243.21.190

#SULAWESI
route add -net 192.243.21.160 netmask 255.255.255.248 gw 192.243.21.206
route add -net 192.243.21.168 netmask 255.255.255.248 gw 192.243.21.206
route add -net 192.243.21.0 netmask 255.255.255.192 gw 192.243.21.206
route add -net 192.243.20.128 netmask 255.255.255.128 gw 192.243.21.206
route add -net 192.243.8.0 netmask 255.255.248.0 gw 192.243.21.206
```
#### SUMATERA
```
#JAWA
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.243.21.177

#SUMATERA-UTARA
route add -net 192.243.21.184 netmask 255.255.255.252 gw 192.243.21.68
route add -net 192.243.20.0 netmask 255.255.255.128 gw 192.243.21.68
route add -net 192.243.21.128 netmask 255.255.255.224 gw 192.243.21.68

#LAMPUNG
route add -net 192.243.19.0 netmask 255.255.255.0 gw 192.243.21.182
```
#### KALIMANTAN
```
route add -net 192.243.18.0 netmask 255.255.255.0 gw 192.243.21.194
route add -net 192.243.21.196 netmask 255.255.255.252 gw 192.243.21.194
route add -net 192.243.16.0 netmask 255.255.254.0 gw 192.243.21.194
route add -net 192.243.21.200 netmask 255.255.255.252 gw 192.243.21.194
route add -net 192.243.21.96 netmask 255.255.255.224 gw 192.243.21.194
route add -net 192.243.0.0 netmask 255.255.248.0 gw 192.243.21.194
```
#### SULAWESI
```
#MALUKU-UTARA
route add -net 192.243.8.0 netmask 255.255.248.0 gw 192.243.20.130

#MAKASAR
route add -net 192.243.21.168 netmask 255.255.255.248 gw 192.243.21.162

#BELAWA
route add -net 192.243.21.0 netmask 255.255.255.192 gw 192.243.21.163
```
#### SUMATERA-UTARA
```
#SW-BLANGKARAI
route add -net 192.243.20.0 netmask 255.255.255.128 gw 192.243.21.186
#SW-BANDA-ACEH
route add -net 192.243.21.128 netmask 255.255.255.224 gw 192.243.21.186 
```
#### LAMPUNG
```
#SUMATERA
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.243.21.181
```
#### KALIMANTAN-UTARA
```
route add -net 192.243.16.0 netmask 255.255.254.0 gw 192.243.21.198
route add -net 192.243.21.200 netmask 255.255.255.252 gw 192.243.21.198
route add -net 192.243.21.96 netmask 255.255.255.224 gw 192.243.21.198
route add -net 192.243.0.0 netmask 255.255.248.0 gw 192.243.21.198
```
#### MAKASAR
```
#SULAWESI
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.243.21.161
```
#### BELAWA 
```
#SULAWESI
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.243.21.161
```
#### MALUKU-UTARA
```
#SULAWESI
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.243.20.129
```
#### ACEH
```
#SUMATERA UTARA
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.243.21.185 
```
#### KALIMANTAN-TIMUR
```
route add -net 192.243.21.96 netmask 255.255.255.224 gw 192.243.21.202
route add -net 192.243.0.0 netmask 255.255.248.0 gw 192.243.21.202
```
#### KALIMANTAN-SELATAN
```
#KALIMANTAN-TIMUR
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.243.21.201
```
### Dokumentasi GNS3 VLSM
Kalimantan Selatan ke Aceh

<img width="502" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/dd393ffc-7041-4a80-bf8a-cf2ae6e53844">

Aceh ke Kalimantan Selatan

<img width="411" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/a502a3e1-2048-4ae2-8ea7-d5e60f838da1">

Sebuku ke Sulawesi 

<img width="479" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/940c7ff6-f480-4282-9879-687c5dcdc4b5">

Sulawesi ke Sebuku

<img width="431" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/4deef04d-884e-45f9-bf94-bc3f1fb06992">

Belawa ke Sabang

<img width="421" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/b47be179-1c22-419e-a24f-1a67ad029324">

Sabang  ke Belawa 

<img width="470" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/fa64c8fc-3ced-45e2-a69b-ec125ab54abb">

Lamaru ke Samosir

<img width="485" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/8b7df8f8-bcff-437c-86f8-012adfe527a2">

Samosir ke Lamaru

<img width="484" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/ecd61e79-2757-4e4f-b7c2-9ef860597d7a">

Ternate ke Starland

<img width="491" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/8842edd7-af98-412a-85d8-d20a5283a7d7">

Starland ke Ternate

<img width="497" alt="image" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/123356941/c86562fb-e09b-4a1e-b6d9-b91c457a6a56">




## CPT CIDR

### Penggabungan Ip

**Kondisi Node Awal**
<img width="1316" alt="topo4" src="https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/128389289/24c74394-a138-4166-9924-cb2a8c78c249">

![image](https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/128389289/d57ee4db-5117-4c53-a6f9-963b8ff91c78)

### Penggabungan Node
![TOPO4 GROUPING_page-0001](https://github.com/clar04/Jarkom-Modul-4-IT20-2024/assets/128389289/acef2932-33f6-487b-a38a-65f00aa5671c)

A: Hitam
B: Merah
C: Hijau
D: Biru
E: Oren
F: Ungu
G: Cyan
H: Kuning
I: Pink










