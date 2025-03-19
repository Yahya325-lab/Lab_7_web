![image](https://github.com/user-attachments/assets/9794b357-8fec-4cda-a0c9-bd75101b5c53)|Nama|NIM|Kelas|Matkul|
|----|---|-----|------|
|Yahya Ramadhan|312310401|TI.23.A4|Pemograman Web 2|

&nbsp;  <br> &nbsp;

**Tugas 1**

&nbsp;  <br> &nbsp;


1. Download Code Igniter terlebih dahulu <br>
  &nbsp;  <br> &nbsp;
2. Cek Code Igniter nya dulu dengan "php spark"
   ![image](https://github.com/user-attachments/assets/d59961bc-9e35-4f5f-8d6b-4d032d4964fb)
  <br> &nbsp;  <br> &nbsp;
3. Nyalakan Code Igniter nya dengan "php spark serve"
   <br> &nbsp; <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/e1107800-805a-402d-a216-63950a7a890d)

<br> &nbsp;<br> &nbsp;
   kita cek di localhost:8080
   ![image](https://github.com/user-attachments/assets/332d02bb-7211-45fa-9cd9-954cb5663ab8)

  Kalau sudah seperti itu berarti sudah work code igniter nya

<br> &nbsp; <br> &nbsp;
4. Sekarang di Vscode buka folder **app/Controller/Home.php**
   ![image](https://github.com/user-attachments/assets/4a3d2da8-2b20-4bee-9fd6-533c68216605)

   Hapus tanda **( ; )** di akhir kalimat welcome_message
<br> &nbsp; <br> &nbsp;

5. Sekarang tambahkan rute di **app/config/Routes.php**
   |$routes->get('/', 'Home::index');|
   |----|
   
   ![image](https://github.com/user-attachments/assets/80264df0-ef16-4573-b2c4-cde21b007e45)
<br> &nbsp; <br> &nbsp;

6. Tambahkan rute baru di **Routes.php** dengan
    |$routes->get('/about', 'Page::about');|
    |----|
    |$routes->get('/contact', 'Page::contact');|
    |$routes->get('/faqs', 'Page::faqs');|
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/c4d847cc-946d-4578-9fb6-6c49fb0b6ff5)
<br> &nbsp; <br> &nbsp;

7. Lalu di shell ketik **php spark routes** untuk mengetahui rute nya
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/002181ca-a160-47fa-ae04-055f60fbb3ad)
  <br> &nbsp;<br> &nbsp;

8. Ketik di localhost nya http://localhost:8080/about
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/831d0447-0db2-4574-883e-d22e4d913245)
   Kalau output nya **404 File Not Found** berarti itu tandanya sudah berhasill
    <br> &nbsp;<br> &nbsp;

9. Buat controller dengan nama **page.php**
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/71bf34c1-4c82-463b-890c-9b1f1cb347f0)
  <br> &nbsp;<br> &nbsp;

10. Lalu refresh page nya, kalau muncul seperti ini berarti sudah work
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/0566df05-d652-4685-928e-22d30fa0f43d)
   <br> &nbsp;<br> &nbsp;

11. Membuat View
     <br> &nbsp;
    Buat file baru di direktori **app/Views/about.php**
    ![image](https://github.com/user-attachments/assets/87a22ee3-b432-4480-86f7-f74665ca192b)
    <br> &nbsp;<br> &nbsp;
    
    <br> &nbsp;<br> &nbsp;
12. Ubah method **about** pada class **Controller Page**
    ![image](https://github.com/user-attachments/assets/34bf20fb-905b-4838-8f9e-34ffd46cbcd3)
    Gunanya untuk menambah elemen ( h1 ), ( hr ), dan elemen ( p ) di dalam web nya
    
    <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/d172eeda-515b-480f-978a-604df293a8c4)
    Hasil dari file **about.php** dan perubahan method about pada class **Controller Page**
     <br> &nbsp;<br> &nbsp;

13. Buat file **Style.css** di folder Public
     <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/61bfb0f1-244c-4cf3-a186-01ef93e7ae14)
     <br> &nbsp;
    Isi CSS nya dari praktikum yang dulu

14. Buat folder **template** di dalam folder **app/view**, di dalam folder **template** dan buat 2 file baru, **header** dan **footer**
     <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/6a168b17-dc3a-4000-944c-42fdf98fe8ff)
    <br> &nbsp;
    Template header.
    <br> &nbsp;<br> &nbsp;
    ![image](https://github.com/user-attachments/assets/55fa9401-9e32-42bb-b14c-c6bec3622eae)
    <br> &nbsp;
    Template Footer.
    <br> &nbsp;<br> &nbsp;

15. Kemudian ubah file **app/view/about.php** dengan menambahkan include header dan footer
    <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/aafea166-49fd-4440-b6a5-52196b607fee)
    <br> &nbsp;
    Setelah itu refresh page http://localhost:8080/about nya, kalau berhasil maka jadinya seperti ini
     <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/1264e4cd-4d26-4af8-81b8-edf4b41d5337)
    <br> &nbsp;<br> &nbsp;

**Tugas :**
<br> &nbsp;
Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua
link pada navigasi header dapat menampilkan tampilan dengan layout yang sama.
<br> &nbsp;
Ini tampilan Kontak
<br> &nbsp;
![image](https://github.com/user-attachments/assets/bc2428b4-984e-4cb9-a577-e4bdabeffb6a)
<br> &nbsp;
Ini tampilan about
<br> &nbsp;
 ![image](https://github.com/user-attachments/assets/1264e4cd-4d26-4af8-81b8-edf4b41d5337)

 <br> &nbsp;<br> &nbsp;
 
**================================================================================**

 <br> &nbsp;<br> &nbsp;
 **Tugas 2**

 1. Buat database bernama **lab_ci4** dan buat tabel bernama **artikel** di dalam nya, dan di dalam tabel artikel ada id, judul, isi, gambar, status, slug
     <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/8519881d-4b6c-426f-862c-674c5d37fad2)
  <br> &nbsp;<br> &nbsp;

2. Koneksikan database
   <br> &nbsp;
   Buka file yang bernama **.env** dan temukan tulisan **Database**
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/360d4d43-1a20-4d9b-bfce-abd5a4027b84)
   <br> &nbsp;
   di dalam tulisan **"database.default.database"** isi dengan nama database yang sebelumnya dibuat, lalu jika menggunakan password pada tulisan **"database.default.password"**
 bisa diisi
     <br> &nbsp;<br> &nbsp;

3. Buat file baru di dalam folder **app/Models** yang bernama **ArtikelModel.php**
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/b5305c27-d64a-4912-8cf8-0e5b12da44fd)
    <br> &nbsp;

4. Buat kontroller baru dengan nama **Artikel.php** pada folder **app/Controllers**
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/6c408e9d-2668-42fd-9732-6b01d84a1b5f)
   <br> &nbsp;
   
     





    

    





