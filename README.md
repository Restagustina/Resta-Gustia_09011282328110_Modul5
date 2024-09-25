## Nama : Resta Gustina
## Kelas : SK3B
## NIM : 09011282328110

<div align="center">
   
## Job Control
</div>
   
<div align="justify">
  <br>
   <br>

#### 1. Eksekusi seluruh profile yang ada :
   
a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :
**echo “Profile dari /etc/profile”**

![1 a selesai](https://github.com/user-attachments/assets/1143c41f-9cf4-491a-9272-ad07dbcbed1d)



![1 a sudo nano](https://github.com/user-attachments/assets/fa0c28e0-446e-43db-abd8-64a91d8d0ae3)



b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :

/home/stD02001/.bash_profile

/home/. stD02001/.bash_login

/home/mahasiswa/.profile

/home/mahasiswa/.bashrc

Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap
file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :
**echo “Profile dari .bash_profile”**
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang
bersangkutan.

**/home/stD02001/.bash_profile**

![1b masuk bash profile](https://github.com/user-attachments/assets/8a5e04f4-caf7-4e85-a5fc-840eff6d77e5)

![1 b as profile](https://github.com/user-attachments/assets/74532881-8b18-4b0c-9188-e5ebf49b459a)



**/home/. stD02001/.bash_login**

![1  b masuk bash login](https://github.com/user-attachments/assets/7e6404a8-b04f-4962-8db5-b9cbec61b59a)


![1 b tampilan bash login](https://github.com/user-attachments/assets/569c7d65-44c9-4ed6-b975-7bcf5f696b2e)



**/home/mahasiswa/.profile**

![1 b  profile](https://github.com/user-attachments/assets/740853ed-9ca7-423a-b2aa-209e59325d99)



![1 b  profile (tampilan)](https://github.com/user-attachments/assets/e64197bd-8558-46ec-bb1f-73159c42e582)




**/home/mahasiswa/.bashrc**


![1 b  bashsrc](https://github.com/user-attachments/assets/f5f66abe-0fe7-4b90-afcb-915fa62c6d94)


![1 b tampilan  bashsrc](https://github.com/user-attachments/assets/ce956f12-7330-4bba-8ee3-e13d414cf080)


c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:

**$ su mahasiswa**

**$ exit**

![1 c ](https://github.com/user-attachments/assets/0feb3b5a-05fe-4fbd-acb5-6be0362e2216)

kemudian gunakan opsi – sebagai berikut :

**$ su – mahasiswa**

**$ exit**

![1 c su-mahasiswa](https://github.com/user-attachments/assets/51206a4e-fd94-4147-8ca7-0748f876cb7d)


Jelaskan perbedaan kedua utilitas tersebut.

= Perbedaannya adalah jika menggunakan perintah su mahasiswa, hanya identitas pengguna yang berubah sementara lingkungan (environment) dari pengguna sebelumnya tetap dipertahankan. Sebaliknya, perintah su - mahasiswa melakukan login baru sepenuhnya, termasuk memuat ulang seluruh lingkungan pengguna baru dari awal.



## **2. Prompt String (PS)**
   
a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan
parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell
PS1=‟> „
export PS1

![2 sudo nano bash profile](https://github.com/user-attachments/assets/36ebc845-e551-4fc0-bb83-0a3bd26ad7af)


![2a bash profile](https://github.com/user-attachments/assets/cd7cf832-5775-47b8-b4cd-686c446c2a7f)





b. Eksperimen hasil PS1 :
$ PS1=“\! > “
69 > PS1=”\d > “
Mon Sep 23 > PS1=”\t > “
10:10:20 > PS1=”Saya=\u > “
Saya=mahasiswa > PS1=”\w >”
~ > PS1=\h >”

![2b](https://github.com/user-attachments/assets/99c0067b-8558-47fc-892e-1a99b70e310d)



## **3. Logout**

Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout
Echo “Terima kasih atas sesi yang diberikan”
Sleep 5
clear

![3 bash logout](https://github.com/user-attachments/assets/0972a2be-f9ef-43a3-a4fe-225bd00b8b3c)

![3  a logout](https://github.com/user-attachments/assets/3d4acdc6-8b13-4f10-b581-13d673e89d85)


![3  a fiks terimakasih](https://github.com/user-attachments/assets/af223ef4-3a1d-4378-9278-1133bfebaa2f)





## **4. Bash script**

a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :

**p1.sh**

#! /bin/bash

echo “Program p1”

ls –l

![nano p1](https://github.com/user-attachments/assets/8e44645a-fa5e-4de4-ba33-9eeae330ce2c)


![4a p1](https://github.com/user-attachments/assets/5fdb86c4-50ba-491d-8c31-d1f2019a25dc)




**p2.sh**

#! /bin/bash

echo “Program p2”

who

![4 nano p2](https://github.com/user-attachments/assets/60d7bf3c-a5ce-4168-add6-38ff956275a0)

![4 p2 who](https://github.com/user-attachments/assets/11404759-d5a9-41f5-bd8f-d566c73f9f40)




**p3.sh**

#! /bin/bash

echo “Program p3”

ps x


![4 nano p3](https://github.com/user-attachments/assets/497e4db0-6882-46f1-8f8d-918190827298)


![4 gnu p3](https://github.com/user-attachments/assets/38d4ba0a-8315-4d92-bcae-fc75b654a8f5)




b. Jalankan script tersebut sebagai berikut :

**$ ./p1.sh ; ./p3.sh ; ./p2.sh**

![4b](https://github.com/user-attachments/assets/3d8e4a9b-89f3-4f49-92cf-46ee1c2c4155)

![4b lanjutan](https://github.com/user-attachments/assets/de3ba93b-eeeb-455b-800d-b8c37a42da02)

![4b lanjutan (2)](https://github.com/user-attachments/assets/091e6ba0-0221-4c22-9942-9c921174b4d1)



**$ ./p1.sh &**

![4 p1 sh ](https://github.com/user-attachments/assets/d089e239-e657-4e00-b458-fb35443736d3)




**$ ./p1.sh $ ./p2.sh & ./p3.sh &**

![4b 3](https://github.com/user-attachments/assets/faa33199-0686-4ca5-9dd4-0f61c73b4040)

![4b 3(lanjutan)](https://github.com/user-attachments/assets/774404c8-2479-4249-a78b-a11fcb805718)



**$ ( ./p1.sh ; ./p3.sh ) &**

![4b 4](https://github.com/user-attachments/assets/779f8d36-7853-437c-9e51-8c4f1ca367b1)



## **5. Jobs**

**a.** Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.

#!/bin/bash
while [ true ]

do

date >> hasil

sleep 10

done


![5 a soal](https://github.com/user-attachments/assets/daf52262-3bd5-4b8b-adca-c6d639d2ab87)

![5a](https://github.com/user-attachments/assets/1f2f502b-6f7e-4bcf-8b28-766d9c4b832e)



**b.** Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :

$ jobs

$ find / -print > files 2>/dev/null &

$ jobs


![5b](https://github.com/user-attachments/assets/11563226-07c8-43fa-9af8-a2187238f596)




**c.** Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

$ fg %1

$ bg

![5c](https://github.com/user-attachments/assets/cf11ab5f-408c-4f44-95e1-73f78e55ce34)




**d.** Stop program background dengan utilitas kil

$ ps x

$ kill [Nomor PID]

![5d](https://github.com/user-attachments/assets/214abd55-6f52-4690-8472-8ca10f630250)




## **6. History**

**a.** Ganti nilai HISTSIZE dari 1000 menjadi 20

$ HISTSIZE=20

$ h

![6a](https://github.com/user-attachments/assets/e7ea129f-b54e-4b98-a5da-d4f075ea6868)




**b.** Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan

$ !-5

![6b](https://github.com/user-attachments/assets/337b6da7-effc-49f0-ab5d-ee2bc24ea472)




**c.** Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer

$ !!

![6c](https://github.com/user-attachments/assets/80946081-ffdd-4631-8346-5887c0be462d)




**d.** Ulangi instruksi pada history bufer nomor 150

$ !150

![6d](https://github.com/user-attachments/assets/8534dc17-68f8-4afc-a319-2678a59361a6)




**e.** Ulangi instruksi dengan prefix “ls”

$ !ls

![63](https://github.com/user-attachments/assets/2bb10278-6d29-4469-a237-3809d6387dff)


</div>

<br>
<br>
