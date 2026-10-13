1. Eksekusi seluruh profile yang ada :

2. a. Edit file profile `/etc/profile` dan tampilkan pesan sebagai berikut :

b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :
Ganti nama `/home/mahasiswa` dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada `/home/mahasiswa/.bash_profile` :
Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.

<p align="center">
  <img width="500" alt="1" src="https://github.com/user-attachments/assets/7b45a5f2-1e70-46f8-a5dc-5649aa38d637" />
</p>

<p align="center">
  <img width="650" alt="2" src="https://github.com/user-attachments/assets/4e217037-6de5-420b-a376-eb168e8f32f1" />
</p>

<p align="center">
  <img width="500" alt="3" src="https://github.com/user-attachments/assets/5cd30823-fe72-4ef4-a68c-9fd2e8a6989c" />
</p>

<p align="center">
  <img width="650" alt="4" src="https://github.com/user-attachments/assets/97bda88d-df3e-4648-90c9-da9bf91eab31" />
</p>

<p align="center">
  <img width="500" alt="5" src="https://github.com/user-attachments/assets/85faa21f-c0b2-483e-8cd7-3f01e3280f5d" />
</p>

<p align="center">
  <img width="650" alt="6" src="https://github.com/user-attachments/assets/b0b87d29-c152-476f-b5be-3c995d283031" />
</p>

<p align="center">
  <img width="500" alt="7" src="https://github.com/user-attachments/assets/e47f9328-08cb-4773-a20d-46fa868cf0fb" />
</p>

<p align="center">
  <img width="650" alt="8" src="https://github.com/user-attachments/assets/f798b42b-b83b-4ae7-b1c6-3eb094a162c6" />
</p>

<p align="center">
  <img width="500" alt="9" src="https://github.com/user-attachments/assets/1e4ee0ff-c243-42e8-87f7-7e4937a0216b" />
</p>

<p align="center">
  <img width="650" alt="10" src="https://github.com/user-attachments/assets/ec4432ff-68c6-4711-a8b0-c059ac69ca07" />
</p>

c. Jalankan instruksi substitute user, kemudian keluar dengan perintah exit

<p align="center">
  <img width="450" alt="11" src="https://github.com/user-attachments/assets/2d09692b-11a2-434f-87cf-6eec76ac27b1" />
</p>

* `su nik-isa`: Non-login shell. Menjaga environment dan working directory user sebelumnya, hanya mengeksekusi `.bashrc`.
* `su - nik-isa`: Full login shell. Menginisialisasi ulang seluruh environment (`PATH`, `HOME`, dll.) serta membaca `/etc/profile` diikuti file startup login user (`.bash_profile`, `.bash_login`, atau `.profile`).

---

**2. Prompt String (PS)**

a. Edit file `.bash_profile`, ganti prompt PS1 dengan `>`. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell

<p align="center">
  <img width="450" alt="1" src="https://github.com/user-attachments/assets/aa17e3cc-c18d-4b09-97d8-96df5cb3ae22" />
</p>

<p align="center">
  <img width="400" alt="2" src="https://github.com/user-attachments/assets/411850f7-d1d2-4b4d-9e80-7f6e751feb25" />
</p>

b. Eksperimen hasil PS1 :

<p align="center">
  <img width="500" alt="3" src="https://github.com/user-attachments/assets/8e81cb04-d673-4d55-87af-f5be717c5557" />
</p>

---

**3. Logout**

Edit file `.bash_logout`, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout

<p align="center">
  <img width="400" alt="1" src="https://github.com/user-attachments/assets/85849991-bf92-4462-ab3a-1830406b7af4" />
</p>

<p align="center">
  <img width="650" alt="2" src="https://github.com/user-attachments/assets/99977de2-6aa9-4f7f-b39c-d7a560c2a13e" />
</p>

Pengujian (*test*):

<p align="center">
  <img width="450" alt="3" src="https://github.com/user-attachments/assets/7c6a3ab9-0b09-4649-9f83-228bcc2dc688" />
</p>

<p align="center">
  <img width="650" alt="4" src="https://github.com/user-attachments/assets/a98d86aa-c337-4b94-80f8-8113d8efe2a5" />
</p>

---

**4. Bash Script**

a. Buat 3 buah script `p1.sh`, `p2.sh`, `p3.sh` dengan isi masing-masing :

