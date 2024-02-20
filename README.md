## Alur Sistem Aplikasi Siakad Terintegrasi
### Versi: 2.0.0-NeoSync

### 1. Mahasiswa:
-  :computer: Mahasiswa membuka halaman login sistem informasi kampus ( U )
-  :key: Mahasiswa memasukkan username dan password yang valid ( U )
-  :closed_lock_with_key: Mahasiswa dapat mengganti password.
-  :house_with_garden: Pada halaman utama, mahasiswa memiliki beberapa opsi:
    -  :page_with_curl: Mahasiswa dapat "KRS Online" berdasarkan semester terbuka dan prodi.
    -  :mag: Sistem menampilkan daftar mata kuliah yang tersedia beserta informasi terkait (U).
    -  :pencil2: Mahasiswa memilih mata kuliah yang ingin diambil dan menentukan jumlah sks yang akan diambil. (U)
    -  :arrows_counterclockwise: Sistem Cache Untuk KRS agar mempercepat loading ( U )
    -  :floppy_disk: Setelah selesai memilih mata kuliah, mahasiswa mengkonfirmasi pilihan dan menyimpan KRS. (U)
    -  :white_check_mark: Sistem melakukan validasi terhadap pilihan mata kuliah yang diambil.
    -  :floppy_disk: Jika valid, KRS mahasiswa akan tersimpan dalam sistem (U)
    -  :bar_chart: Mahasiswa juga dapat memilih menu "Lihat Nilai Semester (KHS)".
    -  :scroll: Sistem menampilkan nilai-nilai yang telah diperoleh mahasiswa pada semester tersebut.
    -  :scroll: Mahasiswa juga dapat memilih menu "Lihat Transkrip Nilai".
    -  :x: Mahasiswa tidak bisa login jika dari keuangan tidak mengaktifkan
    -  :bust_in_silhouette: Profile Mahasiswa
-  :money_with_wings: Melakukan pembayaran aktif mahasiswa dari siakad dengan VA Bank yang sudah ditentukan oleh keuangan
-  :receipt: Mahasiswa dapat melihat riwayat pembayaran uang kuliah yg telah dibayarkan
-  :unlock: Mahasiswa Bisa Login KRS Online jika sudah melakukan pembayaran
-  :arrows_counterclockwise: Mahasiswa Dapat melakukan perubahan KRS dengan persetujuan PA
-  :mortar_board: Pada KRS Mahasiswa tampilkan nama dosen pengajar

### 2. Dosen:
-  :computer: Dosen login ke sistem informasi kampus menggunakan username dan password yang valid (U) WAJIB MENGGUNAKAN NIDN / NIDK
-  :key: Dosen Dapat Ganti password
-  :date: Dosen Melihat Kelas Perkuliahan yang diampu berdasarkan semester
-  :memo: Dosen memilih menu "Masuk Kelas"
-  :pencil2: Masuk kelas Dengan Memilih Input Nilai
-  :pencil2: Dosen memasukkan nilai untuk setiap mahasiswa berdasarkan kriteria penilaian yang telah ditentukan.
-  :floppy_disk: Setelah selesai memberikan penilaian, dosen menyimpan data nilai.
-  :white_check_mark: Sistem melakukan validasi terhadap nilai yang dimasukkan.
-  :floppy_disk: Jika valid, data nilai akan tersimpan dalam sistem.
-  :bust_in_silhouette: Profile Dosen
-  :mortar_board: Dosen PA dapat melihat KRS Mahasiswa yang sudah mengambil KRS Online
-  :mortar_board: Dosen PA dapat menyetujui perubahan KRS Mahasiswa

### 3. Bagian Akademik (BAAK)
-  :computer: Bagian akademik login ke sistem informasi kampus menggunakan username dan password yang valid. ( U )
-  :bookmark_tabs: Input Mata Kuliah Aktif berdasarkan Prodi ( U )
-  :pencil2: Bagian akademik dapat menggunakan fitur "Input Kelas Kuliah" untuk setiap prodi . ( U )
-  :clock1: Dapat Input Jadwal Kuliah Berdasarkan Kelas
-  :busts_in_silhouette: Input Dosen Pengajar Setiap Kelas Kuliah (U)
-  :busts_in_silhouette: Input Dosen Pembimbing Akademik mahasiswa pada data mahasiswa (U)
-  :date: Melakukan Set Tahun Semester Berjalan otomatis berdasarkan inputan terakhir kelas perkuliahan. ( Sudah ) (U)
-  :card_index_dividers: Mengelola Data Dosen (U)
-  :key: Setiap data dosen yang dibuat langsung mendapatkan username dan password login, dengan akses nidn dan nidn
-  :card_index_dividers: Mengelola Data Mahasiswa dapat berdasarkan prodi, tahun masuk dan dosen pembimbing (U)
-  :busts_in_silhouette: Setiap mahasiswa baru yang di input langsung mendapatkan akun login dengan default login username nim dan password nim ( U )
-  :printer: Proses Cetak KRS
-  :printer: Proses Cetak KHS
-  :memo: Absensi ( Peserta KRS ) Berdasarkan kelas perkuliahan
-  :closed_lock_with_key: Ganti password
-  :x: Jika kelas tidak dalam periode pembukaan maka tidak dapat lagi di edit
-  :unlock: Buka Tutup KRS mahasiswa Online
-  :unlock: Buka Tutup KHS Dosen penilaian
-  :chart_with_upwards_trend: Dapat membatasi kuota setiap kelas
-  :arrows_counterclockwise: Dapat merubah KRS mahasiswa yang sudah disetujui oleh PA
-  :heavy_check_mark: Validasi Data Mahasiswa baru dari data PMB

