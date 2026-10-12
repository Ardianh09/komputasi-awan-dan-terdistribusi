# Jurnal Proses — Tugas 4

## Jalur yang dipilih
- RPC (Jalur A), alasan: kebutuhan utama di studi kasus adalah respons seketika
  (cek saldo) sehingga pola sinkron request-response paling cocok. Selain itu
  xmlrpc bagian dari standard library Python sehingga tidak butuh install
  apa pun, dan hasilnya langsung bisa diuji di satu laptop.

## Kendala teknis
- Error saat setup (mis. koneksi RabbitMQ ditolak, port bentrok): ...

## Uji "pesan tidak hilang" (khusus Jalur B)
- Langkah uji: matikan consumer → jalankan publisher → nyalakan consumer
- Hasil yang diamati: ...

## Log Penggunaan AI (Level 2)

> Wajib diisi sesuai kebijakan Level 2 di [`../RUBRIK-UMUM.md`](../RUBRIK-UMUM.md). Tulis "Tidak memakai AI" pada baris pertama jika memang tidak dipakai. Hanya untuk brainstorming ide/outline — bukan untuk kode/analisis/teks akhir.

| Tanggal | Tool AI | Prompt yang diberikan | Ringkasan saran/ide AI | Bagaimana diolah jadi tulisan/kode sendiri |
|---|---|---|---|---|
| ... | ... | ... | ... | ... |
