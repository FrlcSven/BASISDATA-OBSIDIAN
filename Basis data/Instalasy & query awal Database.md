# instalasi mysql
## Menggunakan XAMPP

1. Buka Apk XAMPP
2. Kemudian klik start pada mysql seperti dibawah ini

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/xampp.png?raw=true)

3. Lalu klik shell pada bagian kanan seperti dibawah ini

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/xampp2.png?raw=true)

4. Sesudah itu ketik mysql -u root -p seperti di bawah ini

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/mysql.png?raw=true)

5. Selesai


## Refrensi Video dari Youtube

https://youtu.be/SWs0j2LzcD4?si=1PEEARq-F55bCQbX

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/tutor%20yt.png?raw=true)


# Penggunaan awal mysql
## Query
Perintah mysql -u root -p digunakan untuk masuk ke server MySQL dengan mengidentifikasi pengguna "root" dan meminta pengguna untuk memasukkan kata sandi. Mari bahas komponen-komponen perintah ini:

- mysql: Memulai klien command-line MySQL.
- -u root: Menentukan pengguna (user) yang ingin digunakan untuk login, dalam hal ini "root".
- -p: Menyiratkan bahwa sistem akan meminta kata sandi setelah menekan Enter.

Jadi, secara keseluruhan, perintah ini berfungsi untuk mengakses server MySQL sebagai pengguna "root" dan memastikan bahwa hanya pengguna yang memiliki kata sandi yang benar yang dapat mengakses dan berinteraksi dengan server MySQL tersebut.

## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/h%20query.png?raw=true)

## Analisis
Teks "mysql -u root -p" merupakan perintah baris perintah (command line) untuk mengakses server MySQL dengan menggunakan akun pengguna "root" dan meminta pengguna untuk memasukkan kata sandi ("-p" menunjukkan bahwa kata sandi akan dimasukkan setelah menekan Enter).

## Kesimpulan
Kesimpulannya, perintah ini bertujuan untuk masuk ke server MySQL sebagai pengguna "root" dengan mengidentifikasi diri melalui kata sandi yang diperlukan. Dalam konteks ini, pengguna harus memasukkan kata sandi setelah mengetik perintah ini untuk mendapatkan akses ke lingkungan MySQL dengan hak akses yang sesuai dengan pengguna "root".

# Database
## Buat Database
### query
Perintah 
```mysql
CREATE nma_DATABASE;
```

 nama_database digunakan untuk membuat basis data baru di server MySQL.

Contoh:

`CREATE DATABASE x1_rpl_1;

Fungsinya adalah membuat database dengan nama yang disebutkan setelah kata kunci CREATE DATABASE. Setelah dijalankan, database baru akan dibuat dan dapat digunakan untuk menyimpan tabel, data, dan objek basis data lainnya.
### Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/create%20database.png?raw=true)

### Analisis
Teks "`Created database`" ini menyatakan bahwa sebuah basis data telah dibuat. Dalam konteks pengelolaan basis data, ini mengindikasikan bahwa pengguna atau sistem telah berhasil membuat suatu basis data baru.

`CREATE DATABASE x1_rpl_1;

CREATE DATABASE adalah query untuk membuat database dan x1_rpl_1 adalah nama database nya.



### Kesimpulan
Kesimpulannya, pernyataan ini menunjukkan bahwa proses pembuatan basis data telah berhasil dilakukan. Selanjutnya, pengguna dapat menggunakan basis data tersebut untuk menyimpan dan mengelola data sesuai kebutuhan aplikasi atau proyek yang sedang dijalankan.

## Tampilkan Database
### Query
Perintah 
```mysql
SHOW DATABASES;
```

digunakan pada MySQL untuk menampilkan daftar semua basis data yang ada di server.

### Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/show%20database.png?raw=true)

### Analisis
Teks "`SHOW DATABASES;`" merupakan perintah SQL yang digunakan untuk menampilkan daftar semua basis data yang ada di server MySQL.
Fungsinya adalah memberikan informasi mengenai basis data yang tersedia di server MySQL. Ketika perintah ini dijalankan, server akan memberikan daftar nama basis data yang dapat diakses. Ini berguna untuk mengetahui basis data mana yang sudah ada dan tersedia untuk digunakan.