### 4. Prodi
-  :computer: Prodi Dapat Login
-  :busts_in_silhouette: Menampilkan data dosen yang sudah melakukan input nilai
-  :memo: Masing masing prodi validasi nilai dari dosen.
-  :bar_chart: Rekap KRS Online mahasiswa yang sudah dan Belum
-  :bar_chart: Sistem melakukan validasi nilai (KHS) mahasiswa berdasarkan data yang telah diinput oleh dosen.
-  :closed_lock_with_key: Ganti password
-  :bar_chart: Prodi dapat akses untuk melihat mahasiswa yg aktif dan nonaktif jumlah mahasiswa per angkatan dan keseluruhan
-  :printer: Prodi diberikan akses untuk cetak form absensi dan jurnal perkuliahan berdasarkan data kelas yang sudah diisi oleh mahasiswa

### 5. Calon Maba (Penerimaan Mahasiswa Baru)
1. :money_with_wings: Terlebih dahulu mahasiswa melakukan pembayaran uang pendaftaran ke BAAK atau bank yang sudah ditentukan.
2. :page_with_curl: Selanjutnya, mahasiswa mengisi formulir yang ada pada link formulir pendaftaran mahasiswa baru.
3. :email: Setelah divalidasi, mahasiswa akan menerima bukti pendaftaran sekaligus berfungsi sebagai tanda peserta untuk mengikuti tes masuk ITB Indragiri melalui email yang diinput sebelumnya di formulir pendaftaran, dan diberikan pemberitahuan untuk mengikuti tes calon mahasiswa baru.
4. :white_check_mark: Jika calon mahasiswa baru dinyatakan lulus, maka mahasiswa tersebut diwajibkan melakukan pendaftaran ulang dengan melengkapi berkas pendaftaran.
5. :id: Kemudian, mahasiswa akan diberikan Nomor Induk Mahasiswa (NIM) dan Akun SIAKAD.
6. :pencil2: Setelah itu, mahasiswa diwajibkan untuk mengisi KRS sesuai dengan lokal yang sudah ditentukan.

Saya telah menambahkan emoji untuk mewakili setiap langkah dalam proses penerimaan mahasiswa baru. Semoga ini membuatnya lebih menarik!

### 6. Admin
-  :card_file_box: Data Perguruan Tinggi ( U )
-  :card_file_box: Data Program Studi ( U )
-  :card_file_box: Data Login Semua User ( U )
-  :key: Ganti password
-  :repeat: Auto Login Semua Akses

### 7. BAUK ( Keuangan )
-  :computer: Login Ke Siakad
-  :lock: Dapat melakukan lock (kunci) thd mahasiswa yg masih menunggak utk tidak dapat melihat nilai masing" setelah membayar baru bisa.
-  :money_with_wings: Pengaturan pembayaran SKS Mahasiswa kelas reguler dan non reg
-  :memo: Edit Kelas mahasiswa reguler dan Non Reguler
-  :key: Ganti password
-  :money_with_wings: Bisa Set Pembayaran Setiap NIM berbeda
-  :inbox_tray: Import Dari Excel pembayaran Setiap NIM
-  :closed_lock_with_key: Ketika data pembayaran di import , mahasiswa tersebut langsung tidak bisa login
-  :information_source: Ada Keterangan Pembayaran di Import Data Pembayaran Mahasiswa
-  :heavy_check_mark: Validasi Pembayaran Manual
-  :arrows_counterclockwise: Ketika import data baru pembayaran , data lama langsung jadi arsip
-  :yen: Set Keuangan Pembayaran manual atau payment gateway

### 8. Operator PDDIKTI
-  :computer: Login Operator
-  :computer: Login NEO
-  :arrows_counterclockwise: Sistem memungkinkan bagian akademik untuk melakukan sinkronisasi data nilai dengan sistem Neo Feeder yang digunakan untuk pengelolaan data akademik secara lebih luas.
  - Mahasiswa Baru
  - Kelas Perkulihan
  - Dosen Ajar
  - KRS Online
  - KHS Online
  - Pembimbing Akademik ( Aktivitas Mahasiswa Berdasarkan SK )
