## Perulangan (Looping)

Materi ini membahas **Perulangan (Looping)** dalam C++, yaitu teknik untuk **menjalankan kode secara berulang** selama kondisi tertentu terpenuhi. Materi ini disusun untuk **project GitHub pembelajaran C++ dari dasar**.

---

## 1. Pengertian Perulangan

Perulangan adalah struktur kontrol yang digunakan untuk **mengulang eksekusi kode** tanpa harus menulis kode yang sama berulang-ulang.

Contoh kehidupan nyata:

> Selama lampu merah → berhenti

---

## 2. Jenis-Jenis Perulangan di C++

C++ memiliki 3 jenis perulangan utama:

1. `for`
2. `while`
3. `do while`

---

## 3. Perulangan `for`

Digunakan jika **jumlah perulangan sudah diketahui**.

### Sintaks:

```cpp
for (inisialisasi; kondisi; increment) {
    // kode
}
```

### Contoh:

```cpp
#include <iostream>
using namespace std;

int main() {
    for (int i = 1; i <= 5; i++) {
        cout << "Perulangan ke-" << i << endl;
    }
    return 0;
}
```

---

## 4. Perulangan `while`

Digunakan jika **jumlah perulangan belum diketahui**.

### Sintaks:

```cpp
while (kondisi) {
    // kode
}
```

### Contoh:

```cpp
int i = 1;
while (i <= 5) {
    cout << i << endl;
    i++;
}
```

---

## 5. Perulangan `do while`

Mirip `while`, tetapi **kode dijalankan minimal satu kali**.

### Sintaks:

```cpp
do {
    // kode
} while (kondisi);
```

### Contoh:

```cpp
int i = 1;
do {
    cout << i << endl;
    i++;
} while (i <= 5);
```

---

## 6. Perintah `break` dan `continue`

### `break`

Menghentikan perulangan.

```cpp
for (int i = 1; i <= 10; i++) {
    if (i == 5)
        break;
    cout << i << endl;
}
```

### `continue`

Melewati satu iterasi.

```cpp
for (int i = 1; i <= 5; i++) {
    if (i == 3)
        continue;
    cout << i << endl;
}
```

---

## 7. Perulangan Bersarang (Nested Loop)

Perulangan di dalam perulangan.

```cpp
for (int i = 1; i <= 3; i++) {
    for (int j = 1; j <= 3; j++) {
        cout << "(" << i << "," << j << ") ";
    }
    cout << endl;
}
```

---

## 8. Perulangan dengan Array

```cpp
int nilai[3] = {70, 80, 90};

for (int i = 0; i < 3; i++) {
    cout << nilai[i] << endl;
}
```

---

## 9. Contoh Program Lengkap

```cpp
#include <iostream>
using namespace std;

int main() {
    int pilihan;

    do {
        cout << "\n1. Cetak Angka 1-5" << endl;
        cout << "2. Keluar" << endl;
        cout << "Pilih: ";
        cin >> pilihan;

        if (pilihan == 1) {
            for (int i = 1; i <= 5; i++) {
                cout << i << " ";
            }
            cout << endl;
        }

    } while (pilihan != 2);

    return 0;
}
```

---

## 10. Latihan (Wajib Dicoba)

1. Cetak bilangan genap 1–20
2. Hitung jumlah bilangan 1–100
3. Buat menu looping sederhana

---