### Kesimpulan
Kesimpulannya, perintah ini digunakan untuk melihat semua basis data yang telah dibuat di server MySQL. Ketika perintah ini dijalankan, server akan merespons dengan menampilkan nama-nama basis data yang tersedia. Hal ini memudahkan pengguna untuk mengetahui basis data apa saja yang sudah ada dalam lingkungan MySQL yang sedang diakses.

## Hapus Database
### Query
Perintah 
```mysql
DROP nama_DATABASE
```

 digunakan pada MySQL untuk menghapus sebuah basis data beserta seluruh tabel, indeks, dan objek basis data lainnya yang terkait di dalamnya.

Contoh:

DROP x1_rpl_1

### Hasil
![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/drop%20database.png?raw=true)

### Analisis
Teks "DROP DATABASE" adalah perintah SQL yang digunakan untuk menghapus sebuah basis data beserta seluruh tabel dan data yang terkait di dalamnya.Fungsinya adalah untuk menghapus secara permanen sebuah basis data dari server MySQL. Harap berhati-hati saat menggunakan perintah ini, karena setelah dieksekusi, semua data yang terkait dengan basis data tersebut akan dihapus dan tidak dapat dikembalikan. Pastikan bahwa Anda yakin ingin menghapus basis data tersebut sebelum menjalankan perintah DROP DATABASE.

`DROP x1_rpl_1`

DROP adalah query untuk menghapus database dan x1_rpl_1 adalah database yang akan dihapus

### Kesimpulan
Kesimpulannya, perintah ini digunakan dengan hati-hati karena akan menghapus semua informasi yang terkandung dalam basis data yang ditentukan. Pengguna perlu memastikan bahwa mereka benar-benar ingin menghapus basis data tersebut sebelum menjalankan perintah ini, karena data yang dihapus tidak dapat dipulihkan.

