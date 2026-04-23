# simrs_mLite
Sistem Informasi Manajemen Rumah Sakit (SIMRS) 'mLite".  

mLITE adalah alternatif ringan dan aman untuk Sistem Informasi Kesehatan agar bisa dijalankan via Mobile / Browser. mLITE dibangun dari awal dengan berfokus pada kesederhanaan - programer pemula pun dapat membuat Module-Modul sendiri. Ini karena mLITE menerapkan sistem dan arsitektur aplikasi yang sangat mudah dalam bentuk Kerangka Kerja Mandiri (Independent Framework).

Oh iya, mLITE memiliki panduan pemasangan yang sangat mudah juga. Hanya perlu 1 langkah penyesuaian. Segera setelah anda menyalin file-file ke komputer / server dan pengaturan selesai, mLITE siap digunakan! Proses pemasangan bahkan tidak membutuhkan waktu sebanyak yang diperlukan untuk menyalin file-filenya ;-)

Panel kontrol dan tampilan default sepenuhnya responsif, yang membuatnya dapat diakses dari perangkat mobile apa pun, bahkan di ponsel, berkat kerangka kerja CSS yang digunakan - Bootstrap. Setiap modul dapat menyesuaikan dengan CSS nya sendiri.

Masih banyak fitur-fitur tersembunyi untuk kebutuhan pengembangan. Silahkan eksplore lebih dalam lagi!!

# Kebutuhan Sistem

Persyaratan sistem untuk mLITE sangat sederhana, sehingga setiap server modern sudah cukup. Berikut persyaratan minimal yang diperlukan

Apache 2.2+ dengan mod_rewrite atau Nginx
PHP versi 7.4 - 8.3+
MySQL atau MariaDB
Konfigurasi PHP harus memiliki ekstensi berikut:

dom
gd
mbstring
pdo
zip
cURL
Pemasangan
Pemasangan menggunakan composer.
Install composer di server/PC dan jalankan perintah composer untuk pemasangan paket utama dan independensi
$ composer create-project xampp/mlite-master
Buat folder uploads, tmp/ dan admin/tmp. Beberapa server mungkin memerlukan izin tambahan chmod 777 untuk direktori dan file tersebut.

Sesuaikan pengaturan di .env

Buat database baru di MySQL/MariaDB dan import file mlite.sql

Buka browser Anda dan navigasikan ke alamat tempat file mLITE berada.

Silahkan login dengan Username: admin dan Password: admin

Pemasangan Manual.

Ekstrak semua file dari paket terkompresi dan kemudian transfer ke direktori lokal atau server. Biasanya, file diunggah ke www, htdocs atau public_html.

Install composer di server/PC dan jalankan perintah composer untuk pemasangan independensi

$ composer install
Buat folder uploads, tmp/ dan admin/tmp. Beberapa server mungkin memerlukan izin tambahan chmod 777 untuk direktori dan file tersebut.

Sesuaikan pengaturan di .env

Buat database baru di MySQL/MariaDB dan import file mlite_db.sql (tambahkan sql-mode = '' pada my.cnf atau jalankan perintah berikut)

$ sed -i "/user=mysql/a sql-mode = ''" /etc/my.cnf
Buka browser Anda dan navigasikan ke alamat tempat file mLITE berada.

Silahkan login dengan Username: admin dan Password: admin
