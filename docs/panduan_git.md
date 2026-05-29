# Panduan Git untuk Pemula

Dokumen ini adalah referensi cepat perintah Git yang paling sering dipakai.
Simpan ini, buka setiap kali lupa.

---

## Konsep dasar (baca ini dulu)

Git adalah sistem yang **mencatat setiap perubahan file** yang kamu buat.
Bayangkan seperti "save game" di video game — kamu bisa kembali ke titik manapun.

GitHub adalah **tempat penyimpanan online** untuk project Git kamu.

```
Komputer kamu  →  (git push)  →  GitHub
GitHub         →  (git pull)  →  Komputer kamu
```

---

## Setup awal (hanya sekali)

```bash
# Kenalkan dirimu ke Git
git config --global user.name "Nama Kamu"
git config --global user.email "email@kamu.com"
```

---

## Alur kerja harian

### 1. Mulai repo baru dari nol
```bash
git init
git add .
git commit -m "initial commit: setup struktur folder"
```

### 2. Hubungkan ke GitHub
```bash
git remote add origin https://github.com/USERNAME/NAMA-REPO.git
git push -u origin main
```

### 3. Alur setelah itu (setiap kali kerja)
```bash
# Cek status — file mana yang berubah?
git status

# Tambahkan semua perubahan
git add .

# Atau tambahkan file tertentu saja
git add notebooks/01_eksplorasi_data.ipynb

# Simpan perubahan dengan pesan yang jelas
git commit -m "add: regresi OLS untuk PDRB vs inflasi"

# Kirim ke GitHub
git push
```

---

## Perintah yang sering dipakai

| Perintah | Fungsi |
|----------|--------|
| `git status` | Lihat file mana yang berubah |
| `git log --oneline` | Lihat riwayat commit (ringkas) |
| `git diff` | Lihat detail perubahan yang belum di-commit |
| `git pull` | Ambil update terbaru dari GitHub |

---

## Tips commit message yang baik

Format yang direkomendasikan:

```
<tipe>: <deskripsi singkat>
```

Contoh tipe:
- `add:` menambahkan sesuatu yang baru
- `fix:` memperbaiki kesalahan
- `update:` memperbarui yang sudah ada
- `remove:` menghapus sesuatu

Contoh pesan yang **buruk**:
```
update
fix stuff
aaaaaa
```

Contoh pesan yang **baik**:
```
add: notebook eksplorasi data PDRB Jawa Timur 2019-2023
fix: koreksi perhitungan growth rate di script preprocessing
update: tambah visualisasi scatter plot inflasi vs pengangguran
```

---

## Kalau ada yang salah

```bash
# Batalkan perubahan yang belum di-commit (hati-hati, tidak bisa di-undo)
git checkout -- nama_file.py

# Lihat semua commit untuk menemukan versi yang benar
git log --oneline

# Kembali ke commit tertentu (hanya untuk lihat, tidak mengubah)
git checkout abc1234
```

---

## Referensi lanjutan

- [Pro Git Book (gratis)](https://git-scm.com/book/en/v2) — referensi paling lengkap
- [GitHub Skills](https://skills.github.com/) — tutorial interaktif resmi dari GitHub
- [Oh My Git!](https://ohmygit.org/) — game untuk belajar Git
