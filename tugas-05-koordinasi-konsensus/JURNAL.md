# Jurnal Proses — Tugas 5

## Implementasi Bully
- Kendala saat mengisi TODO 1-4: ...

## Skenario 1: Start normal
- Leader yang terpilih: leader 5 
- Log/observasi: 1. Siapa yang jadi leader dan dari mana kalian tahu. Node 5 mencetak “Saya jadi LEADER”, dan node 1-4 mencetak “Leader sekarang: node 5”.
                 2. Alur election yang terlihat. Node ber-ID kecil mengirim ELECTION ke semua node di atasnya, lalu dibalas OK oleh node yang lebih tinggi dan mundur menunggu COORDINATOR.
                 3. Kenapa node 5 yang menang. Node 5 tidak punya peer yang lebih tinggi (peer lebih tinggi: {}), jadi tidak ada yang membalas OK, timeout 2 detik habis, lalu dia broadcast COORDINATOR.

## Skenario 2: Leader dimatikan
- Leader baru yang terpilih: leader 4 
- Berapa lama waktu sampai leader baru terdeteksi: sekitar 11,62 detik dengan waktu reaksi manual 

## Log Penggunaan AI (Level 2)

> Wajib diisi sesuai kebijakan Level 2 di [`../RUBRIK-UMUM.md`](../RUBRIK-UMUM.md). Tulis "Tidak memakai AI" pada baris pertama jika memang tidak dipakai. Hanya untuk brainstorming ide/outline — bukan untuk kode/analisis/teks akhir.

| Tanggal | Tool AI | Prompt yang diberikan | Ringkasan saran/ide AI | Bagaimana diolah jadi tulisan/kode sendiri |
|---|---|---|---|---|
| ... | ... | ... | ... | ... |
