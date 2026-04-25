# pbasisdata-pertemuan4-sitti-rahma-IK2411048

## Identitas Mahasiswa

| Keterangan | Detail |
|---|---|
| **Nama** | Sitti Rahma |
| **NIM** | IK2411048 |
| **Kelas** | Reguler |
| **Program Studi** | S1 Informatika |
| **Mata Kuliah** | Pemrograman Basis Data |
| **Dosen** | Abdul Malik, S.Kom., M.Cs. |
| **Tahun Akademik** | 2025/2026 |

---

## Ringkasan Tugas

**Pertemuan 4 — Struktur Kontrol Aliran: Percabangan (IF-THEN-ELSE dan CASE)**

Tugas ini berisi implementasi procedure MySQL bernama `cek_predikat_mahasiswa` yang digunakan untuk menentukan predikat dan status kelulusan mahasiswa secara otomatis berdasarkan nilai yang dimasukkan. Procedure menggunakan struktur percabangan `IF-THEN-ELSEIF-ELSE` tanpa melibatkan tabel database.

### Ketentuan Logika

| Nilai | Predikat | Status |
|---|---|---|
| 90 – 100 | Sangat Memuaskan | Lulus |
| 80 – 89 | Memuaskan | Lulus |
| 70 – 79 | Baik | Lulus |
| 60 – 69 | Cukup | Tidak Lulus |
| < 60 | Kurang | Tidak Lulus |

---

## Cara Menjalankan Script SQL

1. Pastikan XAMPP sudah berjalan dan layanan **MySQL/MariaDB** aktif.
2. Buka **phpMyAdmin** melalui browser di `http://localhost/phpmyadmin` atau gunakan **MySQL Shell**.
3. Import atau jalankan file SQL yang ada di folder `kode_sql/`.
4. Jalankan procedure dengan perintah berikut:

```sql
CALL cek_predikat_mahasiswa(85);
```

Ganti angka `85` dengan nilai yang ingin diuji.

### Contoh Output

```
+-------+------------+--------+
| nilai | predikat   | status |
+-------+------------+--------+
|    85 | Memuaskan  | Lulus  |
+-------+------------+--------+
```
