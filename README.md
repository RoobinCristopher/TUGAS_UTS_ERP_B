**Nama: Roobin Cristopher**

**NIM: 12030122120052**

**Mata Kuliah: ERP - B**

Tugas ini disusun untuk menunjukkan pemahaman dan kemampuan dalam menggunakan tools ERP System, serta sebagai bagian dari penilaian Ujian Tengah Semester (UTS) Mata Kuliah Enterprise Resource Planning (ERP) yang diampu oleh Bapak Dr. Totok Dewayanto, S.E., M.Si., Akt.

# **Tampilan _WEB_ dan Penjelasan Setiap Bagian _WEB_**
**1. Halaman Dashboard**
      **Fungsi Utama:** Menyajikan ringkasan operasional secara cepat untuk pemilik/manager: total penjualan, total pembelian, jumlah pelanggan, nilai persediaan, notifikasi          stok rendah, grafik tren penjualan.
      **Komponen:**
      Pada bagian atas terdapat menu:
        - Total Penjualan Hari Ini;
        - Total Produk;
        - Total Pelanggan; dan 
        - Informasi Stock Rendah.
        - Pada bagian tengah terdapat menu:
        - Grafik Penjualan 7 Hari Terakhir, berisikan Pergerakan penjualan harian dalam seminggu.
        - Aksi Cepat, Akses cepat ke fitur-fitur utama seperti Tambah Penjualan Baru, Tambah Produk Baru, Tambah Pelanggan Baru, dan menu untuk bisa langsung melihat Laporan.
    **Catatan Penggunaan:** Dashboard bersifat read-only (umumnya) atau dalam kata lain tampilan ringkasan dari setiap komponen yang berisikan informasi-informasi umum, dari        sini pengguna diarahkan ke halaman detail untuk aksi.
    <img width="1919" height="1074" alt="Screenshot 2025-10-21 153349" src="https://github.com/user-attachments/assets/ec3f70e0-dd18-4ef5-82fd-b3abb341d6d8" />
    <img width="1918" height="1072" alt="Screenshot 2025-10-21 153436" src="https://github.com/user-attachments/assets/0b9aff49-e35b-4d3b-907f-400d46647e86" />

**2. Halaman Produk**
      **Fungsi Utama:** Menyimpan master data produk/jasa yang dijual atau dibeli: kode, nama, kategori, unit ukuran, harga jual, harga beli, stok awal, minimal stok.
      **Komponen:** 
        1. Tabel daftar produk dengan kolom: Kode, Nama, Kategori, Harga Jual, Harga Beli, Stok, Aksi (Edit/Hapus/Detail).
        2. Tombol “Tambah Produk” / “Add New”.
        3. Form input produk (pop-up atau halaman terpisah): fields untuk Kode, Nama, Deskripsi, Kategori, Satuan, Harga, Pajak, Gambar produk, Variasi (ukuran/warna).
        4. Fitur pencarian dan filter: berdasarkan kategori, status stok, rentang harga.
      **Catatan Penggunaan:** 
        1. Kode produk idealnya unik; sistem biasanya menolak jika ada duplikasi.
        2. Jika pakai variant, pastikan tiap varian punya SKU tersendiri.
        3. Menyetel minimal stok membantu notifikasi stok menipis.
    <img width="1919" height="1068" alt="Screenshot 2025-10-21 153606" src="https://github.com/user-attachments/assets/5dd4a9e4-6599-4f46-88f0-99d839c2ed75" />
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 153737" src="https://github.com/user-attachments/assets/95951d11-ce39-4983-a3c3-3349518554d3" />