## Gunakan Database
### Query
Perintah 
```mysql
`USE nama_DATABASE;
```

digunakan pada MySQL untuk beralih ke basis data tertentu, sehingga semua operasi yang dilakukan setelahnya akan berlaku pada basis data tersebut.

Contoh:

`USE farhan_xi;`

Fungsinya adalah mengubah basis data aktif yang digunakan dalam sesi koneksi MySQL. Setelah menjalankan perintah USE DATABASE, semua operasi seperti SELECT, INSERT, UPDATE, atau DELETE akan diterapkan pada tabel dalam basis data yang telah dipilih. Ini memungkinkan pengguna untuk fokus pada manipulasi data di dalam basis data tertentu tanpa harus menyertakan nama basis data secara eksplisit setiap saat.

### Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/use%20database.png?raw=true)

### Analisis
Teks "USE nama_DATABASE" adalah perintah SQL yang digunakan untuk beralih ke basis data tertentu. Basis data yang ditentukan akan menjadi basis data aktif untuk sesi koneksi saat itu.

`USE farhan_xi;`

USE adalah query untuk menggunakan database dan farhan_xi adalah database yang akan digunakan



### Kesimpulan
Kesimpulannya, perintah ini memungkinkan pengguna untuk berpindah antara basis data yang ada dalam server MySQL. Setelah menjalankan perintah "USE DATABASE", semua operasi database selanjutnya dalam sesi tersebut akan diterapkan pada basis data yang telah dipilih, hingga pengguna beralih ke basis data lain atau menutup sesi koneksi.

# Tipe Data
## Angka
Beberapa tipe data angka yang umum digunakan pada MySQL antara lain:

- DOUBLE: Mirip dengan FLOAT, tetapi dapat menyimpan nilai dengan presisi ganda.

- DECIMAL: Cocok untuk nilai desimal yang embutuhkan presisi tetap.

- Integer (Bilangan Bulat): Digunakan untuk menyimpan bilangan bulat tanpa desimal, seperti 1, -5, atau 100.

- Float (Bilangan Desimal): Untuk menyimpan angka dengan desimal, seperti 3.14 atau -0.5.

- Long (Bilangan Bulat Panjang): Digunakan untuk menyimpan bilangan bulat yang sangat besar.

- Complex (Bilangan Kompleks): Untuk menyimpan angka kompleks yang terdiri dari bagian real dan imajiner.

Dalam contoh ini, INTEGER, FLOAT, DOUBLE, dan DECIMAL adalah tipe data angka yang digunakan untuk kolom-kolom tertentu dalam tabel.

## Teks
Beberapa tipe data teks yang umum digunakan pada MySQL antara lain:

- String: Tipe data yang digunakan untuk menyimpan teks atau karakter. String diwakili oleh serangkaian karakter yang diapit oleh tanda kutip, baik itu tunggal (') atau ganda ("). Contoh: 'hello', "world", atau '123abc'.

- Char: Tipe data yang digunakan untuk menyimpan satu karakter. Char diwakili oleh tanda kutip tunggal (''). Contoh: 'a', 'b', atau '1'.

- CHAR: Menyimpan string dengan panjang tetap.

- VARCHAR: Menyimpan string dengan panjang variabel.

- TEXT: Cocok untuk menyimpan teks panjang, seperti paragraf atau dokumen.

Dalam contoh ini, CHAR, VARCHAR, dan TEXT adalah tipe data teks yang digunakan untuk kolom-kolom tertentu dalam tabel.

## Tanggal
Beberapa tipe data tanggal dan waktu yang umum digunakan pada MySQL antara lain:
  
- Date (Tanggal): Tipe data yang digunakan untuk merepresentasikan tanggal. Biasanya terdiri dari tahun, bulan, dan hari (YYYY-MM-DD). Beberapa bahasa pemrograman memiliki tipe data khusus untuk tanggal, misalnya datetime.date di Python.

- Datetime (Tanggal dan Waktu): Tipe data yang digunakan untuk merepresentasikan tanggal dan waktu. Selain tahun, bulan, dan hari, tipe data ini juga menyertakan informasi waktu seperti jam, menit, dan detik. Contoh: 2024-01-27 15:30:00. (YYYY-MM-DD HH:MM:SS.)

- TIME: Menyimpan waktu dengan format 15:30:00. (HH:MM:SS.)

- TIMESTAMP: Mirip dengan DATETIME, tetapi dengan rentang waktu yang lebih kecil dan terkait dengan zona waktu server.

- YEAR: Menyimpan tahun dengan empat digit. (YYYY)

Dalam contoh ini, DATE, TIME, DATETIME, TIMESTAMP, dan YEAR adalah tipe data yang digunakan untuk kolom-kolom tertentu dalam tabel untuk menyimpan informasi tanggal dan waktu.

## Boolean
- tipe data boolean digunakan untuk menyimpan nilai kebenaran, yaitu True (benar) atau False (salah). Tipe data boolean umumnya digunakan dalam kondisi percabangan dan pengambilan keputusan.


## Tipe Data Pilihan
### Enum
Tipe data ENUM (enumeration) dalam basis data adalah tipe data yang digunakan untuk mendefinisikan kumpulan nilai tetap yang dapat diidentifikasi oleh nama. Setiap nilai dalam ENUM diberi label dan harus dipilih dari daftar nilai yang telah ditentukan.

### Set
MySQL memiliki tipe data SET yang memungkinkan Anda untuk menyimpan himpunan nilai tetap yang telah ditentukan sebelumnya. Namun, penggunaannya harus dipertimbangkan dengan hati-hati karena dapat menyulitkan pengelolaan dan perubahan struktur data

# Tabel
## Buat Tabel
### Struktur

```mysql
create table nama_tabel(
    nama_kolom_1 tipe_data(max karakter) constraint,
    nama_kolom_2 tipe_data(max karakter) constraint,
    nama_kolom_3 tipe_data(max karakter),
    ...);
```
### Contoh


```mysql
create table biodata(
    nis_siswa int(8) primary key not null,
    nama_asli  varchar(25) not null,
    nama_panggilan varchar(25),
    no_telp char(12) unique);
