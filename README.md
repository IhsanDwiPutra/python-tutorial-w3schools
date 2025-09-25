# Tutorial Python — W3Schools (0 → Pro)

**Deskripsi singkat**

Koleksi materi, catatan, dan latihan praktis yang saya susun berdasarkan pembelajaran dari W3Schools — disusun mulai dari level *dasar (0)* hingga *lanjutan (Pro)*. Tujuan repo ini adalah menjadi panduan belajar terstruktur yang bisa diikuti siapa saja yang ingin menguasai Python secara praktis dan sistematis.

**Status:** Work in progress · **Created:** 25 September 2025 · **Author:** Ihsan Dwi Putra

---

## Daftar Isi

1. [Tentang Repo ini](#tentang-repo-ini)
2. [Tujuan Pembelajaran & Sasaran Pembaca](#tujuan-pembelajaran--sasaran-pembaca)
3. [Cakupan Materi & Learning Roadmap](#cakupan-materi--learning-roadmap)
4. [Struktur Repository](#struktur-repository)
5. [Persiapan & Cara Menjalankan Contoh](#persiapan--cara-menjalankan-contoh)
6. [Konvensi Penulisan Kode & Standar kualitas](#konvensi-penulisan-kode--standar-kualitas)
7. [Kontribusi](#kontribusi)
8. [Changelog & Versi Awal](#changelog--versi-awal)
9. [License](#license)
10. [Kontak & Pengakuan](#kontak--pengakuan)

---

## Tentang Repo ini

Repo ini dibuat sebagai catatan terstruktur dan sumber latihan yang mengikuti materi Python dari W3Schools. Setiap topik diisi dengan penjelasan singkat, contoh kode sederhana, dan latihan/praktik yang bisa dikerjakan. Materi ditata sedemikian rupa agar pembaca dapat belajar langkah demi langkah dan memiliki bukti kemampuan (code examples, mini-projects) pada setiap tingkatannya.

**Kelebihan pendekatan ini:**

* Praktis: contoh langsung bisa dijalankan.
* Bertahap: dari konsep paling dasar hingga praktik lanjutan.
* Dilengkapi latihan: tiap topik ada soal/mini-task untuk dipraktikkan.

**Catatan:** Materi utama mengikuti struktur dan konten W3Schools, namun contoh dan latihan ditulis ulang agar sesuai gaya pembelajaran praktis dan lebih sesuai untuk proyek nyata.

---

## Tujuan Pembelajaran & Sasaran Pembaca

**Tujuan:**

* Mengantar pembaca dari tidak tahu sama sekali (level 0) menjadi mampu membangun aplikasi Python sederhana sampai menengah (Pro).
* Memberi keterampilan praktis yang bisa diaplikasikan pada tugas kuliah, proyek pribadi, dan portofolio.

**Sasaran pembaca:**

* Pemula tanpa pengalaman pemrograman sebelumnya.
* Programmer pemula yang ingin sistematis mempelajari Python.
* Mahasiswa atau self-learner yang mengikuti materi W3Schools dan ingin menyimpan catatan terstruktur.

---

## Cakupan Materi & Learning Roadmap

Berikut ringkasan roadmap yang ada dalam repo — tiap bagian berisi penjelasan singkat, contoh, latihan, dan referensi.

### Level 0 — Dasar (Introduction)

* **Dasar Python:** instalasi, menulis `hello world`, interpreter vs script.
* **Sintaks dasar:** variabel, tipe data (int, float, str, bool), operasi dasar.
* **Input/Output & formatting string.**

**Outcome:** Menjalankan skrip Python sederhana dan memahami tipe data dasar.

### Level 1 — Dasar Lanjutan

* **Kontrol alur:** `if`, `elif`, `else`, loop `for` dan `while`.
* **Collections dasar:** list, tuple, set, dict — operasi dasar, iterasi.
* **Fungsi dasar:** definisi, parameter, return, scope.

**Outcome:** Menulis program yang menggunakan branching, perulangan, dan fungsi sederhana.

### Level 2 — Intermediate

* **File I/O:** membaca/menulis file teks dan CSV.
* **Modules & Packages:** membuat modul sendiri, `import` dan struktur package.
* **Error & Exception handling.**
* **Working with JSON.**

**Outcome:** Membuat script yang memproses data sederhana dan modular.

### Level 3 — Object-Oriented Programming (OOP)

* **Class & Object**, enkapsulasi, pewarisan, polymorphism.
* **Magic methods** dan `__repr__` / `__str__`.

**Outcome:** Mendesain model data berbasis objek untuk aplikasi kecil.

### Level 4 — Lanjutan / Pro

* **Iterators, Generators, Decorators, Context Managers.**
* **Concurrency dasar:** `threading`, `asyncio` (pengantar).
* **Testing:** unittest / pytest.
* **Packaging & Distribusi:** `setup.py`, `pyproject.toml`, cara publish sederhana.
* **Perkenalan framework/web:** membuat REST API sederhana dengan Flask (opsional).

**Outcome:** Menulis kode Python yang lebih idiomatik, teruji, dan siap dipaketkan.

### Proyek Mini (Milestone)

Setiap akhir modul ada mini-project. Contoh milestone: CLI To-Do App, Contact Book (CRUD ke file/SQLite), Web Notes App (Flask, penyimpanan SQLite), dan proyek kecil untuk deployment.

---

## Struktur Repository (Disarankan)

Contoh struktur folder agar mudah dipahami dan dikembangkan:

```
tutorial-python-w3schools/      # root repo
├── README.md
├── LICENSE
├── requirements.txt
├── .gitignore
├── examples/                   # contoh kode per topik
│   ├── 01_basics/
│   │   └── hello.py
│   ├── 02_control_flow/
│   └── ...
├── exercises/                  # soal latihan terstruktur
├── projects/                   # mini-projects (milestone)
├── notebooks/                  # jupyter notebooks bila ada
├── notes/                      # ringkasan materi & catatan
└── tests/                      # test otomatis (pytest)
```

---

## Persiapan & Cara Menjalankan Contoh

Langkah singkat untuk mulai menggunakan repo ini di laptop:

1. **Clone repository**

```bash
git clone https://github.com/<username>/<repo-name>.git
cd <repo-name>
```

2. **Buat virtual environment (direkomendasikan)**

```bash
python3 -m venv .venv
# macOS / Linux
source .venv/bin/activate
# Windows
.venv\Scripts\activate
```

3. **Install dependency (jika ada)**

```bash
pip install -r requirements.txt
```

4. **Jalankan contoh**

Contoh menjalankan skrip:

```bash
python examples/01_basics/hello.py
```

5. **Menjalankan test** (apabila ada):

```bash
pytest
```

---

## Konvensi Penulisan Kode & Standar Kualitas

Agar konsisten dan profesional, gunakan standar berikut:

* **Format kode:** PEP8.
* **Formatter & Linter:** `black`, `flake8` (opsional but recommended).
* **Typing:** Gunakan type hints untuk fungsi penting.
* **Docstrings:** Setiap fungsi dan class penting harus memiliki docstring singkat (format Google atau NumPy style).
* **Commit message:** Ikuti *Conventional Commits* (contoh: `feat: tambah latihan control flow`, `fix: perbaiki README`).

Contoh docstring singkat:

```python
def add(a: int, b: int) -> int:
    """Return the sum of a and b.

    Args:
        a (int): first number
        b (int): second number

    Returns:
        int: hasil penjumlahan
    """
    return a + b
```

---

## Cara Berkontribusi

Jika ingin menambah materi atau memperbaiki konten:

1. Fork repo ini.
2. Buat branch baru bernama `feat/<deskripsi-singkat>` atau `fix/<deskripsi>`.
3. Lakukan perubahan, tambahkan test bila perlu.
4. Commit dengan pesan yang jelas; gunakan bahasa Indonesia atau Inggris sesuai konteks.
5. Push ke fork kamu dan buat Pull Request (PR) ke branch `main` repo ini.

**Catatan reviewer:** Jelaskan perubahan singkat di deskripsi PR, sertakan contoh input/output jika relevan.

---

## Changelog & Versi Awal

* **v0.1 — 25 September 2025** — Inisialisasi repository: README awal, struktur direktori, beberapa contoh dasar.

Perubahan besar akan dicatat di sini secara kronologis.

---

## License

Lisensi default yang disarankan: **MIT License**. Silakan ganti sesuai kebutuhan organisasi atau preferensi pribadi. Tambahkan file `LICENSE` di root repo.

---

## Kontak & Pengakuan

**Dibuat oleh:** Ihsan Dwi Putra
**Tanggal pembuatan:** 25 September 2025

**Sumber utama referensi:** Materi dasar diambil dan diselaraskan dari W3Schools (diedit ulang untuk keperluan latihan dan penjelasan yang lebih praktis).

---

## Tips untuk Pembaca & Reviewer

* Mulai dari folder `examples/01_basics` dan jalankan satu per satu.
* Kerjakan latihan di `exercises/` — buktikan pemahaman dengan mengunggah solusi ke `projects/`.
* Gunakan virtual environment setiap sesi agar dependency tidak bercampur.
* Coba lakukan code review kecil pada setiap PR: tujuan utama adalah belajar menulis kode yang bersih dan terdokumentasi.

---

Terima kasih sudah melihat repo ini. Jika Anda (atau saya sendiri) ingin menambahkan badge, GitHub Actions untuk testing, atau template issue/PR — bisa saya tambahkan selanjutnya.