**3. Halaman Pelanggan**
      **Fungsi Utama:**  Menyimpan data pelanggan untuk mempermudah pembuatan penjualan, laporan piutang, dan personalisasi.
      **Komponen:** 
        1. Tabel pelanggan (Nama, Tipe: retail/corporate, Kontak, Email, Alamat, Saldo/piutang).
        2. Tombol tambah/edit customer, form data pelanggan.
        3. Riwayat transaksi pelanggan (invoice, pembayaran, retur).
        4. Label/tagging pelanggan (VIP, distributor, grosir) untuk segmentasi.
      **Catatan Penggunaan:** Validasi email/telepon dapat ditambahkan untuk kualitas data.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 153949" src="https://github.com/user-attachments/assets/852e5680-a376-40a4-b937-28d05afe9832" />
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 154048" src="https://github.com/user-attachments/assets/7ffad542-1b86-4e92-9a14-1d3ceca00434" />

**4. Halaman Penjualan**
      **Fungsi Utama:** Membuat transaksi penjualan (order/invoice), mengelola pembayaran, mencetak/menyimpan invoice, dan otomatis mengurangi stok.
      **Komponen:** 
        1. Daftar invoice/transaksi dengan status (Draft, Paid, Unpaid, Canceled).
        2. Form pembuatan transaksi: pilih pelanggan, tambahkan produk (qty, diskon, pajak), pilih metode pembayaran, input catatan.
        3. Ringkasan order: subtotal, diskon, pajak, total.
        4. Tombol aksi: Simpan sebagai Draft, Simpan & Kirim (email), Print Invoice, Mark as Paid, Create Credit Note / Retur.
        5. Metode pembayaran & catatan pembayaran: tunai, transfer, kartu; tanggal & bukti pembayaran.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 154129" src="https://github.com/user-attachments/assets/bfe32e48-f90a-4cc0-802f-fa050b7309bc" />

**5. Halaman Pembelian**
      **Fungsi Utama:** Mencatat pembelian dari supplier, membuat PO, menerima barang (goods receipt), dan menambah stok.
      **Komponen:**
        1. Daftar Purchase Order & status (Open, Received, Partially Received, Closed).
        2. Form PO: pilih supplier, barang, qty, harga beli, estimasi tiba.
        3. Goods Receipt: proses penerimaan barang yang dapat mengubah stok sesaat setelah diterima.
        4. Pengelolaan invoice supplier: mencatat tagihan supplier, pembayaran hutang.
        5. Aksi: Print PO, Kirim PO ke supplier, Terima Barang, Buat Faktur Pembelian.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 154230" src="https://github.com/user-attachments/assets/0738da6a-ac5c-403b-9767-7a0d82a8adf8" />

**6. Halaman Inventory**
      **Fungsi Utama:** Monitoring stok, mutasi barang (in/out), penyesuaian stok (stock opname), pengaturan lokasi gudang.
      **Komponen:**
        1. Daftar stok per produk dan per lokasi gudang.
        2. Filter lokasi/gudang dan kategori.
        3. Fitur Stock Opname: record hasil pengecekan fisik dan buat penyesuaian.
        4. Mutasi stok: transfer antar gudang, stok masuk (purchase receipt), stok keluar (sales dispatch).
        5. Laporan kunci: stok minimum, stok slow-moving, top-selling items.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 154335" src="https://github.com/user-attachments/assets/472a9973-7a67-4fb2-8045-72a8663ac924" />

**7. Halaman Laporan**
      **Fungsi Utama:** Menyediakan laporan analitis dan operasional: penjualan, pembelian, laba rugi sederhana, stok, piutang & hutang, arus kas ringkas.
      **Komponen:**
        1. Filter tanggal, customer, produk, kategori, lokasi gudang.
        2. Preview laporan, opsi ekspor (Excel, PDF, CSV).
        3. Grafik dan tabel: ringkasan dan detail.
        4. Laporan khusus: aging receivables, stock valuation.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 154427" src="https://github.com/user-attachments/assets/c33b3249-93d8-4da5-a68f-a431c41e796f" />

**8. Halaman Pengaturan**
      **Fungsi Utama:** Konfigurasi sistem: profil perusahaan, pajak, mata uang, template invoice, manajemen user & role.
      **Komponen:** 
        1. Profil perusahaan: nama, alamat, logo, kontak, NPWP.
        2. Konfigurasi pajak: persentase PPN, PPh, pengaturan pajak per produk.
        3. Manajemen user: tambah user, atur role (Admin, Manager, Staff Penjualan, Staff Gudang), reset password.
        4. Audit log: catatan aktivitas user (login, perubahan data penting).
        5. Backup / Restore data dan pengaturan integrasi (mis. email SMTP, API keys).
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 154541" src="https://github.com/user-attachments/assets/82ef347f-1924-4bb5-91e3-cd33d4d752f3" />