```

## Tampilkan Struktur Tabel
### Hasil


![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/descibe%20tabel.png?raw=true)

### Analisis
Program di atas adalah perintah SQL untuk membuat tabel bernama                "**biodata**" dengan empat kolom. Berikut analisisnya:

1. Create table biodata
`CREATE TABEL` ADALAH query membuat tabel,`BIODATA` adalah nama tabelnya


2. nis_siswa int(8) primary key not null
`NIS_SISWA` adalah nama kolom Pertama, `int` adalah tipe datanya,(8) adalah max karakternya`primary key` adalah constraint kunci induk,`not null` adalah constraint data tidak boleh kosong.

3. nama_asli  varchar(25) not null
`nama_asli` adalah nama kolom Kedua, Varchar adalah tipedatanya,(25) adalah max karakternya,not null adalah adalah constraint data tidak boleh kosong.

4. nama_panggilan varchar(25)
`nama_panggilan` adalah  nama kolom Ketiga, `Varchar` adalah tipedata,`(25)` adalah max karakternya.

5. no_telp char(12) unique
`no_telp` adalah nama kolom Keempat, `Varchar` adalah tipedata,`(12)` adalah max karakternya, `unique` adalah constraint tidak ada data yang sama 

### kesimpulan
Kesimpulannya, tabel "**biodata"** ini dirancang untuk menyimpan informasi biodata siswa, dengan fokus pada nomor induk siswa (nis_siswa) sebagai kunci utama dan keterbatasan tertentu pada kolom nama_asli dan no_telp untuk memastikan integritas data.
## menampilkan daftar tabel

```
MariaDB [rental_farhan]> show tables;
+-------------------------+
| Tables_in_rental_farhan |
+-------------------------+
| biodata                 |
| pelanggan               |
+-------------------------+
```

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/tampilkan%20tabel.png?raw=true)

## Q & A

>[!Faq] Mengapa hanya kolom id_pelanggan yang menggunakan constraint PRIMARY KEY?
>= Jika kolom id_pelanggan menggunakan tipe data CHAR, mungkin karena panjang ID pelanggan selalu tetap, dan penggunaan CHAR dapat mengoptimalkan penyimpanan dalam situasi tersebut. Jika menggunakan VARCHAR, itu akan menyimpan panjang yang bervariasi dan membutuhkan sedikit lebih banyak ruang.

>[!Faq] mengapa pada kolom no_telepon yang menggunakan tipe data char bukan varchar?
>=Pemilihan antara tipe data CHAR dan VARCHAR untuk kolom no_telepon mungkin tergantung pada kebutuhan dan preferensi desain basis data. Jika panjang nomor telepon selalu tetap dan memiliki panjang yang konsisten, menggunakan CHAR bisa menjadi pilihan yang efisien karena menyimpan data dengan panjang tetap.

>[!Faq] Mengapa hanya kolom no_telepon yang menggunakan constraint UNIQUE?
>Pemberian constraint UNIQUE pada kolom no_telepon bertujuan untuk memastikan bahwa setiap nomor telepon yang dimasukkan ke dalam basis data adalah unik. Hal ini dapat membantu mencegah duplikasi nomor telepon yang dapat menyebabkan masalah seperti kesulitan dalam mengidentifikasi dan mengelola data.


>[!Faq] Mengapa kolom no_telepon tidak memakai constraint NOT NULL, sementara kolom lainnya menggunakan constraint tersebut?
>Pemberian constraint NOT NULL pada suatu kolom menunjukkan bahwa nilai dalam kolom tersebut tidak boleh kosong (NULL).

>[!Faq] Perbedaan PK dan UNIQUE?
>primary key digunakan untuk mengidentifikasi unik suatu baris dan sering kali menjadi dasar untuk hubungan antar-tabel, sementara unique constraint digunakan untuk memastikan bahwa suatu kolom memiliki nilai yang unik tetapi tidak selalu terkait dengan identifikasi unik baris.

   


# Insert
## Insert 1 data
### Struktur

```mysql
insert into nama_table
     values ('nilai1','nilai2','nilai3','nilai4');
```
### Contoh
```mysql
insert into pelanggan
     values (1,'farhan','mln','088247291854');
