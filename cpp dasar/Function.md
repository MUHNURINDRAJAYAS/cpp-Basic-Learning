## Function (Fungsi)

Materi ini membahas **Function (Fungsi)** dalam C++, yaitu cara memecah program menjadi bagian-bagian kecil agar **rapi, mudah dibaca, dan mudah dikembangkan**. Materi ini disusun untuk **project GitHub pembelajaran C++ dari dasar**.

---

## 1. Pengertian Function

Function adalah **blok kode** yang dapat dipanggil untuk menjalankan tugas tertentu.

Keuntungan menggunakan function:

* Program lebih **terstruktur**
* Kode bisa **digunakan ulang**
* Mudah **debugging & maintenance**

---

## 2. Struktur Dasar Function

### Sintaks:

```cpp
tipe_kembalian namaFunction(parameter) {
    // kode
    return nilai;
}
```

### Contoh:

```cpp
int tambah(int a, int b) {
    return a + b;
}
```

---

## 3. Function Tanpa Parameter

```cpp
#include <iostream>
using namespace std;

void salam() {
    cout << "Hello C++!" << endl;
}

int main() {
    salam();
    return 0;
}
```

---

## 4. Function dengan Parameter

```cpp
#include <iostream>
using namespace std;

void cetakNama(string nama) {
    cout << "Nama: " << nama << endl;
}

int main() {
    cetakNama("Indra");
    return 0;
}
```

---

## 5. Function dengan Nilai Kembalian

```cpp
#include <iostream>
using namespace std;

int luasPersegi(int sisi) {
    return sisi * sisi;
}

int main() {
    cout << luasPersegi(5);
    return 0;
}
```

---

## 6. Function Prototype

Prototype digunakan jika function ditulis **di bawah fungsi main()**.

```cpp
#include <iostream>
using namespace std;

int tambah(int a, int b); // prototype

int main() {
    cout << tambah(3, 4);
    return 0;
}

int tambah(int a, int b) {
    return a + b;
}
```

---

## 7. Function dengan Array

```cpp
#include <iostream>
using namespace std;

void tampilArray(int arr[], int size) {
    for (int i = 0; i < size; i++) {
        cout << arr[i] << " ";
    }
}

int main() {
    int data[] = {1, 2, 3, 4, 5};
    tampilArray(data, 5);
    return 0;
}
```

---

## 8. Function dengan String

```cpp
#include <iostream>
#include <string>
using namespace std;

string cekStatus(int nilai) {
    if (nilai >= 75)
        return "Lulus";
    else
        return "Tidak Lulus";
}

int main() {
    cout << cekStatus(80);
    return 0;
}
```

---

## 9. Scope Variabel

* **Variabel Lokal** → hanya berlaku di dalam function
* **Variabel Global** → bisa diakses semua function

```cpp
int global = 10;

void tampil() {
    int lokal = 5;
}
```

---

## 10. Contoh Program Lengkap

```cpp
#include <iostream>
using namespace std;

int tambah(int a, int b);

int main() {
    int x = 10, y = 20;
    cout << "Hasil: " << tambah(x, y);
    return 0;
}

int tambah(int a, int b) {
    return a + b;
}
```

---

## 11. Latihan (Wajib Dicoba)

1. Function menghitung keliling & luas
2. Function cek ganjil / genap
3. Function rata-rata array

---