# **Langkah-langkah Menjalankan _WEB_**\
**1. Akses Awal dan _Login_**
      **Tujuan:** Masuk ke sistem sebagai user terdaftar.
      **Langkah:**
        1. Buka alamat web aplikasi.
        2. Pada halaman login, masukkan username/email dan password.
        3. Klik tombol “Login”.
      **Hasil:** Masuk ke Dashboard jika kredensial valid.

**2. Menambah Produk Baru**
      **Tujuan:** Menambahkan master data produk yang akan dijual/dibeli.
      **Langkah:**
        1. Masuk ke menu Produk / Products.
        2. Klik tombol Tambah Produk / Add New Product.
        3. Isi form:
            - Kode Produk (unik)
            - Nama Produk
            - Kategori (pilih dari dropdown atau buat kategori baru)
            - Satuan (pcs/kg/liter)
            - Harga Beli (cost) dan Harga Jual
            - Stok Awal (opsional) dan Minimal Stok
            - Pajak (jika ada)
            - Deskripsi singkat dan upload gambar (opsional)
            - Klik Simpan / Save.
      **Hasil:** Produk muncul di daftar produk; dapat dipilih saat membuat penjualan/pembelian.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 170118" src="https://github.com/user-attachments/assets/a05a34e5-c6b1-4570-96e8-28e7f143d395" />

**3. Mengedit dan menghapus produk**
      **Tujuan:** Perbaiki atau hapus data produk yang salah/tidak relevan.
      **Langkah edit:** 
        1. Di daftar produk, cari produk (pakai pencarian atau filter).
        2. Klik tombol Edit pada baris produk.
        3. Ubah field yang perlu diperbarui lalu klik Simpan.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 171718" src="https://github.com/user-attachments/assets/88919daf-d07e-46f3-a111-c201dbe17ead" />
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 171902" src="https://github.com/user-attachments/assets/67095973-da47-4289-82e0-1d7b6bbe3caa" />

   **Langkah hapus**
      1. Di daftar produk, klik tombol Hapus / Delete.
      2. Konfirmasi penghapusan pada popup.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 171820" src="https://github.com/user-attachments/assets/43f1342c-5170-4766-9d85-73bc8f6e954a" />
    **Hasil:** Produk diperbarui atau dihapus.

**4. Menambah Pelanggan Baru**
      **Tujuan:** Memasukkan data pelanggan agar mudah dipilih saat transaksi penjualan.
      **Langkah:** 
        1. Menu Pelanggan / Customers → Tambah Pelanggan.
        2. Isi: Nama, Email, Telepon, Alamat, Tipe Pelanggan, Syarat Pembayaran.
        3. Klik Simpan.
      **Hasil:** Pelanggan baru muncul di daftar dan dapat dipilih saat membuat invoice.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 171941" src="https://github.com/user-attachments/assets/ffbd16ca-b848-4c05-bfd0-cd2ec0a04955" />

