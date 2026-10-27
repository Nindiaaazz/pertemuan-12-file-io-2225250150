# Pertemuan 12 - File I/O dan Error Handling

**Nama:** Nindia Najihatuz Zahro  
**NIM:** 2225250150  
**Kelas:** 3E

## Tujuan
Membaca, memvalidasi, mengolah, dan menulis data file menggunakan Python serta menangani error dasar.

## Struktur Program
- `data/nilai.txt`: file input data nilai.
- `data/hasil_rekap.txt`: file output hasil rekap.
- `latihan/`: enam program latihan file I/O dan error handling.
- `tugas/rekap_nilai_file.py`: program utama rekap nilai.

## Format File Input
Data disimpan dalam format `NIM,nilai`, satu data per baris.

Contoh:
```text
A001,85
A002,78
A003,92
A004,abc
A005,74
A006,88
```

## Cara Menjalankan
Jalankan perintah berikut melalui terminal VS Code dari folder utama proyek:

```powershell
python tugas/rekap_nilai_file.py
```

## Error yang Ditangani
- `FileNotFoundError`: menangani file input yang tidak ditemukan.
- `ValueError`: menangani format data atau nilai yang tidak valid.

Baris kosong dilewati, dan baris dengan nilai tidak valid tidak dimasukkan dalam perhitungan.

## Hasil Rekap
Berdasarkan data contoh, program menghasilkan:
- Jumlah data valid: 5
- Rata-rata: 83.40
- Minimum: 74.00
- Maksimum: 92.00
- Jumlah lulus: 5

Mahasiswa dinyatakan lulus jika memperoleh nilai minimal 60.

## Test Case
1. **Data normal:** nilai valid berhasil diproses.
2. **File hilang:** program menampilkan pesan bahwa file tidak ditemukan.
3. **Nilai invalid:** baris `A004,abc` dilewati dan data lainnya tetap diproses.
4. **Baris kosong:** baris kosong dilewati.
5. **Batas lulus:** nilai 60 dihitung sebagai lulus.

## Refleksi
Saya mempelajari cara membaca dan menulis file menggunakan Python, mengolah data dengan `strip()` dan `split()`, serta menangani `FileNotFoundError` dan `ValueError` menggunakan `try-except`. Dengan demikian, kesalahan pada satu baris tidak harus menghentikan seluruh proses rekap.

## Bantuan dan Referensi
- Bahan Ajar Algoritma dan Pemrograman Pertemuan 12.
- Python Software Foundation, dokumentasi Python tentang membaca file dan penanganan exception.
- Bantuan AI digunakan untuk membantu memahami kode dan menyusun dokumentasi. Kode diuji melalui VS Code.
