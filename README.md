MongoDB Compass
------------------------------------------------
Langkah 1) Lakukan koneksi ke MongoDB menggunakan connection string
<img src="1.jpg">

Langkah 2) Buat database dengan melakukan klik “Create Database”
<img src="2.jpg">

Langkah 3&4) Lakukan insert buku pertama dan kedua dengan melakukan klik “Add Data”, pilih “Insert
Document”,
isi dengan data yang diinginkan dan klik “Insert”
<img src="3.jpg">
<img src="4.jpg">
<img src="5.jpg">
<img src="6.jpg">

Langkah 5) Lakukan Pencarian Buku dengan Author“Osamu Dazai”dengan mengisi filter
yang diinginkan dan klik“find”
<img src="7.jpg">

Langkah 6) Lakukan perubahan summary pada buku “No Longer Human” menjadi “Buku
yang bagus (<NAMA>,<NIM>) dengan melakukan klik “Edit Document”
(berlambang pensil), mengisi nilai summary yang baru, dan melakukan klik
“Update”
<img src="8.jpg">

Langkah 7) Lakukan penghapusan pada buku “I Am a Cat” dengan melakukan klik
“Remove Document” (berlambang tong sampah) dan melakukan klik “Delete”
<img src="9.jpg">
<img src="10.jpg">


MongoDB SHELL
------------------------------------------------
Langkah 1) Lakukan koneksi ke MongoDB server dengan menjalankan command mongosh bagi yang
menggunakan terminal build in OS sehingga tampilan terminal kalian menjadi seperti
berikut.
<img src="11.jpg">

Langkah 2) Mencoba melihat list database yang ada di server dengan menjalankan command show
dbs
Untuk berpindah ke database “bookstore” gunakan command use bookstore , kalian
dapatmemastikan telah berpindah ke database yang benar dengan melihat tulisan sebelum
tanda “>”
<img src="12.jpg">

Langkah 3) Lakukan insert buku “Overlord I” dengan menggunakan command
db.books.insertOne(<data kalian>) , setelah insert buku berhasil maka MongoDB akan
mengembalikan pesan sebagai berikut.
<img src="13.jpg">

Langkah 4) Lakukan insert buku “The Setting Sun” dan “Hujan” dengan insert many dengan
menggunakan command db.books.insertMany(<data kalian>) , dan akan mengembalikan
pesan seperti pada modul
<img src="14.jpg">

Langkah 5) Lakukan pencarian buku dengan menggunakan command db.books.find() untuk
melakukan pencarian semua buku.
<img src="15.jpg">

Langkah 6) Tampilkan seluruh buku dengan author “Osamu Dazai” dengan mengisi argument pada
find() dengan menggunakan command db.books.find({<filter yang ingin diisi>})
<img src="16.jpg">

Langkah 7) Lakukan perubahan summary pada buku “Hujan” menjadi “Buku yang bagus
(<NAMA>,<NIM>) dengan mengunakan command db.books.updateOne({<filter>},
{$set: {<data yang akan di update>}}) sehingga output yang dihasilkan oleh MongoDB
akan menjadi seperti pada modul
<img src="17.jpg">

Langkah 8) Lakukan perubahan publisher menjadi “Yen Press” pada semua buku “Osamu Dazai”
dengan menggunakan command db.books.updateMany({<filter>}, {$set: {<data yang
akan di update>}})
<img src="18.jpg">

Langkah 9) Lakukan penghapusan pada buku “Overlord I” dengan menggunakan command
db.books.deleteOne({<argument>})
<img src="19.jpg">

Langkah 10) Lakukan penghapusan pada semua buku “Osamu Dazai dengan menggunakan
command db.books.deleteMany({<argument>})
<img src="20.jpg">