**5. Membuat Penjualan/Invoice**
      **Tujuan:** Mencatat penjualan dan menghasilkan invoice.
      **Langkah:** 
        1. Menu Penjualan / Sales → Buat Penjualan Baru / New Invoice.
        2. Pilih Pelanggan (cari dari daftar).
        3. Tambah Produk ke keranjang: pilih produk → masukkan kuantitas → tentukan diskon per item (jika ada).
        4. Periksa ringkasan: subtotal, diskon, pajak, total.
        5. Pilih Metode Pembayaran (Tunai/Transfer/Kredit) dan Masukkan status pembayaran (Paid/Unpaid/Due Date).
        6. Klik Simpan atau Simpan & Cetak / Kirim Email bila perlu.
      **Hasil:** Invoice tersimpan; stok otomatis berkurang (jika sistem diatur demikian).
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 172032" src="https://github.com/user-attachments/assets/764d9786-54db-4d55-9102-0d8d543eb389" />

  **6. Mencatat Pembayaran dari Pelanggan**
      **Tujuan:** Menandai invoice sebagai dibayar dan mengurangi saldo piutang.
      **Langkah:**
        1. Buka menu Penjualan → cari invoice yang bersangkutan.
        2. Klik Record Payment atau Mark as Paid.
        3. Isi: Tanggal pembayaran, jumlah yang dibayar, metode pembayaran, no. bukti/transfer.
        4. Simpan.
      **Hasil:** Invoice terupdate statusnya menjadi Paid (atau partially paid), catatan transaksi pembayaran disimpan.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 172140" src="https://github.com/user-attachments/assets/4fc730ff-13ce-4081-b816-98dc8feb9834" />

  **7. Membuat Purchase Order (PO) & Menerima Barang**
      **Tujuan:** Mengajukan pembelian ke supplier dan menerima barang ke gudang.
      **Langkah membuat PO:** 
        1. Menu Pembelian / Purchases → Buat Purchase Order.
        2. Pilih supplier, tambahkan produk & qty, set harga beli, estimasi tanggal tiba.
        3. Simpan & cetak PO (opsional).
      **Hasil:** Stok diperbarui sesuai qty diterima; status PO berubah sesuai realisasi.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 172233" src="https://github.com/user-attachments/assets/629ef5d7-7054-44f5-92ca-a3d4f23abcd7" />

**8. Menjalankan Stock Opname / Penyesuaian Stok**
      **Tujuan:** Menyamakan catatan stok sistem dengan kondisi fisik gudang.
      **Langkah:** 
        1. Menu Inventory → Stock Opname → Buat session opname baru.
        2. Pilih lokasi/gudang dan rentang produk yang akan dicek.
        3. Untuk tiap produk, input hasil hitungan fisik.
        4. Sistem menampilkan selisih (fisik vs sistem).
        5. Konfirmasi & buat penyesuaian stok (adjustment) jika perlu.
      **Hasil:** Stok di sistem di-update sesuai hasil fisik; catatan adjustment tersimpan untuk audit.
    <img width="1920" height="1200" alt="Screenshot 2025-10-21 172416" src="https://github.com/user-attachments/assets/383d92ab-36c2-4a80-9b17-1e6a857f30e9" />

**9. Membuat Laporan & Mengekspor Data**
      **Tujuan:** Mengambil laporan untuk analisis atau penilaian tugas.
      **Langkah:** 
        1. Menu Reports → pilih jenis laporan (Penjualan, Pembelian, Persediaan, Laba Rugi).
        2. Set filter: periode tanggal, customer, produk, gudang.
        3. Klik Generate / Preview.
        4. Jika sesuai, klik Export → pilih format (Excel, PDF, CSV).
      **Hasil:** File laporan diunduh dan siap diserahkan/diolah.

# **ALUR KERJA LENGKAP (WORKFLOW)**
Berikut contoh langkah nyata yang menunjukkan hubungan antar modul:
1. Tambah Produk: Admin menambahkan 10 produk baru (Products → Add).
2. Buat Purchase Order ke Supplier untuk refill stok (Purchases → New PO).
3. Terima Barang saat barang datang (Purchases → Receive Goods) → stok di Inventory bertambah.
4. Buat Pelanggan jika pelanggan baru melakukan pembelian (Customers → Add).
5. Buat Penjualan: Staff penjualan membuat invoice, memilih produk dan qty (Sales → New Invoice).
6. Catat Pembayaran: Pelanggan bayar via transfer; staff mencatat pembayaran (Sales → Record Payment).
7. Lihat Laporan: Manager membuat laporan penjualan per minggu (Reports → Sales by Date Range → Export → PDF).
8. Stock Opname: Tim gudang melakukan stock opname bulanan (Inventory → Stock Opname) → lakukan penyesuaian jika perlu.








 









