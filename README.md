# Tugas-9 
## Menjalankan akses Create, select, Insert, delete, Privillage dan Drop pada CMD

1. Pertama kita buka CMD dan jalankan perintah 

* cd ../..
* cd xampp/mysql/bin
* mysql -u root

**Perintah ini unruk masuk ke root dari pada mysql**

![1](https://user-images.githubusercontent.com/46746119/123499872-95f92d00-d5ee-11eb-8ee7-e0619262663c.png)

---

2. Setelah masuk ke root mysql, selanjutnya memasukan perintah **create** *(yaitu membuat database)*

* setelah membuat database, bisa kita tampilkan database yang telah kita buat dengan memasukan perintah ***show databases;***

![2](https://user-images.githubusercontent.com/46746119/123499873-9691c380-d5ee-11eb-8c9f-e58287c64738.png)

---

3. Setelah membuat database, masukan perintah ***use (nama database);***

* selanjutnya create table didalam database yang sudah dipilih seperti gambar di bawah ini

![3](https://user-images.githubusercontent.com/46746119/123499857-88dc3e00-d5ee-11eb-9b47-959caf592f17.png)

---

4. Setelah itu masukan perintah ***Insert*** untuk mengedit data entri pada table seperti dibawah ini

![4](https://user-images.githubusercontent.com/46746119/123499859-8b3e9800-d5ee-11eb-9b40-35ba20bfdb6b.png)

---

5. Setelah membuat table pada database, selanjutnya kita akan memberikan user pada table yang kita buat

* Contohnya dibawah ini

![5](https://user-images.githubusercontent.com/46746119/123499860-8c6fc500-d5ee-11eb-9963-738d2cccca59.png)

---

6. Setelah membuat user, kita masukan perintah ***show grants for (nama user)*** untuk melihat **user** yang telah dibuat

![6](https://user-images.githubusercontent.com/46746119/123499862-91347900-d5ee-11eb-9c0e-f5fe2089b345.png)

---

7. Setelah itu masukan perintah untuk membuat akses database : grant create, select on (nama table).* (nama user); 

![7](https://user-images.githubusercontent.com/46746119/123499864-9265a600-d5ee-11eb-9066-2747b89b7ead.png)

---

8. Setelah membuat user, selanjutnya exit 

* dan masukan perintah ***mysql -u (nama user) -p*** untuk masuk ke database menggunakan password

![8](https://user-images.githubusercontent.com/46746119/123499865-92fe3c80-d5ee-11eb-8d8a-3b6992a379eb.png)

---

9. Selanjutnya kita coba tampilkan database yang sebelumnya kita buat

![9](https://user-images.githubusercontent.com/46746119/123499866-9396d300-d5ee-11eb-92e8-d7f2dedfb372.png)

---

10. setelah berhasil membuat akses pada database lalu kita exit

* selanjutnya masukan perintah ***revoke all privillege*** pada table dalam user untuk menghapus hak kusus
* kemudian exit

![10](https://user-images.githubusercontent.com/46746119/123499867-942f6980-d5ee-11eb-98f5-9ddd00c3ed27.png)

---

11. setelah itu kita masuk lagi ke ***mysql -u (nama user) -p***

* dan masuk kan perinta ***use (table);*** untuk masuk ke table
* dan jika muncul error, berarti hak akses sudah berhasil kita hapus

![11](https://user-images.githubusercontent.com/46746119/123499869-94c80000-d5ee-11eb-9604-9fd9dcc0491b.png)

---

12. Terakhir kita masukan perintah ***drop user (nama user@localhost);*** untuk menghapus user agar kita bisa membuka table kembali

* sebelum kita masukan perintah **drop** kita masuk sebagai root terlebih dahulu

![12](https://user-images.githubusercontent.com/46746119/123499870-95609680-d5ee-11eb-8582-7c28aae6a28d.png)

---

### selesai
