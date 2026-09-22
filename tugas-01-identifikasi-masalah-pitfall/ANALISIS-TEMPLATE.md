# Tugas 1 — Analisis Pitfall FoodGo

**Kelompok:** [nama kelompok]

| Nama | NIM | Kontribusi |
|---|---|---|
| Ardian Hoart| [103072400098] | [pitfall 1] |
| [nama 2] | [nim] | [pitfall/bagian yang dikerjakan] |
| [nama 3] | [nim] | [pitfall/bagian yang dikerjakan] |

## Pitfall 1: [Bandwidth is infinite] — ditulis oleh [Ardian Hoart]

**Bukti di skenario:** Saat trafik naik, satu server yang menangani semua modul menjadi kewalahan.

**Kenapa ini keliru:** Server tidak memiliki resource yang tidak terbatas. CPU, RAM, koneksi, dan kemampuan server dalam memproses request semuanya memiliki batas. Jika jumlah pengguna meningkat secara tiba-tiba, server bisa kewalahan karena harus memproses terlalu banyak request dalam waktu yang bersamaan.

**Dampak ke FoodGo:** Saat jam makan siang atau ada promo besar, jumlah pengguna FoodGo meningkat dan banyak request masuk secara bersamaan. Karena semua modul seperti pesanan, pembayaran, dan notifikasi berjalan pada satu server, beban server menjadi terlalu tinggi. Akibatnya aplikasi menjadi lambat dan server bisa mengalami crash.

**Solusi desain awal:** FoodGo dapat menggunakan horizontal scaling, yaitu menambah beberapa server atau instance untuk membagi beban. Request dari pengguna dapat dibagi menggunakan load balancer. Untuk proses yang tidak harus langsung selesai, FoodGo juga dapat menggunakan message queue agar pekerjaan diproses secara bertahap.

**Trade-off:** Menambah server dapat membantu mengurangi beban pada satu server, tetapi biaya infrastruktur menjadi lebih besar. Selain itu, sistem juga menjadi lebih kompleks karena harus mengatur beberapa server dan melakukan monitoring terhadap masing-masing server.

---

## Pitfall 2: [nama pitfall] — ditulis oleh [nama]

(ulangi struktur di atas)

---

## Pitfall 3: [nama pitfall] — ditulis oleh [nama]

(ulangi struktur di atas)

---

## Kesimpulan Kelompok

[Ringkasan: jika FoodGo memperbaiki ketiga pitfall ini, apa arsitektur yang disarankan secara garis besar? Kaitkan dengan Tugas 2.]
