## Variabel & Tipe Data

Repository ini berisi materi **C++** untuk pemula.  
Cocok untuk:
- 🎓 Mahasiswa
- 🐧 Pengguna Linux & Termux

---

## 1. Pengertian Variabel

Variabel adalah **tempat untuk menyimpan data** di dalam program. Setiap variabel memiliki:

* **Nama variabel**
* **Tipe data**
* **Nilai**

### Contoh sederhana:

```cpp
int umur = 20;
```

Artinya:

* `int`  → tipe data
* `umur` → nama variabel
* `20`   → nilai

---

## 2. Aturan Penamaan Variabel

✅ Boleh:

* Huruf (a-z, A-Z)
* Angka (0-9) *(tidak boleh di awal)*
* Garis bawah `_`

❌ Tidak boleh:

* Spasi
* Karakter khusus (`@`, `#`, `%`, dll)
* Kata kunci C++ (`int`, `return`, `if`, dll)

### Contoh benar:

```cpp
int nilai;
int nilai_akhir;
int nilai2;
```

### Contoh salah:

```cpp
int 2nilai;   // salah
int nilai akhir; // salah
```

---

## 3. Tipe Data Dasar C++

### 3.1 Integer (`int`)

Digunakan untuk bilangan bulat.

```cpp
int angka = 10;
```

### 3.2 Float (`float`)

Digunakan untuk bilangan desimal.

```cpp
float berat = 55.5;
```

### 3.3 Double (`double`)

Bilangan desimal dengan presisi lebih tinggi.

```cpp
double phi = 3.14159;
```

### 3.4 Character (`char`)

Digunakan untuk **1 karakter**.

```cpp
char huruf = 'A';
```

### 3.5 Boolean (`bool`)

Digunakan untuk nilai **true / false**.

```cpp
bool isLogin = true;
```

### 3.6 String (`string`)

Digunakan untuk teks / kalimat.

```cpp
#include <string>
string nama = "Indra";
```

---

## 4. Contoh Program Lengkap

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    int umur = 20;
    float tinggi = 170.5;
    char grade = 'A';
    bool isMahasiswa = true;
    string nama = "Indra";

    cout << "Nama        : " << nama << endl;
    cout << "Umur        : " << umur << endl;
    cout << "Tinggi      : " << tinggi << endl;
    cout << "Grade       : " << grade << endl;
    cout << "Mahasiswa   : " << isMahasiswa << endl;

    return 0;
}
```

---

## 5. Tabel Ringkas Tipe Data

| Tipe Data | Fungsi                 | Contoh  |
| --------- | ---------------------- | ------- |
| int       | Bilangan bulat         | 10      |
| float     | Desimal                | 3.5     |
| double    | Desimal presisi tinggi | 3.14159 |
| char      | 1 karakter             | 'A'     |
| bool      | True / False           | true    |
| string    | Teks                   | "Hello" |

---

## 6. Latihan (Wajib Dicoba)

1. Buat program input nama & umur
2. Hitung umur + 5 tahun
3. Tampilkan hasil ke layar

---

## 7. Struktur Folder GitHub (Rekomendasi)

```
C++-Dasar/
├── 01-Variabel-TipeData/
│   └── variabel.cpp
├── README.md
```

---