<p align="center">
  <img width="350" alt="1" src="https://github.com/user-attachments/assets/14604547-5b46-4a6d-9489-59618c8c544b" />
</p>

<p align="center">
  <img width="350" alt="2" src="https://github.com/user-attachments/assets/9bee4624-f708-4531-b149-aa26ed2a3863" />
</p>

<p align="center">
  <img width="350" alt="3" src="https://github.com/user-attachments/assets/af4343d8-a33f-489b-9f31-0a1d159346eb" />
</p>

<p align="center">
  <img width="300" alt="4" src="https://github.com/user-attachments/assets/dd696ed0-1cdf-4230-a882-44f91f9d9bc3" />
</p>

<p align="center">
  <img width="350" alt="5" src="https://github.com/user-attachments/assets/76533b3b-f144-451e-9cc7-4de4642bb007" />
</p>

<p align="center">
  <img width="300" alt="6" src="https://github.com/user-attachments/assets/596240a9-7cb6-4b4d-9e80-7f6e751feb25" />
</p>

b. Jalankan script tersebut sebagai berikut :

<p align="center">
  <img width="600" alt="7" src="https://github.com/user-attachments/assets/79e24293-9799-4c33-b350-a4c8bb341856" />
</p>

<p align="center">
  <img width="500" alt="8" src="https://github.com/user-attachments/assets/bc17c3b2-0bb3-443a-8d1b-79f9a8606900" />
</p>

<p align="center">
  <img width="400" alt="9" src="https://github.com/user-attachments/assets/dc6d8811-2cd4-4017-8a3c-16f275886420" />
</p>

<p align="center">
  <img width="400" alt="10" src="https://github.com/user-attachments/assets/8916146b-4e4c-4c49-bf99-88d0617f24b9" />
</p>

<p align="center">
  <img width="550" alt="11" src="https://github.com/user-attachments/assets/66f96621-8a9c-4452-a6c4-bd35332b3a9e" />
</p>

---

**5. Jobs**

a. Buat shell-script yang melakukan loop dengan nama `pwaktu.sh`, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.

<p align="center">
  <img width="350" alt="1" src="https://github.com/user-attachments/assets/09ed72e9-289e-4839-b99f-c3c2719a7ac7" />
</p>

<p align="center">
  <img width="300" alt="2" src="https://github.com/user-attachments/assets/bdb61bf5-46be-4629-9e4d-2a7180f4c0c3" />
</p>

<p align="center">
  <img width="400" alt="3" src="https://github.com/user-attachments/assets/ba07eac9-a212-4f34-9949-6b8f6301b612" />
</p>

b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :

<p align="center">
  <img width="600" alt="4" src="https://github.com/user-attachments/assets/7b42618d-a0cd-4b71-954c-f7641b732065" />
</p>

c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

<p align="center">
  <img width="450" alt="5" src="https://github.com/user-attachments/assets/42a7a325-b19f-4464-a3aa-e67b13489a44" />
</p>

d. Stop program background dengan utilitas kill

<p align="center">
  <img width="500" alt="6" src="https://github.com/user-attachments/assets/b09e146f-1f38-477d-8f5d-eea9622065b0" />
</p>

<p align="center">
  <img width="450" alt="7" src="https://github.com/user-attachments/assets/58e55af6-7e65-42a1-9df9-5cbc0f000633" />
</p>

---

**6. History**

a. Ganti nilai HISTSIZE dari 1000 menjadi 20

<p align="center">
  <img width="350" alt="1" src="https://github.com/user-attachments/assets/a6a91fae-9b39-4025-94d4-357daaaeaa3e" />
</p>

b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan

<p align="center">
  <img width="350" alt="2" src="https://github.com/user-attachments/assets/793a08f6-8c83-4438-8a6b-aed26af635d6" />
</p>

c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history buffer

<p align="center">
  <img width="350" alt="3" src="https://github.com/user-attachments/assets/97a2a915-e122-4b83-a09c-4ec1d5521d66" />
</p>

d. Ulangi instruksi pada history buffer nomor 150

<p align="center">
  <img width="300" alt="4" src="https://github.com/user-attachments/assets/ac7ddec9-0487-4efe-b1dc-b1e76cf6a789" />
</p>

<p align="center">
  <img width="300" alt="6" src="https://github.com/user-attachments/assets/acfd8446-a55a-4af1-b94e-5e9e5e467db3" />
</p>
