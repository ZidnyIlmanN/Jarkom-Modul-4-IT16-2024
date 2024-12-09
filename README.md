# Jarkom-Modul-4-IT16-2024

| Nama          | NRP          |
| ------------- | ------------ |
| Zidny Ilman Nafi'an | 5027221072 |
| MUHAMMAD DZAKWAN | 5027201065 |

## Pembagian Rute Subnet

| Nama Subnet           | Rute                                                         | Jumlah IP | Netmask |
|-----------------------|--------------------------------------------------------------|-----------|---------|
| A1                    | Hololive - Holo-EN                                           | 2         | /30     |
| A2                    | Holo-EN - Holo-Myth                                          | 2         | /30     |
| A3                    | Holo-Myth - Switch2 - Kiara_Calli--(193_HOST) - Gura_Ame_Ina--(309_HOST) | 503       | /23     |
| A4                    | Holo Myth - HoloPromise - Project-Hope - HoloCouncil         | 3         | /29     |
| A5                    | Project-Hope - Irys--(2_HOST)                                | 3         | /29     |
| A6                    | Holo-Council - Switch4 - Kronii_Mumei--(39_HOST) - Bae-Fauna--(22_HOST) | 62 | /26 |
| A7                    | Holo-EN - HoloAdvent                                         | 2         | /30     |
| A8                    | HoloAdvent - Switch5 - FuwaMoco--(5_HOST) - Shiori_Nerissa--(12_HOST) - Biboo--(10_HOST) | 28 | /27 |
| A9                    | Hololive - Holo-JP                                           | 2         | /30     |
| A10                   | Holo-JP - Switch1 - GEN:0 - DEV_IS                           | 3         | /29     |
| A11                   | DEV_IS - Re:GLOSS = Ririka_Raden--(3_HOST) - Ao--(3_HOST) - Hajime_Kanade--(7_HOST) | 14 | /28 |
| A12                   | GEN:0 - Switch3 - MiComet--(1501_HOST) - Sora_Robo_AZKi--(542_HOST) - GEN:1 | 2045 | /21 |
| A13                   | GEN:1 - GAMERS                                               | 2         | /30     |
| A14                   | GEN:1 - Member - FBK_Matsuri--(321_HOST) - Aki_Hachama--(148_HOST) | 470 | /23 |
| A15                   | GAMERS - Fubuki - Korone--(51_HOST) - Okayu--(32_HOST) - Mio--(36_HOST) | 120 | /25 |
| A16                   | Hololive - Holo-ID                                           | 2         | /30     |
| A17                   | Holo-ID - AREA15                                             | 2         | /30     |
| A18                   | AREA15 - Switch6 - Risu--(319_HOST) - Moona--(201_HOST) - lofi--(140_HOST) | 661 | /22 |
| A19                   | Holo-ID - holoro                                             | 2         | /30     |
| A20                   | holoro - Switch7 - Ollie--(20_HOST) - Anya--(3_HOST) - Reina--(10_HOST) | 34 | /26 |
| A21                   | Holo-ID - holoh3ro                                           | 2         | /30     |
| A22                   | holoh3ro - Switch8 - Zeta--(81_HOST) - Kaela--(71_HOST) - Kobo--(146_HOST) | 299 | /23 |
| **Total**             |                                                              | **4263**  | **/19** |

