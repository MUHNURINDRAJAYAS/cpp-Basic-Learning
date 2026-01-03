# Mini Project C++

## CLI Linux Tool – Aplikasi Manajemen Data Sederhana

Mini project ini bertujuan melatih penggunaan **Variabel, Operator, Percabangan, Array, String, dan Function** dalam satu aplikasi **Command Line Interface (CLI)** di Linux.

Project ini **sangat cocok untuk portfolio GitHub pemula**.

---

## 1. Deskripsi Project

Aplikasi CLI sederhana untuk:

* Menampilkan menu
* Menambah data pengguna
* Menampilkan daftar data
* Menghitung rata-rata nilai
* Keluar dari program

📌 Contoh kasus: **Manajemen Nilai Siswa**

---

## 2. Fitur Aplikasi

* Menu interaktif (switch case)
* Input data menggunakan array
* Proses data menggunakan function
* Output rapi di terminal Linux

---

## 3. Struktur Folder Project

```
C++-CLI-Tool/
├── src/
│   └── main.cpp
├── README.md
```

---

## 4. Alur Program

1. Program menampilkan menu
2. User memilih menu
3. Program menjalankan fungsi sesuai pilihan
4. Program kembali ke menu sampai user keluar

---

## 5. Source Code Lengkap

```cpp
#include <iostream>
#include <string>
using namespace std;

const int MAX = 100;
string nama[MAX];
int nilai[MAX];
int jumlah = 0;

void tambahData() {
    cout << "Masukkan nama: ";
    cin.ignore();
    getline(cin, nama[jumlah]);

    cout << "Masukkan nilai: ";
    cin >> nilai[jumlah];

    jumlah++;
    cout << "Data berhasil ditambahkan!\n";
}

void tampilData() {
    if (jumlah == 0) {
        cout << "Belum ada data.\n";
        return;
    }

    for (int i = 0; i < jumlah; i++) {
        cout << i + 1 << ". " << nama[i] << " - " << nilai[i] << endl;
    }
}

void rataRata() {
    if (jumlah == 0) {
        cout << "Belum ada data.\n";
        return;
    }

    int total = 0;
    for (int i = 0; i < jumlah; i++) {
        total += nilai[i];
    }

    cout << "Rata-rata nilai: " << (float)total / jumlah << endl;
}

int main() {
    int pilihan;

    do {
        cout << "\n=== MENU ===\n";
        cout << "1. Tambah Data\n";
        cout << "2. Tampilkan Data\n";
        cout << "3. Hitung Rata-rata\n";
        cout << "4. Keluar\n";
        cout << "Pilih: ";
        cin >> pilihan;

        switch (pilihan) {
        case 1:
            tambahData();
            break;
        case 2:
            tampilData();
            break;
        case 3:
            rataRata();
            break;
        case 4:
            cout << "Keluar dari program." << endl;
            break;
        default:
            cout << "Pilihan tidak valid." << endl;
        }

    } while (pilihan != 4);

    return 0;
}
```

---

## 6. Cara Compile & Jalankan (Linux)

```bash
g++ src/main.cpp -o cli-tool
./cli-tool
```

---

## 7. Pengembangan Lanjutan (Opsional)

* Simpan data ke file (`fstream`)
* Login sederhana (username & password)
* Sorting nilai
* Validasi input

---