```


### Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/contoh%20buat%20insert.png?raw=true)

### Analisis

1. `insert into pelanggan;` :
`insert into` merupakan sebuah query untuk menambahkan data baru ke dalam sebuah tabel di database `pelanggan` adalah nama tabelnya

2.  `values (1,'farhan','mln','088247291854');` :
`values` digunakan untuk menyediakan nilai nilai yang akan dimasukkan ke dalam sebuah tabel.

- Angka `1` akan dimasukkan ke dalam kolom pertama
- String `'farhan'` akan dimasukkan ke dalam kolom kedua.
- String `'mln'` akan dimasukkan ke dalam kolom ketiga.
- String `'088247291854'` akan dimasukkan ke dalam kolom keempat.
### Kesimpulan

kesimpulannya adalah perintah ini akan menambahkan satu baris data baru ke dalam tabel "pelanggan" dengan nilai-nilai yang sesuai yang telah ditentukan.
## insert >1 data
### struktur

```mysql
insert into nama_table
     values ('nilai1','nilai2','nilai3','nilai4'),
     ('nilai1','nilai2''nilai3','nilai4'),
     ('nilai1','nilai2','nilai3','nilai4');
```
### Contoh

 ``` mysql
 insert into pelanggan
     values (2,'rehan','alfa','087868449445'),
     (3,'ardy','rd','0895333405548'),
     (4,'ilham','vp','087733345678');
```


### Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/tabel%20%20lebih%20dari%201.png?raw=true)


### Analisis


1. insert into pelanggan :
`insert into` merupakan sebuah query untuk menambahkan data baru ke dalam sebuah tabel di database `pelanggan` adalah nama tabelnya

2. values (2,'rehan','alfa','087868449445'),
         (3,'ardy','rd','0895333405548'),
         (4,'ilham','vp','087733345678'); :

`values` digunakan untuk menyediakan nilai nilai yang akan dimasukkan ke dalam sebuah tabel.

- Angka `2,3,4`adalah baris yang akan dimasukkan ke dalam kolom pertama
- String `'rehan','ardy','ilham'` akan dimasukkan ke dalam kolom kedua dan sesuai dengan barisnya.
- String `'alfa','rd','vp'` akan dimasukkan ke dalam kolom ketiga dan sesuai dengan barisnya.
- String `'087868449445','0895333405548','087733345678'` akan dimasukkan ke dalam kolom keempat dan sesuai dengan barisnya.

### Kesimpulan

Kesimpulannya, perintah ini akan menambahkan tiga baris data baru ke dalam tabel "pelanggan" dengan nilai-nilai yang sesuai untuk setiap baris yang disediakan.
## Menyebut Kolom
### Struktur

```mysql
insert into nama_table
    (kolom1,kolom2) values (nilai1,nilai2)
```

### Contoh

```mysql
 insert into pelanggan
     (nama_depan,id_pelanggan) values ('radit',5);
```


## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/menyebut%20kolom5.png?raw=true)

## Analisis

1. `insert into pelanggan;` :
`insert into` merupakan sebuah query untuk menambahkan data baru ke dalam sebuah tabel di database `pelanggan` adalah nama tabelnya

2. `(nama_depan,id_pelanggan) values ('radit',5);`:

- Tabel yang dituju adalah "pelanggan".
- Data yang akan dimasukkan ke dalam tabel adalah nama depan "radit" dan ID pelanggan 5.

`(nama_depan,id_pelanggan)` sebelum klausa `VALUES`. Ini menunjukkan bahwa hanya kolom-kolom yang ditentukan (yaitu `nama_depan` dan `id_pelanggan`) yang akan menerima nilai, sedangkan kolom-kolom lainnya akan memiliki nilai default (jika ada) atau NULL.


## Kesimpulan

Kesimpulannya, perintah ini akan menambahkan satu baris data baru ke dalam tabel "pelanggan" dengan nilai nama depan "radit" dan ID pelanggan 5, sementara kolom-kolom lainnya mungkin akan memiliki nilai default atau NULL,

# Select
## Seluruh Data
### Struktur

```mysql
select * from nama_tabel;
```
### Contoh

```mysql
select * from pelanggan;
```

## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/select%20seluruh%20data.png?raw=true)

## Analisis

`select * from pelanggan;`:

Perintah `SELECT * from pelanggan` adalah pernyataan dalam SQL yang digunakan untuk memilih semua kolom dari sebuah tabel.

## Kesimpulan


Kesimpulannya,Perintah SELECT * FROM pelanggan; memberikan gambaran keseluruhan tentang data yang tersimpan dalam tabel "pelanggan" pada saat perintah tersebut dijalankan.
## Data kolom tertentu
### Struktur

```mysql
select nama_kolom1,nama_kolom2,nama_kolom_n from nama_table;
```

### Contoh

```mysql
select nama_depan from pelanggan;
```

## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/select%20data%20tertentu.png?raw=true)
## Analisis

`select nama_depan from pelanggan;`:
Perintah ini akan mengembalikan nilai dari kolom "nama_depan" untuk setiap baris data yang ada dalam tabel "pelanggan".

## Kesimpulan

Kesimpulan:
Dengan menggunakan perintah `SELECT nama_depan FROM pelanggan;`, Anda meminta sistem database untuk mengembalikan atau menampilkan hanya kolom "nama_depan" dari tabel "pelanggan".

## Klausa WHERE

### Struktur

```mysql
select nama_kolom / * from nama_table
where kondisi;
```

### Contoh

```mysql
select * from pelanggan
    where id_pelanggan=2;
