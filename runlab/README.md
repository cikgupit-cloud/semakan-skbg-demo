# RunLab · Afiq × Ahnaf
Portal latihan 5K dua pelari, dibuat untuk GitHub Pages.

## Akses
Apabila GitHub Pages untuk repositori ini diaktifkan melalui Settings → Pages → Deploy from a branch → main → /(root), buka:
https://cikgupit-cloud.github.io/semakan-skbg-demo/runlab/

Fail ini ditempatkan dalam folder runlab/ supaya laman sekolah pada akar repositori tidak diubah.

## Fungsi
- Dashboard dua pelari, carta palang jarak mingguan, checklist yang boleh ditanda.
- Pelan 8 minggu pertama diambil daripada Google Sheets gabungan Afiq dan Ahnaf. Enam blok sasaran Afiq hingga 5K 17:30 (pace 3:30/km), dengan rehat 7 hari antara blok.
- Boleh menambah 7 hari / 4 minggu jika tertinggal; tarikh PB dan blok selepasnya berubah. Menanda minggu tertinggal juga menambah satu minggu.
- Log berasingan (Afiq/COROS, Ahnaf/Garmin), imej tangkap layar terkompres setempat, rekod PB manual.
- Import/eksport sandaran JSON.

## Had sambungan
**GitHub Pages ialah laman statik.** Plugin COROS ChatGPT tidak tersedia terus kepada JavaScript di portal. Sambungan COROS automatik memerlukan backend peribadi dan kebenaran/saluran data yang sesuai. Gambar Garmin boleh dilampirkan, tetapi OCR automatik belum disediakan. Tiada tindakan sebenar menghantar data larian ke GitHub atau Google Sheets.

Data peribadi dan HR tidak dimasukkan dalam fail projek di repositori awam. Semua catatan pengguna disimpan dalam localStorage pelayar dan hanya pada peranti itu. Pindahkan rekod menggunakan Tetapan → Eksport JSON dan Import JSON. Fail permulaan peribadi mesti dimuat turun daripada ChatGPT dan diimport sendiri; jangan commit fail itu ke repositori awam.

## Keselamatan latihan
Sasaran 3:30/km ialah aspirasi jangka panjang Afiq, bukan sasaran wajib mengikut kalendar. Ahnaf berumur 9 tahun mengikut hari/jenis sesi tetapi **tidak** perlu mengikut pace dewasa; utamakan rehat, bermain, keseronokan dan intensiti yang sesuai.

## Fail
- index.html — rangka halaman
- styles.css — tema & responsif
- app.js — checklist, log, carta, road map, sandaran
- plan-data.js — templat pelan minggu dari Google Sheets tanpa HR atau data peribadi
