# Materi C++ Dasar

## Array & String

Materi ini membahas **Array** dan **String** sebagai struktur data dasar dalam C++. Materi disusun untuk **project GitHub pembelajaran C++ dari dasar** dan cocok untuk pemula Linux / Termux.

---

## 1. Pengertian Array

Array adalah **kumpulan data dengan tipe yang sama** yang disimpan dalam satu variabel dan diakses menggunakan **index**.

📌 Index array dimulai dari **0**.

### Contoh:

```cpp
int nilai[5] = {80, 75, 90, 85, 70};
```

---

## 2. Deklarasi & Inisialisasi Array

### 2.1 Deklarasi Array

```cpp
int angka[3];
```

### 2.2 Inisialisasi Array

```cpp
int angka[3] = {10, 20, 30};
```

### 2.3 Mengakses Array

```cpp
cout << angka[0]; // output: 10
```

---

## 3. Array dengan Perulangan

Array sangat sering digunakan bersama **loop**.

```cpp
#include <iostream>
using namespace std;

int main() {
    int nilai[5] = {70, 75, 80, 85, 90};

    for (int i = 0; i < 5; i++) {
        cout << "Nilai ke-" << i << " = " << nilai[i] << endl;
    }

    return 0;
}
```

---

## 4. Array Input dari User

```cpp
#include <iostream>
using namespace std;

int main() {
    int angka[3];

    for (int i = 0; i < 3; i++) {
        cout << "Masukkan angka ke-" << i+1 << ": ";
        cin >> angka[i];
    }

    for (int i = 0; i < 3; i++) {
        cout << angka[i] << " ";
    }

    return 0;
}
```

---

## 5. Pengertian String

String digunakan untuk **menyimpan teks / kalimat**.

📌 Di C++ modern, gunakan `string` dari library `<string>`.

```cpp
#include <string>
string nama = "Indra";
```

---

## 6. Operasi Dasar String

### 6.1 Input String

```cpp
string nama;
getline(cin, nama);
```

### 6.2 Menggabungkan String

```cpp
string depan = "Linux";
string belakang = "User";
string hasil = depan + " " + belakang;
```

### 6.3 Panjang String

```cpp
cout << nama.length();
```

---

## 7. String vs Array of Char

| string             | char[]                 |
| ------------------ | ---------------------- |
| Mudah digunakan    | Lebih kompleks         |
| Aman dari overflow | Risiko error           |
| Disarankan pemula  | Digunakan level lanjut |

---

## 8. Contoh Program Lengkap

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string nama;
    int nilai[3];

    cout << "Masukkan nama: ";
    getline(cin, nama);

    for (int i = 0; i < 3; i++) {
        cout << "Masukkan nilai ke-" << i+1 << ": ";
        cin >> nilai[i];
    }

    cout << "Nama: " << nama << endl;
    cout << "Nilai: ";
    for (int i = 0; i < 3; i++) {
        cout << nilai[i] << " ";
    }

    return 0;
}
```

---

## 9. Latihan (Wajib Dicoba)

1. Program input 5 nama siswa (array string)
2. Cari nilai tertinggi dari array
3. Hitung rata-rata nilai

---

## 10. Struktur Folder GitHub

```
C++-Dasar/
├── 04-Array-String/
│   └── array_string.cpp
├── README.md
```

---