## CPT / VLSM
### Topologi
![test](https://github.com/user-attachments/assets/b5292789-9da2-4973-afc7-b1f8b5bdded5)

### Pembagian IP - VLSM
| Subnet | Network ID     | Netmask         | Broadcast      | Range IP                        |
| ------ | -------------- | --------------- | -------------- | ------------------------------- |
| A12    | 192.237.0.0    | 255.255.248.0   | 192.237.7.255  | 192.237.0.1 - 192.237.7.254     |
| A18    | 192.237.8.0    | 255.255.252.0   | 192.237.11.255 | 192.237.8.1 - 192.237.11.254    |
| A3     | 192.237.12.0   | 255.255.254.0   | 192.237.13.255 | 192.237.12.1 - 192.237.13.254   |
| A14    | 192.237.14.0   | 255.255.254.0   | 192.237.15.255 | 192.237.14.1 - 192.237.15.254   |
| A22    | 192.237.16.0   | 255.255.254.0   | 192.237.17.255 | 192.237.16.1 - 192.237.17.254   |
| A15    | 192.237.18.0   | 255.255.255.128 | 192.237.18.127 | 192.237.18.1 - 192.237.18.126   |
| A6     | 192.237.18.128 | 255.255.255.192 | 192.237.18.191 | 192.237.18.129 - 192.237.18.190 |
| A20    | 192.237.18.192 | 255.255.255.192 | 192.237.18.255 | 192.237.18.193 - 192.237.18.254 |
| A8     | 192.237.19.0   | 255.255.255.224 | 192.237.19.31  | 192.237.19.1 - 192.237.19.30    |
| A11    | 192.237.19.32  | 255.255.255.240 | 192.237.19.47  | 192.237.19.33 - 192.237.19.46   |
| A4     | 192.237.19.48  | 255.255.255.248 | 192.237.19.55  | 192.237.19.49 - 192.237.19.54   |
| A5     | 192.237.19.56  | 255.255.255.248 | 192.237.19.63  | 192.237.19.57 - 192.237.19.62   |
| A10    | 192.237.19.64  | 255.255.255.248 | 192.237.19.71  | 192.237.19.65 - 192.237.19.70   |
| A1     | 192.237.19.72  | 255.255.255.252 | 192.237.19.75  | 192.237.19.73 - 192.237.19.74   |
| A2     | 192.237.19.76  | 255.255.255.252 | 192.237.19.79  | 192.237.19.77 - 192.237.19.78   |
| A7     | 192.237.19.80  | 255.255.255.252 | 192.237.19.83  | 192.237.19.81 - 192.237.19.82   |
| A9     | 192.237.19.84  | 255.255.255.252 | 192.237.19.87  | 192.237.19.85 - 192.237.19.86   |
| A13    | 192.237.19.88  | 255.255.255.252 | 192.237.19.91  | 192.237.19.89 - 192.237.19.90   |
| A16    | 192.237.19.92  | 255.255.255.252 | 192.237.19.95  | 192.237.19.93 - 192.237.19.94   |
| A17    | 192.237.19.96  | 255.255.255.252 | 192.237.19.99  | 192.237.19.97 - 192.237.19.98   |
| A19    | 192.237.19.100 | 255.255.255.252 | 192.237.19.103 | 192.237.19.101 - 192.237.19.102 |
| A21    | 192.237.19.104 | 255.255.255.252 | 192.237.19.107 | 192.237.19.105 - 192.237.19.106 |

### Tree VLSM
![image](https://github.com/user-attachments/assets/af529d6e-1518-47bb-bf89-99b9cb608307)

### Testing Revisi - CPT VLSM
https://drive.google.com/file/d/13TTobOthT_bvFklVow5gwLow9cwsoHpW/view?usp=sharing

## GNS3 / CIDR
### TOPOLOGI
![Screenshot 2024-11-13 012515](https://github.com/user-attachments/assets/1994f60a-8f4c-4b6b-8949-5fde5c979a6c)

### Penggabungan
1. Penggabungan 1
![gabung1](https://github.com/user-attachments/assets/17b0b1a3-01ba-45aa-87ab-49585d57c164)

2. Pembagian 2
![gabung2](https://github.com/user-attachments/assets/13851991-1201-49fd-938f-6add06cc09df)
![zgabung1](https://github.com/user-attachments/assets/c05fae0b-d023-4313-a0ae-fb960eea3598)

3. Pembagian 3
![gabung3](https://github.com/user-attachments/assets/c0cda4e1-675f-4f40-a898-1df180a2f2c4)
![zgabung2](https://github.com/user-attachments/assets/2a936ef0-d61c-4c28-ac48-16a40800c215)

4. Pembagian 4
![gabung4](https://github.com/user-attachments/assets/b670a59d-0cab-487e-a502-0f64423f99d9)
![zgabung3](https://github.com/user-attachments/assets/11848333-2bd9-4403-a021-d8a026f7b25d)

5. Pembagian 5
![gabung5](https://github.com/user-attachments/assets/84fd6591-350f-4ab3-a840-2d7ff740921a)
![zgabung4](https://github.com/user-attachments/assets/7f7d20f1-e17b-4aa3-8bb5-783346aa1484)

6. Pembagian 6
![gabung6](https://github.com/user-attachments/assets/674147fa-2a46-4526-a9c9-d6163e770dd6)
![zgabung5](https://github.com/user-attachments/assets/b0b5265f-494b-41fd-944a-7a09af853660)

7. Pembagian 7
![gabung7](https://github.com/user-attachments/assets/954b693b-d721-4d99-8fbe-ce364bf5ed1a)
![zgabung6](https://github.com/user-attachments/assets/5e6460a0-2790-44a2-9bf9-5083d45bc00b)

8. Pembagian 8
![gabung9](https://github.com/user-attachments/assets/6ba73f97-40b7-485b-8422-6d92907eecd7)
![zgabung7](https://github.com/user-attachments/assets/1a27e545-6be2-48a1-baf3-9a22395ef793)

9. Pembagian 9
![gabung8](https://github.com/user-attachments/assets/ae97eaa2-f6f8-40ad-9a00-0fb9f54d84d2)
![zgabung8](https://github.com/user-attachments/assets/5318e8d9-1c30-40ea-8bda-217b6a36c5c9)

10. Pembagian 10
![gabung10](https://github.com/user-attachments/assets/32278479-76cc-41c5-9911-35368295b7ee)
![zgabung9](https://github.com/user-attachments/assets/bae38709-269a-4b7b-8409-30d8236fd0bb)

### Tree CIDR
![cidr ayya](https://github.com/user-attachments/assets/71053e98-048d-4e94-8b4c-b087441cbdbb)

### Pembagian IP - CIDR

| Subnet | Network ID       | Netmask           | Broadcast       | Range IP                          |
|--------|------------------|-------------------|-----------------|-----------------------------------|
| A1     | 192.238.16.0     | 255.255.255.252   | 192.238.16.3    | 192.238.16.1 - 192.238.16.2      |
| A2     | 192.238.4.0      | 255.255.255.252   | 192.238.4.3     | 192.238.4.1 - 192.238.4.2        |
| A3     | 192.238.0.0      | 255.255.254.0     | 192.238.1.255   | 192.238.0.1 - 192.238.0.254      |
| A4     | 192.238.2.128    | 255.255.255.248   | 192.238.2.135   | 192.238.2.129 - 192.238.2.134    |
| A5     | 192.238.2.64     | 255.255.255.252   | 192.238.2.67    | 192.238.2.65 - 192.238.2.66      |
| A6     | 192.238.2.0      | 255.255.255.192   | 192.238.2.63    | 192.238.2.1 - 192.238.2.62       |
| A7     | 192.238.8.32     | 255.255.255.252   | 192.238.8.35    | 192.238.8.33 - 192.238.8.34      |
| A8     | 192.238.8.0      | 255.255.255.224   | 192.238.8.31    | 192.238.8.1 - 192.238.8.30       |
| A9     | 192.237.64.0     | 255.255.255.252   | 192.237.64.3    | 192.237.64.1 - 192.237.64.2      |
| A10    | 192.237.32.0     | 255.255.255.248   | 192.237.32.7    | 192.237.32.1 - 192.237.32.6      |
| A11    | 192.237.16.0     | 255.255.255.240   | 192.237.16.15   | 192.237.16.1 - 192.237.16.14     |
| A12    | 192.237.0.0      | 255.255.248.0     | 192.237.7.255   | 192.237.0.1 - 192.237.0.254      |
| A13    | 192.237.10.128   | 255.255.255.252   | 192.237.10.131  | 192.237.10.129 - 192.237.10.130  |
| A14    | 192.237.8.0      | 255.255.254.0     | 192.237.9.255   | 192.237.8.1 - 192.237.8.254      |
| A15    | 192.237.10.0     | 255.255.255.128   | 192.237.10.127  | 192.237.10.1 - 192.237.10.126    |
| A16    | 192.237.160.0    | 255.255.255.252   | 192.237.160.3   | 192.237.160.1 - 192.237.160.2    |
| A17    | 192.237.132.0    | 255.255.255.252   | 192.237.132.3   | 192.237.132.1 - 192.237.132.2    |
| A18    | 192.237.128.0    | 255.255.252.0     | 192.237.131.255 | 192.237.128.1 - 192.237.131.254  |
| A19    | 192.237.144.64   | 255.255.255.252   | 192.237.144.67  | 192.237.144.64 - 192.237.144.66  |
| A20    | 192.237.144.0    | 255.255.255.192   | 192.237.144.63  | 192.237.144.1 - 192.237.144.62   |
| A21    | 192.237.138.0    | 255.255.255.252   | 192.237.138.3   | 192.237.138.1 - 192.237.138.2    |
| A22    | 192.237.136.0    | 255.255.254.0     | 192.237.137.255 | 192.237.136.1 - 192.237.136.254  |

### Konfigurasi
1. Hololive (Getaway)

```
auto lo
iface lo inet loopback

auth eth0
iface eth0 inet dhcp

#A1
auto eth1
iface eth1 inet static
	address 192.238.16.1 #range IP A1
	netmask 255.255.255.252

#A16
auto eth2
iface eth1 inet static
	address 192.237.160.1 
	netmask 255.255.255.252

#A9
auto eth3
iface eth1 inet static
	address 192.237.64.1
	netmask 255.255.255.252
```

2. Holo-EN (Getaway)

```
auto lo
iface lo inet loopback

#A1
auto eth0
iface eth1 inet static
	address 192.238.16.2 #IP range sisa A1
	netmask 255.255.255.252
	getaway 192.238.16.1 #IP address Hololive

#A2
auto eth1
iface eth1 inet static
	address 192.237.4.1
	netmask 255.255.255.252

#A7
auto eth2
iface eth1 inet static
	address 192.238.8.33
	netmask 255.255.255.252
```

3. Holo-Myth (Getaway)

```
auto lo
iface lo inet loopback

#A2
auto eth0
iface eth1 inet static
	address 192.238.4.2
	netmask 255.255.255.252
	getaway 192.237.4.1 #IP address Holo-EN

#A3
auto eth1
iface eth1 inet static
	address 192.238.0.1
	netmask 255.255.254.0

#A4
auto eth2
iface eth1 inet static
	address 192.238.2.129
	netmask 255.255.255.248
```

4. Gura_Ame_Ina (Client)

```
#A3
auto eth0
iface eth1 inet static
	address 192.238.0.2
	netmask 255.255.254.0
	getaway 192.238.0.1 #IP address Holo-Myth
```

5. Kiara_Calli (Client)

```
#A3
auto eth0
iface eth1 inet static
	address 192.238.0.3
	netmask 255.255.254.0
	getaway 192.238.0.1 #IP address Holo-Myth
```

6. Project-Hope (Getaway)

```
auto lo
iface lo inet loopback

#A4
auto eth0
iface eth1 inet static
	address 192.238.2.130
	netmask 255.255.255.248
	getaway 192.238.2.129 #IP adress Holo-Myth

#A5
auto eth1
iface eth1 inet static
	address 192.238.2.65
	netmask 255.255.255.252
```

7. Irys (Client)

```
#A5
auto eth0
iface eth1 inet static
	address 192.238.2.66
	netmask 255.255.255.252
	getaway 192.238.2.65 #IP address Project-Hope
```

8. Holo-Council (Getaway)

```
auto lo
iface lo inet loopback

#A4
auto eth0
iface eth1 inet static
	address 192.238.2.131
	netmask 255.255.255.248
	getaway 192.238.2.129 #IP adress Holo-Myth

#A6
auto eth1
iface eth1 inet static
	address 192.238.2.1
	netmask 255.255.255.192
```

9. Kronii_Mumei (Client)

```
#A6
auto eth0
iface eth1 inet static
	address 192.238.2.2
	netmask 255.255.255.192
	getaway 192.238.2.1 #IP address Holo-Council
```

10. Bae_Fauna (Client)

```
#A6
auto eth0
iface eth1 inet static
	address 192.238.2.3
	netmask 255.255.255.192
	getaway 192.238.2.1 #IP address Holo-Council
```

11. HoloAdvent (Getaway)

```
auto lo
iface lo inet loopback

#A7
auto eth0
iface eth1 inet static
	address 192.238.8.34
	netmask 255.255.255.252
	getaway 192.238.8.33 #IP address Holo-EN

#A8
auto eth1
iface eth1 inet static
	address 192.238.8.1
	netmask 255.255.255.224
```

12. FuwaMoco (Client)

```
#A8
auto eth0
iface eth1 inet static
	address 192.238.8.2
	netmask 255.255.255.224
	getaway 192.238.8.1 #IP address HoloAdvent
```

13. Shiori_Nerissa (Client)

```
#A8
auto eth0
iface eth1 inet static
	address 192.238.8.3
	netmask 255.255.255.224
	getaway 192.238.8.1 #IP address HoloAdvent
```

14. Biboo (Client)

```
#A8
auto eth0
iface eth1 inet static
	address 192.238.8.4
	netmask 255.255.255.224
	getaway 192.238.8.1 #IP address HoloAdvent
```

15. Holo-JP (Getaway)

```
auto lo
iface lo inet loopback

#A9
auto eth0
iface eth1 inet static
	address 192.237.64.2
	netmask 255.255.255.252
	getaway 192.237.64.1 #IP address Hololive

#A10
auto eth1
iface eth1 inet static
	address 192.237.32.1
	netmask 255.255.255.248
```

16. DEV_IS (Getaway)

```
auto lo
iface lo inet loopback

#A10
auto eth0
iface eth1 inet static
	address 192.237.32.2
	netmask 255.255.255.248
	getaway 192.237.32.1 #IP address Holo-JP

#A11
auto eth1
iface eth1 inet static
	address 192.237.16.1
	netmask 255.255.255.240
```

17. Ririka_Raden (Client)

```
#A11
auto eth0
iface eth1 inet static
	address 192.237.16.2
	netmask 255.255.255.240
	getaway 192.237.16.1 #IP address DEV_IS
```

18. Ao (Client)

```
#A11
auto eth0
iface eth1 inet static
	address 192.237.16.3
	netmask 255.255.255.240
	getaway 192.237.16.1 #IP address DEV_IS
```

19. Hajime_Kanade (Client)

```
#A11
auto eth0
iface eth1 inet static
	address 192.237.16.4
	netmask 255.255.255.240
	getaway 192.237.16.1 #IP address DEV_IS
```

20. GEN:0 (Getaway)

```
auto lo
iface lo inet loopback

#A10
auto eth0
iface eth1 inet static
	address 192.237.32.3
	netmask 255.255.255.248
	getaway 192.237.32.1 #IP address Holo-JP

#A12
auto eth1
iface eth1 inet static
	address 192.237.0.1
	netmask 255.255.248.0
```

21. MiComet (Client)

```
#A12
auto eth0
iface eth1 inet static
	address 192.237.0.2
	netmask 255.255.248.0
	getaway 192.237.0.1 #IP address GEN:0
```

22. Sora_Robo_AZKi (Client)

```
#A12
auto eth0
iface eth1 inet static
	address 192.237.0.3
	netmask 255.255.248.0
	getaway 192.237.0.1 #IP address GEN:0
```

23. GEN:1 (Getaway)

```
auto lo
iface lo inet loopback

#A12
auto eth0
iface eth1 inet static
	address 192.237.0.4
	netmask 255.255.248.0
	getaway 192.237.0.1 #IP address GEN:0

#A14 - MEMBERS
auto eth1
iface eth1 inet static
	address 192.237.8.1
	netmask 255.255.254.0

#A13 - GAMERS
auto eth2
iface eth1 inet static
	address 192.237.10.129
	netmask 255.255.255.252
```

24. GAMERS (Getaway)

```
auto lo
iface lo inet loopback

#A13 - GEN:1
auto eth0
iface eth1 inet static
	address 192.237.10.130
	netmask 255.255.255.252
	getaway 192.237.10.129 #IP address GEN:1

#A15
auto eth1
iface eth1 inet static
	address 192.237.10.1
	netmask 255.255.255.128
```

25. Korone (Client)

```
#A15
auto eth0
iface eth1 inet static
	address 192.237.10.2
	netmask 255.255.255.128
	getaway 192.237.10.1 #IP address GAMERS
```

26. Okayu (Client)

```
#A15
auto eth0
iface eth1 inet static
	address 192.237.10.3
	netmask 255.255.255.128
	getaway 192.237.10.1 #IP address GAMERS
```

27. Mio (Client)

```
#A15
auto eth0
iface eth1 inet static
	address 192.237.10.4
	netmask 255.255.255.128
	getaway 192.237.10.1 #IP address GAMERS
```

28. FBK_Matsuri (Client)

```
#A14
auto eth0
iface eth1 inet static
	address 192.237.8.2
	netmask 255.255.254.0
	getaway 192.237.8.1 #IP address GEN:1
```

29. Aki_Hachama (Client)

```
#A14
auto eth0
iface eth1 inet static
	address 192.237.8.2
	netmask 255.255.254.0
	getaway 192.237.8.1 #IP address GEN:1
```

30. Holo-ID (Getaway)

```
auto lo
iface lo inet loopback

#A16
auto eth0
iface eth1 inet static
	address 192.237.160.2
	netmask 255.255.255.252
	getaway 192.237.160.1 #IP address Hololive

#A17
auto eth1
iface eth1 inet static
	address 192.237.132.1
	netmask 255.255.255.252

#A19
auto eth2
iface eth1 inet static
	address 192.237.144.65
	netmask 255.255.255.252
	
#A21
auto eth3
iface eth1 inet static
	address 192.237.138.0
	netmask 255.255.255.252
```

31. AREA15 (Getaway)

```
auto lo
iface lo inet loopback

#A17
auto eth0
iface eth1 inet static
	address 192.237.132.2
	netmask 255.255.255.252
	getaway 192.237.132.1 #IP address Holo-ID
	
#A18
auto eth1
iface eth1 inet static
	address 192.237.128.1
	netmask 255.255.252.0
```

32. Risu (Client)

```
#A18
auto eth0
iface eth1 inet static
	address 192.237.128.2
	netmask 255.255.252.0
	getaway 192.237.128.1 #IP address AREA15
```

33. Moona (Client)

```
#A18
auto eth0
iface eth1 inet static
	address 192.237.128.3
	netmask 255.255.252.0
	getaway 192.237.128.1 #IP address AREA15
```

34. lofi (Client)

```
#A18
auto eth0
iface eth1 inet static
	address 192.237.128.4
	netmask 255.255.252.0
	getaway 192.237.128.1 #IP address AREA15
```

35. holoro (Getaway)

```
auto lo
iface lo inet loopback

#A19
auto eth0
iface eth1 inet static
	address 192.237.144.66
	netmask 255.255.255.252
	getaway 192.237.132.1 #IP address Holo-ID

#A20
auto eth1
iface eth1 inet static
	address 192.237.144.1
	netmask 255.255.255.192
```

36. Ollie (Client)

```
#A20
auto eth0
iface eth1 inet static
	address 192.237.144.2
	netmask 255.255.255.192
	getaway 192.237.144.1 #IP address holoro
```

37. Anya (Client)

```
#A20
auto eth0
iface eth1 inet static
	address 192.237.144.3
	netmask 255.255.255.192
	getaway 192.237.144.1 #IP address holoro
```

38. Reina (Client)

```
#A20
auto eth0
iface eth1 inet static
	address 192.237.144.4
	netmask 255.255.255.192
	getaway 192.237.144.1 #IP address holoro
```

39. holoh3ro (Getaway)

```
auto lo
iface lo inet loopback

#A21
auto eth0
iface eth1 inet static
	address 192.237.138.1
	netmask 255.255.255.252
	getaway 192.237.132.1 #IP address Holo-ID

#A22
auto eth0
iface eth1 inet static
	address 192.237.136.1
	netmask 255.255.254.0
```

40. Zeta (Client)

```
#A22
auto eth0
iface eth1 inet static
	address 192.237.136.2
	netmask 255.255.254.0
	getaway 192.237.136.1 #IP address holoh3ro
```

41. Kaela (Client)

```
#A22
auto eth0
iface eth1 inet static
	address 192.237.136.3
	netmask 255.255.254.0
	getaway 192.237.136.1 #IP address holoh3ro
```

42. Kobo (Client)

```
#A22
auto eth0
iface eth1 inet static
	address 192.237.136.4
	netmask 255.255.254.0
	getaway 192.237.136.1 #IP address holoh3ro
```

## Revisi
1. CIDR
   https://youtu.be/Xfkgv68063Y





