# Jurnal Proses — Tugas 1

> Isi jurnal ini selama proses diskusi berlangsung, bukan ditulis ulang rapi di akhir. Tulis dengan gaya bebas — poin diskusi, kebuntuan, perubahan pikiran.

## [Tanggal diskusi 1]
- Peserta: [nama-nama yang hadir]
- Poin diskusi: ...
- Perbedaan pendapat (jika ada): ...

## [Tanggal diskusi 2]
- ...

## Review Silang
- [Nama] mengomentari analisis [Nama lain]: ...

## Log Penggunaan AI (Level 2)

> Wajib diisi sesuai kebijakan Level 2 di [`../RUBRIK-UMUM.md`](../RUBRIK-UMUM.md). Tulis "Tidak memakai AI" pada baris pertama jika memang tidak dipakai. Hanya untuk brainstorming ide/outline — bukan untuk kode/analisis/teks akhir.

| Tanggal | Tool AI | Prompt yang diberikan | Ringkasan saran/ide AI | Bagaimana diolah jadi tulisan/kode sendiri |
|---|---|---|---|---|
| 22 September 2026 |  GPT |Saya sedang membahas Bandwidth infinite pada studi kasus FoodGo, yaitu aplikasi pesan-antar makanan yang mengalami masalah ketika trafik meningkat dan satu server menangani semua modul. Tolong bantu saya brainstoorming saja, jangan buat jawaban tugas yang siap dikumpulkan. Berikan: 1.  Ide sederhana kenapa asumsi resource tidak terbatas itu salah. 2.  Contoh dampaknya pada FoodGo. 3.  Beberapa ide solusi desain awal. 4. Contoh trade-off dari solusi tersebut.|1. Kenapa asumsi ini salah? Setiap server memiliki kemampuan yang terbatas, seperti RAM, CPU, dan koneksi jaringan,Jumlah request akan bertambah ketika jumlah pengguna semakin banyak,Jika semua request ditangani oleh satu server, beban kerja server akan semakin berat, Jadi, kapasitas server tidak bisa dianggap mampu menangani pengguna dalam jumlah yang tidak terbatas. 2. Dampaknya pada FoodGo. Ketika jam makan siang atau sedang ada promo, jumlah pengguna FoodGo bisa meningkat,Server harus menangani proses pesanan, pembayaran, dan notifikasi secara bersamaan,Hal tersebut membuat penggunaan resource server menjadi tinggi,Akibatnya aplikasi dapat menjadi lambat dan beberapa request mengalami timeout,Jika beban terlalu tinggi, server juga dapat mengalami crash. 3. Ide solusi desain awal. Menambah beberapa server agar beban tidak hanya ditanggung oleh satu server,Menggunakan load balancer untuk membagi request ke beberapa server,Memisahkan fungsi pesanan, pembayaran, dan notifikasi agar tidak semuanya bergantung pada satu proses,Menggunakan message queue untuk pekerjaan yang tidak perlu langsung diproses,Menggunakan caching agar request yang sama tidak perlu selalu diproses dari awal. 4. Contoh trade-off. Penambahan server tentu membutuhkan biaya infrastruktur yang lebih besar,Semakin banyak server dan service yang digunakan, pengelolaannya juga menjadi lebih rumit,Penggunaan load balancer membutuhkan konfigurasi dan pemantauan tambahan,Message queue dapat membuat beberapa proses membutuhkan waktu lebih lama karena harus menunggu proses dalam antrean.|1.Server tidak memiliki resource yang tidak terbatas. CPU, RAM, koneksi, dan kemampuan server dalam memproses request semuanya memiliki batas. Jika jumlah pengguna meningkat secara tiba-tiba, server bisa kewalahan karena harus memproses terlalu banyak request dalam waktu yang bersamaan, 2.Saat jam makan siang atau ada promo besar, jumlah pengguna FoodGo meningkat dan banyak request masuk secara bersamaan. Karena semua modul seperti pesanan, pembayaran, dan notifikasi berjalan pada satu server, beban server menjadi terlalu tinggi. Akibatnya aplikasi menjadi lambat dan server bisa mengalami crash, 3.FoodGo dapat menggunakan horizontal scaling, yaitu menambah beberapa server atau instance untuk membagi beban. Request dari pengguna dapat dibagi menggunakan load balancer. Untuk proses yang tidak harus langsung selesai, FoodGo juga dapat menggunakan message queue agar pekerjaan diproses secara bertahap, 4.Menambah server dapat membantu mengurangi beban pada satu server, tetapi biaya infrastruktur menjadi lebih besar. Selain itu, sistem juga menjadi lebih kompleks karena harus mengatur beberapa server dan melakukan monitoring terhadap masing-masing server.|
