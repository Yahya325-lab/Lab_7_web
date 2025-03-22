|Nama|NIM|Kelas|Matkul|
|----|---|-----|------|
|Yahya Ramadhan|312310401|TI.23.A4|Pemograman Web 2|

&nbsp;  <br> &nbsp;
**================================================================================**
<br> &nbsp;

                                                                   Tugas 1

<br> &nbsp;
**================================================================================**
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

                                                                  Tugas 2

**================================================================================**


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

5. Buat folder dengan nama **artikel** pada direktori **app/views**, kemudian buat file baru bernama **index.php**
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/38e43477-bff0-499f-a0d3-cf94349a9481)
     <br> &nbsp;
   Lalu buka web http://localhost:8080/artikel, dan lihat apa sudah berubah apa belum, tampilannya akan seperti ini
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/0fa33fa2-28ca-42bf-9d15-2c070657d206)
     <br> &nbsp; <br> &nbsp;

6. Kemudian di MySQL insert beberapa kalimat ke dalam table **artikel** yang terhubung di database
    <br> &nbsp; <br> &nbsp;

7. Lalu refresh web **artikel** nya dan cek tampilan sudah muncul apa belum
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/212a90c7-5266-493a-9bb9-34009ab6e547)
    <br> &nbsp; <br> &nbsp;

8. Buat tampilan detail artikel dengan menambah fungsi baru pada **app/Controllers/artikel.php** dengan nama **View()**
     <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/278ad721-ad9e-4184-b5d2-97d143861cf5)
    <br> &nbsp; <br> &nbsp;
   
   Buat view baru untuk halaman detail artikelnya pada direktori **app/views/artikel** dengan nama **detail.php**
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/b17b3f87-279a-4896-b23d-74dc67fac8c0)
    <br> &nbsp;<br> &nbsp;

   Lalu buat rute untuk artikel detail
   <br> &nbsp;
    |$routes->get('/artikel/(:any)', 'Artikel::view/$1');|
    |----|
   <br> &nbsp; <br> &nbsp;
   
   
   Fungsi dari **View()** & **detail.php** ini ketika judul artikel di klik maka akan memunculkan artikel tersebut saja, ini contohnya :
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/1bc0c4ad-923f-4c0c-8c96-e7c008bae25e)
    <br> &nbsp;
   Ketika judul artikel pertama di klik akan muncul artikel tersebut

9. Buat panel Admin, menu admin digunakan untuk CRUD data artikel. Buat metode nya baru pada **app/Controllers/artikel.php** dengan **admin_index()**
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/302950f1-b826-4a33-8ed3-82c776de9464)
     <br> &nbsp;

   Lalu buat view tampilan adminnya di direktori **app/Views/artikel** dengan nama **admin_index.php**
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/73201db0-de47-41de-9830-ce3d2c03172d)
    <br> &nbsp; <br> &nbsp;

   Tambahkan route baru untuk menu admin di direktori **app/config/Routers.php**
    <br> &nbsp;
   
   ![image](https://github.com/user-attachments/assets/7d901a65-68f6-4dd6-a144-19d707bc53cb)
    <br> &nbsp; <br> &nbsp;

   Lalu akses menu admin dengan url http://localhost:8080/admin/artikel/
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/e83fa7df-37ab-404e-bfc9-28b0c3a6d9a9)
    <br> &nbsp;<br> &nbsp;

10. Menambah data artikel, menambah fungsi baru di direktori **app/Controllers/artikel.php** dengan nama **add()**
    <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/2631c580-dfd5-46af-8723-36b99d0b258c)
    <br> &nbsp;<br> &nbsp;

    Kemudian buat view baru untuk menambah artikel di direktori **app/Views/artikel** dengan nama **form_add.php**
    <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/c5efe6ce-df3d-477d-943a-efefd950eaa6)
     <br> &nbsp; <br> &nbsp;

11. Menmbuat fungsi untuk mengubah data artikel di direktori **app/Controllers/artikel.php** dengan nama **edit()**
    <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/4fddab49-8900-4bcf-ab99-b28906ca0429)
    <br> &nbsp;<br> &nbsp;

    Lalu buat view untuk tampilan edit nya di direktori **app/Views/artikel** dengan nama **form_edit.php**
    <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/f1a375ea-9f8d-4b52-9ddc-3252bdf3f088)
     <br> &nbsp; <br> &nbsp;

    Maka tampilannya seperti ini
     <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/4c5b52f9-bb9a-404c-87af-f299dde885bc)
    <br> &nbsp;
    Fungsi nya untuk mengedit artikel yang sudah dibuat sebelumnya
    <br> &nbsp; <br> &nbsp;

13. Membuat fungsi hapus/delete di direktori **app/Controllers/artikel.php** dengan nama **delete()**
     <br> &nbsp;
    ![image](https://github.com/user-attachments/assets/c30d8bf1-64c5-4478-a81b-97d594d70f53)
     <br> &nbsp;
    Fungsinya untuk menghapus artikel dari table 
       <br> &nbsp; <br> &nbsp;


 
**================================================================================**

                                                                  Tugas 3

**================================================================================**

1. Buat folder **layout** di dalam **app/Views** dan buat file dengan nama **main.php** di dalam folder **layout** dengan kode berikut
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/ecaa2255-75db-47c2-baad-54f86315b159)
   <br> &nbsp;<br> &nbsp;
   ![image](https://github.com/user-attachments/assets/e6c98fc6-f0d2-4cc9-bcac-337a688a3189)
   <br> &nbsp;<br> &nbsp;

2. Buat file pada direktori **app/Views** dengan nama **home.php**
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/36190b12-8e8a-49fd-8b46-402d78d2191c)
   <br> &nbsp;<br> &nbsp;

3. Buat class view, buat folder baru di **app/** dengan nama **Cells**, buat file **ArtikelTerkini.php** di dalam **app/Cells**
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/434af6ad-2641-4700-8f4a-6e8d5501b4d3)
    <br> &nbsp;<br> &nbsp;

4. Buat folder **components** di dalam **app/Views**, dan buat file **artikel_terkini.php** di dalam direktori **app/Views/components**
   <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/bc041cbe-565d-4240-8a47-c41742b9cc81)
    <br> &nbsp; <br> &nbsp;

5. Hasilnya akan seperti ini
    <br> &nbsp;
   ![image](https://github.com/user-attachments/assets/7029fe3b-e8b0-4458-974a-d4cbf1566d88)
    <br> &nbsp;<br> &nbsp;
    

**================================================================================**

                                                                  Tugas & Pertanyaan

**================================================================================**

1. Apa manfaat utama dari penggunaan View Layout dalam pengembangan aplikasi?
   <br> &nbsp;
2. Jelaskan perbedaan antara View Cell dan View biasa.
   <br> &nbsp;
3. Ubah View Cell agar hanya menampilkan post dengan kategori tertentu..

   
<br> &nbsp;<br> &nbsp;



**================================================================================**

                                                                  Jawaban

**================================================================================**

  1. Dengan menggunakan View Layout, kode menjadi lebih modular, rapi, dan mudah dikelola, sehingga pengembangan aplikasi menjadi lebih cepat dan efisien.

  2. Gunakan view() untuk menampilkan halaman utama atau bagian besar dari aplikasi, Gunakan view_cell() jika ingin membuat komponen kecil yang bisa digunakan ulang di berbagai bagian aplikasi.

  3. 



    

   


   



   

   
   
     





    

    





