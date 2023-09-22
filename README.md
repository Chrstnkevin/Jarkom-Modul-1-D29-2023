# Laporan Resmi Jarkom Modul 01 Kelompok D29 2023

| Nama        | NRP | Kelas    |
|-------------|------|---------|
| Ferza Noveri    | 5025211097   | Jarkom B|
| Christian Kevin Emor  | 5025211153   | Jarkom B|

## 1. User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.
### a. Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? 
### b. Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? 
```Penjelasan : Kode unggah file adalah “STOR”```

<img width="526" alt="Screenshot 2023-09-22 at 14 23 01" src="https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/110340182/c31d6408-8051-483b-919d-65a4367a18a9">

### c. Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut? 
### d. Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut? 

<img width="526" alt="Screenshot 2023-09-22 at 14 26 07" src="https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/110340182/15864c9d-a97d-48fe-9030-69e8a88cbb2a">

##### Kendala: Tidak ada kendala selama pengerjaan

## 2. Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer! 

<img width="526" alt="Screenshot 2023-09-22 at 14 27 52" src="https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/110340182/9cbc016d-35ad-47f0-bfb7-12890cb00fe5">

<img width="526" alt="Screenshot 2023-09-22 at 14 28 34" src="https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/110340182/535e9c5f-8cb3-41b9-88aa-94c430230ab9">

##### Kendala: Tidak ada kendala selama pengerjaan

## 3. Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
### a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
### b. Protokol layer transport apa yang digunakan?

<img width="526" alt="Screenshot 2023-09-22 at 14 31 19" src="https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/110340182/5a545e6b-b536-44f6-9d25-a240632c9d32">

##### Kendala: Tidak ada kendala selama pengerjaan

## 4. Berapa nilai checksum yang didapat dari header pada paket nomor 130?

<img width="526" alt="Screenshot 2023-09-22 at 14 32 03" src="https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/110340182/9a13b5b2-184f-4785-93a7-5a20f541694a">

##### Kendala: Tidak ada kendala selama pengerjaan

## 5. Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
### a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
### b. Port berapakah pada server yang digunakan untuk service SMTP?
### c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

<img width="422" alt="Screenshot 2023-09-22 at 14 33 13" src="https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/110340182/89660989-4a69-4f7c-be77-86c06704cc32">

##### Kendala: Tidak ada kendala selama pengerjaan

### FILTERING
## 7. Berapa jumlah packet yang menuju IP 184.87.193.88?

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/1cb7a0f4-67fc-4ce2-a880-cbdd075eb6f7)

Untuk mencari jumlah packet bisa menggunakan ip.dst untuk menentukan alamat tujuan yang tepat menuju alamat 184.87.193.88

#### Jawaban: ip.dst == 184.87.193.88 dan mendapatkan bahwa terdapat 6 packet
![Screenshot 2023-09-22 084055](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/8a3a8192-99a1-4b12-a02c-e01b81e52382)

##### Kendala: Tidak ada kendala selama pengerjaan



## 8. Berikan kueri filter

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/fd15d478-d666-4260-ae76-1dc4fc2234ec)

Untuk mencari tahu kueri yang digunakan bisa menggunakan tcp.dstprot untuk mencari protokol yang menuju port 80

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/d237a81a-f196-4f91-ad3c-72df883433fd)

Refrensi: Link Github Modul 1

#### Jawaban: tcp.dstport == 80 || udp.dstport == 80
- 'tcp.dstport' == 80: Bagian ini berarti aturan ini akan mencocokkan paket-paket yang menggunakan protokol TCP (seperti HTTP) dan memiliki port tujuan 80
- 'udp.dstport' == 80: Bagian ini berarti aturan ini juga akan mencocokkan paket-paket yang menggunakan protokol UDP dan memiliki port tujuan 80

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/a53e0476-04da-425b-b200-2caee7f324cd)

##### Kendala: Tidak ada kendala selama pengerjaan

## 9. Berikan kueri filter

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/a78971b6-d25b-4be3-a210-2bc1d6e0aa59)

Untuk mencari tahu kueri yang bisa digunakan kita bisa menggunakan src (untuk mencari berasal dari mana) dan dst (untuk mencari ip yang menuju suatu alamat). Untuk mencari tidak maka bisa menggunakan Comparison Operator !=

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/226f372b-4247-4260-9040-07375acaf2eb)

Refrensi: Link Github Modul 1

#### Jawaban : ip.src == 10.51.40.1 && ip.dst != 10.39.55.34
![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/b0f5c572-e023-493b-9b1d-701231442fc0)

##### Kendala: Tidak ada kendala selama pengerjaan

## 10. Kredensial yang benar ketika user mencoba menggunakan Telnet

Untuk mencari tahu bagaimana kredensial yang benar ketika menggunakan Telnet adalah seperti berikut

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/26f96904-c26a-4e36-852f-8e509b4cedf7)
- Dalam file PCAP, dilakukan penyaringan untuk menemukan paket yang hanya menggunakan protokol Telnet

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/58654b6d-26d2-4977-a128-eaf3eb05c30f)
- Pilih paket yang paling bawah dan follow tcp stream

![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/5259a78b-f8a3-4c1e-b92e-8670302e8d40)
- Didapatkan user dan pass
##### Jawaban: dhafin:kesayangannyak0k0 
![image](https://github.com/Chrstnkevin/Jarkom-Modul-1-D29-2023/assets/97864068/1c95dd29-bdf3-4356-81dd-6ceb83f630be)

##### Kendala: Username awalnya tidak sesuai, karena di display yaitu ddhhaaffiinn akan tetapi saat diganti hanya menjadi dhafin jawaban bisa disubmit

