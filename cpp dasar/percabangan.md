# Materi C++ Dasar

## Percabangan (if, else, switch)

Materi ini membahas **percabangan logika** dalam C++, yaitu cara program **mengambil keputusan** berdasarkan kondisi tertentu. Materi ini cocok untuk **project GitHub pembelajaran C++ dari dasar**.

---

## 1. Pengertian Percabangan

Percabangan adalah struktur kontrol yang digunakan untuk **menentukan alur program** berdasarkan kondisi (true / false).

Contoh dalam kehidupan sehari-hari:

> Jika hujan → bawa payung, jika tidak → tidak bawa payung

---

## 2. Percabangan `if`

Digunakan ketika hanya ada **satu kondisi**.

### Sintaks:

```cpp
if (kondisi) {
    // kode dijalankan jika kondisi true
}
```

### Contoh:

```cpp
#include <iostream>
using namespace std;

int main() {
    int nilai = 80;

    if (nilai >= 75) {
        cout << "Lulus" << endl;
    }

    return 0;
}
```

---

## 3. Percabangan `if else`

Digunakan jika terdapat **dua kemungkinan kondisi**.

### Sintaks:

```cpp
if (kondisi) {
    // true
} else {
    // false
}
```

### Contoh:

```cpp
int nilai = 60;

if (nilai >= 75) {
    cout << "Lulus";
} else {
    cout << "Tidak Lulus";
}
```

---

## 4. Percabangan `if else if`

Digunakan jika terdapat **lebih dari dua kondisi**.

### Contoh:

```cpp
int nilai = 85;

if (nilai >= 90) {
    cout << "Grade A";
} else if (nilai >= 80) {
    cout << "Grade B";
} else if (nilai >= 70) {
    cout << "Grade C";
} else {
    cout << "Grade D";
}
```

---

## 5. Percabangan `switch case`

Digunakan untuk **banyak pilihan berdasarkan satu nilai**.

### Sintaks:

```cpp
switch (variabel) {
case nilai1:
    // kode
    break;
case nilai2:
    // kode
    break;
default:
    // kode
}
```

### Contoh:

```cpp
#include <iostream>
using namespace std;

int main() {
    int menu;
    cout << "1. Kopi\n2. Teh\nPilih menu: ";
    cin >> menu;

    switch (menu) {
    case 1:
        cout << "Anda memilih Kopi";
        break;
    case 2:
        cout << "Anda memilih Teh";
        break;
    default:
        cout << "Pilihan tidak tersedia";
    }

    return 0;
}
```

---

## 6. Perbedaan if else vs switch

| if else                    | switch                    |
| -------------------------- | ------------------------- |
| Kondisi kompleks           | Kondisi sederhana         |
| Bisa pakai operator logika | Tidak bisa pakai operator |
| Lebih fleksibel            | Lebih rapi untuk menu     |

---

## 7. Contoh Program Lengkap

```cpp
#include <iostream>
using namespace std;

int main() {
    int umur;
    cout << "Masukkan umur: ";
    cin >> umur;

    if (umur >= 17) {
        cout << "Boleh membuat SIM" << endl;
    } else {
        cout << "Belum boleh membuat SIM" << endl;
    }

    return 0;
}
```

---

## 8. Latihan (Wajib Dicoba)

1. Program cek ganjil / genap
2. Program cek nilai (A, B, C, D)
3. Program menu sederhana pakai switch

---

