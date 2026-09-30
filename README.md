# Strategic SWOT → BMC — Simple GitHub Edition

Aplikasi statis satu halaman untuk membantu organisasi/proyek/produk:
1. mendefinisikan konteks keputusan;
2. mengidentifikasi Strengths, Weaknesses, Opportunities, dan Threats berbasis bukti;
3. menghasilkan alternatif strategi TOWS (SO, WO, ST, WT) secara transparan;
4. memprioritaskan strategi dengan heuristic sederhana dan dapat ditelusuri;
5. menerjemahkan strategi terpilih menjadi rencana aksi;
6. memetakan strategi ke 9 blok Business Model Canvas (BMC).

## Prinsip metodologis

- **SWOT adalah analisis situasi**, bukan algoritme prediksi.
- S/W diperlakukan sebagai faktor internal; O/T sebagai faktor eksternal.
- Setiap faktor menyediakan kolom **bukti/sumber**. Bukti tidak dicampur ke skor prioritas agar kualitas bukti tidak disamakan dengan besarnya dampak.
- Prioritas faktor = `Kepentingan × Urgensi` (1–25). Ini hanya heuristic pengurutan.
- TOWS digunakan untuk *matching*: SO, WO, ST, WT.
- Prioritas strategi = rata-rata empat penilaian skala 1–5: relevansi, dampak, kelayakan, dan kebalikan risiko; dikonversi menjadi 0–100. Bobot dibuat sama untuk transparansi, bukan karena ada klaim bahwa bobot itu universal.
- BMC tidak diisi dengan fakta yang tidak diberikan pengguna. Bila data tidak cukup, laporan menyatakan **Belum cukup data / belum diisi**.

## Basis sumber

Dokumen `ANALISISSWOT.pdf` yang diberikan pengguna menyatakan SWOT sebagai alat penting dalam perencanaan strategis, menekankan analisis situasi sebelum perumusan strategi, serta menyebut observasi, wawancara mendalam, kuesioner, dan studi dokumentasi sebagai teknik pengumpulan data. Aplikasi ini menggunakan bagian tersebut secara langsung dan tidak mengarang isi bab yang tidak tersedia dalam file.

Untuk penguatan eksternal:
- Weihrich, H. (1982). *The TOWS Matrix—A Tool for Situational Analysis*. Long Range Planning, 15(2), 54–66. DOI: 10.1016/0024-6301(82)90120-0.
- Strategyzer / Osterwalder: Business Model Canvas terdiri dari sembilan blok yang menggambarkan bagaimana organisasi menciptakan, menyampaikan, dan menangkap nilai. BMC harus diperlakukan sebagai model/hipotesis yang perlu diuji dan diperbarui ketika bukti baru muncul.

## Ekspor

- **Cetak / PDF**: tombol membuka dialog cetak browser; pilih “Save as PDF”.
- **Export DOC**: menghasilkan file `.doc` yang dapat dibuka oleh Microsoft Word/LibreOffice.
- **Reset**: menghapus semua data dari `localStorage` browser setelah konfirmasi.

## Deploy GitHub Pages

1. Buat repository GitHub.
2. Upload `index.html` dan `.nojekyll` ke root repository.
3. Commit ke branch `main`.
4. Buka **Settings → Pages**.
5. Pilih **Deploy from a branch → main → /(root)**.
6. Simpan dan tunggu URL GitHub Pages aktif.

Tidak membutuhkan server, database, Node.js, atau proses build.

## Batasan

Aplikasi ini tidak mengklaim validitas prediktif, kausal, atau probabilistik. Kualitas keluaran tergantung pada kualitas faktor, bukti, penilaian pengguna, serta validasi dan diskusi stakeholder. Rekomendasi otomatis TOWS bersifat **templated and traceable**: ia hanya menghubungkan faktor yang dimasukkan pengguna dan tidak menciptakan fakta baru.

Footer aplikasi: `@ramakertamukti`.