```

## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/klausa%20where%201.png?raw=true)
## Analisis

`select * from pelanggan where id_pelanggan=2;`:
Perintah ini akan mengembalikan semua kolom untuk baris data yang memenuhi kondisi di mana nilai kolom "id_pelanggan" adalah 2.
`

## Kesimpulan

Kesimpulan:
Dengan menggunakan perintah ini, Anda meminta sistem database untuk mengembalikan atau menampilkan semua informasi yang tersedia untuk pelanggan dengan ID 2 dari tabel "pelanggan

# Update (Perbarui Data)
## struktur

```mysql
update nama_tabel set nama_kolom="nilai" where kondisi;
```
## contoh

```mysql
update pelanggan set no_telp="085657199460" where id_pelanggan="4";
```

## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/update%20no%20telp.png?raw=true)
## Analisis

`update pelanggan set no_telp="085657199460" where id_pelanggan="4";` :
- Perintah ini akan mengubah nilai kolom `"no_telp"` menjadi `"085657199460"` untuk baris data yang memenuhi kondisi di mana nilai kolom `"id_pelanggan"` adalah 4.
- Perintah ini hanya memengaruhi satu baris data yang memenuhi kondisi tersebut.
## Kesimpulan

Kesimpulan:
Dengan menggunakan perintah UPDATE, Anda dapat memperbarui nilai dari satu atau beberapa kolom untuk baris data tertentu dalam tabel. Dalam hal ini, nomor telepon ("no_telp") untuk pelanggan dengan ID 4 akan diperbarui menjadi "085657199460"

# Delete (Hapus Baris Data)
## Struktur 

```mysql
delete from nama_table where kondisi;
```

## Contoh
```mysql
delete from pelanggan where id_pelanggan="3";
```


## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/hapus%20baris%20data.png?raw=true)
## Analisis

`delete from pelanggan where id_pelanggan="3";`:
- Perintah ini akan menghapus satu baris data dari tabel "pelanggan" yang memiliki nilai kolom "id_pelanggan" sama dengan 3.
- Setelah perintah ini dijalankan, baris data tersebut akan dihapus dari tabel "pelanggan".


## Kesimpulan

Kesimpulan:
Dengan menggunakan perintah DELETE FROM, Anda dapat menghapus baris data yang memenuhi kondisi tertentu dari tabel. Dalam hal ini, baris data yang memiliki nilai "id_pelanggan" sama dengan 3 akan dihapus dari tabel "pelanggan".

# Hapus Tabel
## struktur

```mysql
drop table nama_tabel;
```
## Contoh

```mysql
drop table biodata;
```

## Hasil

![alt text](https://github.com/FrlcSven/BASISDATA-OBSIDIAN/blob/main/ASET%20BASIS%20DATA/hapus%20tabel.png?raw=true)
## Analisis 

`drop table biodata;`:
- Perintah ini akan menghapus seluruh struktur tabel, termasuk semua data dan indeks yang terkait, dari database.
- Setelah perintah ini dijalankan, tabel "biodata" beserta semua informasi yang terkait dengannya akan dihapus dari database
## Kesimpulan

Kesimpulan:
Dengan menggunakan perintah DROP TABLE, Anda dapat menghapus tabel secara permanen dari database. 



