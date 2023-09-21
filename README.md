<h1>Praktikum Modul 1 Jaringan Komputer</h1>
<h3>Kelompok I07</h3>

| NAME                          | NRP       |
|-------------------------------|-----------|
|Pascal Roger Junior Tauran     |5025211072 |
|Mochammad Naufal Ihza Syahzada |5025211260 |



## Number 1
```
User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
```
### 1A

```
Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? 
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

### 1B
```
Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? 
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

### 1C

```
Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

### 1D

```
Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 



## Number 2
```
Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
```
Solution:<br>

```sh
//No current solution
```

Explanation:
- `No current explanation` 


## Number 3
```
Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
```

### 3A

```
Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

### 3B
```
Protokol layer transport apa yang digunakan?
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

## Number 4
```
Berapa nilai checksum yang didapat dari header pada paket nomor 130?
```
Solution:<br>

![Number4_image](https://media.discordapp.net/attachments/824131614073683968/1154435177255288943/Screenshot_2023-09-18_205640.png?width=681&height=671)  

```sh
Frame 130: 196 bytes on wire (1568 bits), 196 bytes captured (1568 bits) on interface \Device\NPF_{3F96C891-C513-447E-9B66-6C81A5C93077}, id 0
Ethernet II, Src: 02:e4:90:54:f3:42 (02:e4:90:54:f3:42), Dst: zte_e8:05:1c (28:c8:7c:e8:05:1c)
Internet Protocol Version 4, Src: 192.168.1.19, Dst: 74.125.130.139
User Datagram Protocol, Src Port: 57296, Dst Port: 443
    Source Port: 57296
    Destination Port: 443
    Length: 162
    Checksum: 0x18e5 [unverified]
    [Checksum Status: Unverified]
    [Stream index: 9]
    [Timestamps]
    UDP payload (154 bytes)
QUIC IETF
QUIC IETF
```
Explanation:
- First go to the Header number 130, afterwards double click it.
- Then click on the `User Datagram Protocol`, it will open a drop down tab.
- There we can search for the `Checksum value`, which in this case is `0x18e5` 

## Number 5
```
Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
```
### 5A

```
Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

### 5B
```
Port berapakah pada server yang digunakan untuk service SMTP?
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

### 5C

```
Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?
```
Solution:<br>
```sh
//No current solution
```
Explanation:
- `No current explanation` 

## Number 6
```
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.
```
Solution:<br>

```sh
//No current solution
```

Explanation:
- `No current explanation` 

## Number 7
```
Berapa jumlah packet yang menuju IP 184.87.193.88?
```
Solution:<br>

![Number7_image](https://media.discordapp.net/attachments/906158395617320980/1154435868950548531/Screenshot_2023-09-18_193024.png)  

```sh
ip.dst == 184.87.193.88
```

Explanation:
- Since the question asks for the packets that are  `menuju IP 184.87.193.88`, it means that the `destination` of the packets are `184.87.193.88`
- `ip.dst` is for filtering the `IP destinations` which in this case is  `184.87.193.88`
- Afterwards we count number of packets which are `6`

## Number 8
```
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)
```
Solution:<br>

```sh
//No current solution
```

Explanation:
- `No current explanation` 

## Number 9
```
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!
```
Solution:<br>

![Number9_image](https://media.discordapp.net/attachments/824131614073683968/1154435176940711996/Screenshot_2023-09-18_203242.png?width=627&height=671)

```sh
ip.src == 10.51.40.1 && ip.dst != 10.39.55.34
```

Explanation:
- The question asks for packets that `berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34` which means that it is looking for packets which `source` is IP `10.51.40.1` and the `destination` is not IP `10.39.55.34` 
- `ip.src` is for filtering the `IP sources` which in this case is  `10.51.40.1`
- `ip.dst` is for filtering the `IP desinations` which in this case is NOT `10.39.55.34` which is denoted by the `!=`.

## Number 10
```
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet
```

Solution:<br>

![Number10_image](https://media.discordapp.net/attachments/824131614073683968/1154435176592592996/Screenshot_2023-09-18_202027.png)

```sh
Frame 87: 92 bytes on wire (736 bits), 92 bytes captured (736 bits) on interface tap2, id 0
Ethernet II, Src: 0c:c8:32:27:00:00 (0c:c8:32:27:00:00), Dst: 26:82:4f:e4:c2:07 (26:82:4f:e4:c2:07)
Internet Protocol Version 4, Src: 172.16.0.4, Dst: 172.16.0.254
Transmission Control Protocol, Src Port: 23, Dst Port: 57784, Seq: 13, Ack: 26, Len: 26
Telnet
    Data: dhafin:kesayangannyak0k0\r\n
```

Explanation:
- First we filter out with `telnet`
- Then we browse the headers and look into the `Telnet` drop down tab until we find one where the data resembles a username and password which we find in `header number 87` and the login credentials are `dhafin:kesayangannyak0k0`
