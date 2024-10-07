# Report-EH-Praktikum


| Nama      | NRP         |
  |-----------|-------------|
  | Hasan | 5027231073  | 

  # STEP
  
1.	Pertama kita lakukan tes pada IP 10.15.42.245 untuk mengecek apakah sudah tersambung, dengan command (ping 10.15.42.245)
![step 1](https://github.com/user-attachments/assets/66a53a63-581a-4577-91fe-7bee3716dd84)

2.	Setelah itu kita lakukan scanning menggunakan nmap pada IP tersebut dengan command (nmap -Pn 10.15.42.245)
![step 2](https://github.com/user-attachments/assets/2d88d512-0772-4dd6-bbc0-465a1ef06a05)

3.	Saya menemukan 2 port yang terbuka, yaitu port [21 ftp] & port [22 ssh]
![step 3](https://github.com/user-attachments/assets/487b0edb-f5f4-42ba-89ee-4867dd29bf29)

4.	Setelah itu saya ingin mengecek versi service dari port yang terbuka menggunakan command (nmap -sV -Pn 10.15.42.245)
![step 4](https://github.com/user-attachments/assets/1ad46f0b-cf75-4eac-be5a-011f15ecc975)

5.  Lalu saya menemukan kejanggalan username di readme
![username di readme (step5)](https://github.com/user-attachments/assets/c3905c29-5688-4132-b5e6-16eb7ec974c5)

6.  Lalu saya menemukan hash dari username ethack di List.xyz
![username ethack, hash, email di list xyz (step 6)](https://github.com/user-attachments/assets/b7c0fb7d-9e3b-4795-98f6-50afc6cfb864)

7.  Setelah itu saya menggunakan hashcat untuk menemukan passwordnya
![hashcat (step7)](https://github.com/user-attachments/assets/420c28c3-a74f-4379-9bec-0eed935d1688)

8.  Setelah dapat passwordnya saya login menggunakan ftp
![berhasil login di user ethack (step8)](https://github.com/user-attachments/assets/9a2814a2-8dbb-4c8c-808d-492f444b6e08)

9.  Saya melakukan nmap ulang karena hasil nmap diawal tidak lengkap 
![step 9](https://github.com/user-attachments/assets/8b991f3a-481f-4996-a282-576811dde2a6)

10.  Lalu baru disini saya menemukan port 487 (port dari web) Open
![hasil nmap (step10)](https://github.com/user-attachments/assets/2efc12fd-282e-4a22-ace6-5603e7d61ff5)

11.  Setelah itu saya masuk ke webnya
![masuk web (11)](https://github.com/user-attachments/assets/e6e1aaff-4c9c-447f-8496-532cd7840fa7)

12.  Di web saya menemukan sesuatu di trial dan ternyata setelah saya inspect itu ada plugin (wpdiscuz)
![berhasil menemukan sesuatu yang suspicious (step11)](https://github.com/user-attachments/assets/32b9e2fd-5a49-42fc-a56d-c5687d2e9c74)

![melihat sesuatu yang aneh -plugin (step12)](https://github.com/user-attachments/assets/a70938ac-a403-4fac-a31d-085b2cc60876)

13.  Setelah itu saya metasploit
![kita sploit dulu (step13)](https://github.com/user-attachments/assets/f37ada53-a4cd-40a1-aa1d-77f211c0306d)

14.  Disini saya show options untuk melihat apa yang bisa diganti
![cari inpo wpdiscuz (step14)](https://github.com/user-attachments/assets/4bbd7c3e-0e7f-4582-8114-30aff2d19f7b)

15.  berhasil masuk dan ngerun
![berhasil masuk (step15)](https://github.com/user-attachments/assets/473c4123-317a-475f-8271-a68cf5914824)

16.  Selesai 
![izin masuk (kelar)](https://github.com/user-attachments/assets/2664445d-7368-43dd-bf01-38962ef3dc0f)
 


