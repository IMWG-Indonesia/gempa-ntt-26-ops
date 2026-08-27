# GEMPA-NTT-26

Papan tugas Information Management untuk respons Gempa NTT, dikelola bersama oleh IMWG Indonesia dan Sekretariat IHCP.

| | |
|---|---|
| **Papan tugas** | [Buka papan](https://github.com/orgs/IMWG-Indonesia/projects/5/views/1) |
| **Folder kerja bersama** | [Google Drive IMWG](https://drive.google.com/drive/folders/1HJVCke1NuWa8Om2K1YWvnJ_z0upt6Ooo?usp=sharing), akses lewat permintaan |
| **Koordinasi harian** | Grup WhatsApp, lewat undangan |

---

## Mulai dari sini

**Yang perlu diketahui untuk mulai berkontribusi cuma tiga hal:**

1. Ambil tugas dari kolom **Prioritas Hari Ini**
2. Tulis di kolom komentar bahwa kamu mengambilnya
3. Unggah hasilnya ke folder kerja bersama, tempel tautannya di tugas

Sisanya di halaman ini adalah penjelasan, bukan syarat.

Belum pernah memakai GitHub? Tidak masalah, dan tidak ada yang bisa dirusak karena semua versi tersimpan. Panduan bergambar ada di folder [`howto`](howto).

> [!NOTE]
> Cara kerja di halaman ini masih dalam bentuk awal dan sengaja belum lengkap. Isinya akan berubah mengikuti apa yang ternyata dibutuhkan di lapangan.

---

## Untuk semua

### Jenis tugas

Memakai issue type bawaan GitHub, ditetapkan di tingkat organisasi sehingga berlaku di semua aktivasi.

| Jenis | Dipakai untuk |
|---|---|
| **Task** | Permintaan produk informasi yang sudah jelas keluarannya dan bisa ditentukan kapan selesainya. |
| **Finding** | Temuan yang muncul di luar tugas yang sedang dikerjakan, misalnya sumber data baru, angka yang tidak cocok antar sumber, atau wilayah yang tidak terdata. Dicatat dulu, ditriase belakangan. |
| **Incident** | Produk atau data yang sudah beredar dan ternyata bermasalah. Bukan untuk perangkat lunak. |
| **Bug** | Cacat pada perkakas yang kita kembangkan sendiri, misalnya skrip pengolah atau dasbor buatan sendiri. **Bukan** untuk data yang keliru, untuk itu pakai Incident. |
| **Feature** | Kemampuan baru pada perkakas yang kita kembangkan sendiri. |

Dua baris terakhir sengaja menyebut apa yang **bukan** cakupannya. Tanpa itu, orang yang tidak berlatar belakang perangkat lunak hampir pasti memilih "Bug" ketika ada angka yang salah, dan hitungan insiden data jadi kacau sejak minggu pertama.

Jenis **Finding** adalah yang paling sering terlupa, padahal paling berharga di respons. Dalam sepuluh hari pertama, sebagian besar hal berguna justru ditemukan orang secara kebetulan sambil mengerjakan hal lain. Tanpa wadah, temuan itu tenggelam di percakapan.

---

### Struktur badan tugas

Tujuh bagian tetap untuk jenis Task. Semuanya sudah tersedia sebagai formulir, jadi tidak perlu diketik ulang.

```
Pekerjaan        Satu kalimat, apa yang dikerjakan.
Tujuan           Masalah konkret apa yang ditutup, keputusan apa yang dibantu.
Hasil            Daftar keluaran yang bisa diperiksa.
Selesai bila     Kriteria yang bisa dicek sendiri tanpa bertanya balik.
Format           Wujud berkas dan di folder mana disimpan.
Sumber data      Tautan. Yang belum ada ditulis "belum tersedia", bukan dikosongkan.
Diminta oleh     Nama pemohon, bukan pengerja.
Asal permintaan  Dari percakapan mana dan tanggal berapa. Boleh kosong kalau
                 permintaannya memang lahir di papan ini.
```

#### Contoh tugas yang sudah terisi

> **Analisis Data Sekunder Gempa NTT 2026** `#16`
> Jenis: Task · Label: `bidang:analisis` `wilayah:semua`
> Prioritas: High · Target date: 28 Agustus · Effort: 8 jam · Diminta oleh: Sekretariat IHCP
>
> ---
>
> **Pekerjaan**
> Kompilasi dan analisis data sekunder Gempa M7,7 Flores memakai kerangka analisis tiga pilar: dampak krisis, kondisi kemanusiaan, serta kapasitas dan respons.
>
> **Tujuan**
> Laporan situasi yang beredar sejauh ini masih berhenti di angka dampak, sehingga rapat koordinasi belum punya dasar untuk menjawab dua pertanyaan yang berulang ditanyakan: apa artinya angka itu bagi penduduk terdampak, dan di wilayah mana gap respons paling besar.
>
> **Hasil**
> Ringkasan bencana sepanjang tiga sampai lima halaman, berisi:
> 1. Profil krisis dan estimasi dampak, memakai peta serta tabel dari tugas #12
> 2. Profil kerentanan wilayah terdampak, dari data kependudukan, kemiskinan, dan akses layanan
> 3. Pemetaan kapasitas dan gap respons, mencakup pemerintah dan lembaga yang sudah beroperasi
> 4. Kesimpulan analitis dan daftar kebutuhan prioritas
>
> **Selesai bila**
> - Setiap angka dalam dokumen bisa ditelusuri ke sumbernya oleh orang yang tidak menyusunnya
> - Bagian kebutuhan prioritas menyebut wilayah spesifik, bukan hanya sektor
> - Satu orang di luar penyusun sudah membaca dan bisa menyebutkan tiga wilayah prioritas tanpa penjelasan lisan
>
> **Format**
> Word (.docx) dan PDF, diunggah ke folder kerja bersama pada `/produk/analisis/`
>
> **Sumber data**
> - Keluaran tugas #12: peta situasi awal dan tabel statistik zonal
> - Laporan situasi IHCP nomor 1 sampai 3
> - Data guncangan GDACS, tautan pada tugas #12
> - Data kependudukan dan sosial ekonomi BPS NTT: Kecamatan Dalam Angka, Susenas
> - Data kebencanaan historis BNPB (DIBI)
> - Rujukan kerangka analisis: IFRC Analysis Framework
>
> **Diminta oleh**
> Sekretariat IHCP

Perhatikan bahwa **Prioritas dan Tenggat tidak muncul di badan tugas**, melainkan di baris field pada bagian atas. Ini yang membuat keduanya bisa disortir dan difilter. Kalau ditulis di badan, papan tidak bisa diurutkan menurut tenggat, dan setiap perubahan meninggalkan versi lama di dalam teks.

Perhatikan juga rujukan silang ke tugas `#12`. Tugas yang bergantung pada keluaran tugas lain sebaiknya menyebut nomornya, bukan mengulang isinya. Menyebut nomor membuat GitHub menautkan keduanya secara otomatis, sehingga terlihat dari kedua arah.

#### "Selesai bila" adalah bagian yang paling menentukan

Tanpa bagian ini, "kompilasi data lembaga per kabupaten" bisa dianggap selesai dengan dua belas baris atau dua ratus. Tulis kriteria yang bisa diverifikasi:

- Kurang baik: "Datanya sudah bersih"
- Lebih baik: "Setiap baris punya nama kabupaten yang cocok dengan kode wilayah resmi, dan baris tanpa pasangan sudah didaftar terpisah beserta alasannya"

Kriteria terbaik memaksa pemeriksaan oleh orang yang berbeda. Untuk produk informasi, bentuknya biasanya begini: *"satu orang di luar pembuat sudah membaca peta ini dan bisa menyebutkan tiga wilayah prioritas tanpa penjelasan lisan."*

Alasannya sederhana. Produk informasi yang hanya bisa dijelaskan oleh pembuatnya belum menyelesaikan masalah apa pun. Begitu orang itu tidak hadir di rapat, produknya kembali jadi gambar yang bagus.

---

### Label

Tiga dimensi. Jumlahnya sengaja ditahan supaya tim kecil tidak menghabiskan waktu memilih label.

**`bidang:`** menunjukkan keahlian yang dibutuhkan. Satu per tugas, wajib.

| Label | Keahlian yang dicari |
|---|---|
| `bidang:gis` | Analisis geospasial dan produksi peta |
| `bidang:data` | Pembersihan, penggabungan, dan pengolahan data tabular |
| `bidang:mdc` | Perancangan formulir pendataan dan pengelolaan datanya |
| `bidang:infografis` | Produk grafis statis: poster, ringkasan satu halaman, ilustrasi. Dikerjakan dengan Inkscape, Illustrator, Canva, atau sejenisnya. |
| `bidang:dashboard` | Tampilan data yang bisa ditelusuri sendiri oleh pembacanya. Power BI, Looker Studio, Tableau, atau buatan sendiri dengan HTML/CSS/JS. |
| `bidang:analisis` | Penafsiran situasi dan kebutuhan, bukan sekadar penyajian angka |
| `bidang:qa` | Pemeriksaan mutu sebelum produk beredar |
| `bidang:dokumentasi` | Metodologi, catatan sumber, panduan |

Dua label yang paling sering tertukar adalah `bidang:infografis` dan `bidang:dashboard`. Pembedanya bukan perkakas, melainkan **apakah pembacanya bisa menelusuri sendiri.** Infografis sudah selesai saat dikirim, karena pembaca menerima kesimpulan yang sudah dipilihkan. Dasbor menyerahkan penyaringan kepada pembaca, sehingga menuntut data yang lebih rapi dan pemutakhiran yang berkelanjutan.

Ini penting saat menerima permintaan. "Bikin dasbor" sering sebenarnya berarti "saya butuh satu gambar untuk rapat besok", dan kalau salah dibaca, kita membangun sesuatu yang perlu dirawat berbulan-bulan padahal yang dibutuhkan cuma satu lembar. Kalau ragu, tanyakan di tugasnya: apakah ini akan dibuka berulang kali, atau cukup sekali dipakai lalu selesai.

**`wilayah:`** menunjukkan cakupan geografis. Satu per tugas, wajib. Pakai `wilayah:semua` untuk produk yang lintas wilayah.

**`tanda:`** boleh lebih dari satu, boleh tidak ada. Ini yang tidak bisa digantikan field, karena field hanya menampung satu nilai.

| Tanda | Arti |
|---|---|
| `tanda:butuh-keputusan` | Menunggu keputusan sekretariat sebelum bisa jalan |
| `tanda:butuh-data` | Terhambat karena sumber datanya belum ada atau belum bisa diakses |
| `tanda:menunggu-pihak-luar` | Menunggu jawaban dari luar jejaring. Sebutkan siapa dan sejak kapan di komentar. |
| `tanda:cepat` | Selesai di bawah dua jam, cocok untuk kontributor yang baru bergabung |
| `tanda:sensitif` | Menyangkut data pribadi atau informasi yang bisa merugikan bila salah beredar. Wajib diperiksa orang kedua sebelum keluar. |

Tiga tanda pertama adalah **antrean koordinator, bukan antrean kontributor.** Filter ketiganya setiap beberapa hari. Kalau menumpuk, yang memperlambat produksi kemungkinan besar bukan kurangnya tenaga.

`tanda:cepat` sebaiknya selalu ada isinya. Kontributor baru yang membuka papan dan hanya melihat tugas berdurasi enam jam biasanya menutupnya lagi.

---

### Papan

Kolom: `Permintaan Masuk` → `Prioritas Hari Ini` → `Dikerjakan` → `Review` → `Selesai`, ditambah `Terhambat` di samping.

**Permintaan Masuk** berarti sudah tercatat, belum siap dikerjakan. Semua tugas baru mendarat di sini, dari siapa pun asalnya.

**Terhambat** bukan tahap yang dilewati semua tugas, melainkan tempat parkir sementara. Tugas yang macet karena menunggu keputusan atau akses data dipindah ke sana, lalu kembali ke Dikerjakan begitu hambatannya hilang. Tanpa kolom ini, tugas yang berhenti akan tetap duduk di Dikerjakan dan tampak seolah masih berjalan.

Batasi **Dikerjakan** maksimal dua tugas per orang. Untuk kontributor sukarela dengan slot beberapa jam, lebih dari itu artinya ada yang cuma berpindah kolom.

Buat papan di **tingkat organisasi**, bukan repo, supaya bisa menarik tugas dari beberapa aktivasi. Field organisasi tidak otomatis muncul sebagai kolom, harus ditambahkan lewat tombol `+`.

Dua tampilan yang cukup:

- **Papan** dikelompokkan menurut status, untuk kerja harian
- **Tabel** diurutkan menurut tenggat dengan saringan `tanda:`, untuk tinjauan berkala

---


---

## Untuk koordinator dan petugas piket

Bagian ini tidak perlu dibaca kalau kamu datang untuk mengerjakan tugas.

### Field

Ditetapkan di tingkat organisasi. Field harus diatur **visibility**-nya ke jenis tugas tertentu, kalau tidak dia tidak muncul di panel kanan. Ini yang sering bikin orang mengira fiturnya rusak.

| Field | Dipakai untuk |
|---|---|
| **Priority** | Urgent / High / Medium / Low. Pakai apa adanya. |
| **Target date** | Menggantikan baris tenggat di badan tugas, sehingga bisa disortir. |
| **Effort** | **Perkiraan jam kerja, bukan hari.** Satuan ini yang membuat kontributor berslot dua jam bisa menyaring sendiri tugas yang muat. |
| **Diminta oleh** | Field kustom, pilihan tunggal. Berguna untuk melihat dari mana permintaan sebenarnya datang, dan permintaan pihak mana yang paling sering menggantung. |

---

### Siapa mengisi apa

Ini pembagian yang paling menentukan apakah papan ini berguna atau justru menyesatkan.

| Bagian | Diisi oleh |
|---|---|
| Pekerjaan, Tujuan, Hasil, Format, Sumber data, Diminta oleh | Pemohon |
| Target date | Pemohon |
| Effort, Priority, seluruh label | Petugas piket saat triase |
| Koreksi Effort | Pengambil tugas, saat mulai mengerjakan |

**Pemohon tidak mengisi Effort.** Dia tahu apa yang dibutuhkan dan kapan, tetapi tidak tahu berapa lama membuatnya, dan memang tidak perlu tahu. Kalau tetap ditanya, semua akan terisi angka yang sama, lalu kontributor mengambil tugas yang dikira muat dua jam padahal enam. Sekali itu terjadi, kepercayaan pada seluruh angka Effort hilang dan tidak kembali.

**Pengambil tugas mengoreksi Effort** kalau ternyata meleset, sebagai hal pertama yang dilakukan saat mengambil. Estimasi piket pun tebakan. Koreksi dari orang yang benar-benar mengerjakan adalah satu-satunya cara angka itu jadi akurat seiring waktu.

### Triase harian

Siapa saja boleh membuat tugas. Tidak ada persetujuan, tidak ada moderasi. Yang ada adalah triase ringan.

Sekali sehari, petugas piket menyisir kolom Permintaan Masuk selama kira-kira lima belas menit:

1. Melengkapi Effort, Priority, dan ketiga label
2. Menambahkan `tanda:butuh-data` kalau sumbernya belum tersedia
3. Menanyakan hal yang belum jelas lewat kolom komentar
4. Memindahkan tugas yang sudah lengkap ke **Prioritas Hari Ini**

Aturan turunannya satu kalimat: **kontributor hanya mengambil tugas dari Prioritas Hari Ini, tidak pernah dari kolom Permintaan Masuk.** Ini yang menjamin tidak ada orang yang mengambil tugas berisi estimasi asal-asalan.

Piket bergilir, bukan satu orang tetap. Lima belas menit sehari adalah beban yang wajar, dan menyebarkannya ke beberapa orang membuat papan ini tidak berhenti setiap kali satu orang sibuk.

#### Jalur mendesak

Triase harian berarti permintaan yang masuk sore hari baru siap dikerjakan besok. Untuk sebagian situasi itu terlalu lambat.

Permintaan yang benar-benar mendesak tetap disampaikan lewat WhatsApp, dikerjakan lebih dulu, dan tugasnya dicatat menyusul. Mekanisme yang tidak punya jalur darurat akan dilanggar diam-diam, dan sekali dilanggar tanpa akibat, seluruh disiplinnya ikut longgar.

---

### Dari percakapan ke papan, lalu kembali

Sebagian besar permintaan tidak lahir di papan. Datangnya dari grup WhatsApp, telepon, japri, atau rapat. Kalau dibiarkan berhenti di sana, papan ini akan berisi sebagian kecil saja dari pekerjaan yang sebenarnya berjalan, dan itu lebih menyesatkan daripada tidak punya papan sama sekali.

Alurnya tiga langkah:

1. **Permintaan muncul** di percakapan mana pun
2. **Disadur ke papan** dengan format baku, mencantumkan asal permintaannya
3. **Diumumkan kembali** ke grup WhatsApp beserta tautannya

Langkah ketiga yang paling sering dilewat, padahal justru itu yang membuat mekanisme ini terasa berguna bagi orang yang tidak membuka GitHub. Pemohon melihat permintaannya diterima dan tercatat. Kontributor melihat ada pekerjaan baru yang bisa diambil. Keduanya tidak perlu memantau papan untuk tahu.

#### Format pengumuman ke WhatsApp

Disalin dari tugas yang sudah dibuat, dipangkas seperlunya supaya nyaman dibaca di layar ponsel.

```
🆕 *TUGAS BARU* #23

*Apa*: Peta sebaran lokasi pengungsian per kecamatan
*Untuk*: Bahan rapat koordinasi lintas klaster
*Hasil*: Peta A3 dengan titik pengungsian, jumlah jiwa,
dan nama kecamatan
*Format*: PNG dan PDF

*Bidang*: gis
*Prioritas*: Tinggi
*Tenggat*: 28 Agustus, 17.00
*Perkiraan*: 3 jam
*Pemohon*: Sekretariat IHCP

Ambil di sini, tulis di komentar kalau mengambilnya:
https://github.com/IMWG-Indonesia/gempa-ntt-26-ops/issues/23
```

Beberapa hal yang sengaja tidak ikut disalin:

**Sumber data** biasanya berupa beberapa tautan panjang yang membuat pesan sulit dibaca di ponsel. Cukup ada di tugasnya.

**Selesai bila** memang penting, tetapi bacaannya untuk orang yang sudah memutuskan mengambil, bukan untuk orang yang sedang menimbang. Menaruhnya di pengumuman membuat pesan terasa berat.

**Perkiraan jam kerja** justru wajib ada, karena itu satu-satunya angka yang dipakai orang untuk memutuskan apakah pekerjaan ini muat di waktu luangnya. Kalau saat mengumumkan angkanya belum ada, berarti tugas itu belum ditriase dan belum siap diumumkan.

#### Siapa yang mengumumkan

Pengumuman dikirim oleh **koordinator IM yang sedang bertugas**, yaitu orang yang hari itu menyisir kolom Permintaan Masuk. Perannya melekat pada hari, bukan pada nama, dan siapa pun yang ditunjuk bisa memegangnya.

Cukup sekali sehari, satu pesan, berisi semua tugas yang selesai ditriase hari itu. Mengumumkan setiap kali ada tugas baru terdengar lebih responsif, tetapi dalam praktiknya lebih sulit dijaga dan lebih cepat membuat grup jenuh.

Karena jejaring ini berjalan atas dasar kesukarelaan, akan ada hari ketika yang bertugas berhalangan dan tidak sempat mengabari. Itu wajar dan tidak perlu diperlakukan sebagai pelanggaran. Dua aturan sederhana yang menjaganya tetap berjalan:

- Siapa pun boleh mengumumkan kalau yang bertugas belum sempat. Tidak perlu izin.
- Tugas yang terlanjur diumumkan dua kali jauh lebih ringan akibatnya daripada tugas yang tidak pernah diumumkan sama sekali.

Sebutkan nama yang bertugas hari itu di grup, satu baris saja. Ini bukan formalitas: peran yang tidak disebut siapa pemegangnya akan diasumsikan dipegang orang lain, dan akhirnya tidak dipegang siapa pun.

#### Kapan tidak perlu diumumkan

Tidak setiap tugas layak jadi pesan di grup. Tugas yang sudah jelas siapa pengerjanya sejak awal, atau yang lahir dari percakapan yang sedang berlangsung di grup itu juga, cukup dibalas dengan tautannya saja.

Grup yang menerima pengumuman terlalu sering akan berhenti membacanya, dan saat itu terjadi, pengumuman yang benar-benar butuh kontributor pun ikut terlewat.

Untuk tugas yang sudah selesai, pengumuman berbentuk lebih pendek dan lebih berguna dikirim menempel pada produknya:

```
✅ *SELESAI* #23 Peta sebaran lokasi pengungsian
Dikerjakan oleh: (nama)
Berkas: (tautan folder kerja bersama)
```

---

## Usulan perbaikan

Cara kerja di dokumen ini masih tebakan awal. Sebagian mungkin tidak berguna, sebagian mungkin justru menghambat.

Kalau ada yang membingungkan, merepotkan, atau kurang, sampaikan saja di grup WhatsApp atau lewat komentar di tugas mana pun. Tidak perlu usulan yang matang, keluhan setengah jadi juga berguna.
