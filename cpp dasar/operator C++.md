# Materi C++ Dasar

## Operator C++

Materi ini merupakan lanjutan dari **Variabel & Tipe Data** dan disusun untuk **project GitHub pembelajaran C++ dari dasar**.

---

## 1. Pengertian Operator

Operator adalah **simbol khusus** yang digunakan untuk melakukan operasi terhadap satu atau lebih operand (nilai / variabel).

Contoh:

```cpp
int hasil = 10 + 5;
```

`+` adalah operator, `10` dan `5` adalah operand.

---

## 2. Jenis-Jenis Operator C++

### 2.1 Operator Aritmatika

Digunakan untuk operasi matematika.

| Operator | Fungsi      | Contoh |
| -------- | ----------- | ------ |
| +        | Penjumlahan | a + b  |
| -        | Pengurangan | a - b  |
| *        | Perkalian   | a * b  |
| /        | Pembagian   | a / b  |
| %        | Sisa bagi   | a % b  |

#### Contoh Program:

```cpp
#include <iostream>
using namespace std;

int main() {
    int a = 10, b = 3;

    cout << a + b << endl;
    cout << a - b << endl;
    cout << a * b << endl;
    cout << a / b << endl;
    cout << a % b << endl;

    return 0;
}
```

---

### 2.2 Operator Assignment (Penugasan)

Digunakan untuk memberikan nilai ke variabel.

| Operator | Contoh | Arti         |
| -------- | ------ | ------------ |
| =        | a = 5  | a bernilai 5 |
| +=       | a += 2 | a = a + 2    |
| -=       | a -= 2 | a = a - 2    |
| *=       | a *= 2 | a = a * 2    |
| /=       | a /= 2 | a = a / 2    |

---

### 2.3 Operator Perbandingan (Relasional)

Menghasilkan nilai **true** atau **false**.

| Operator | Fungsi                  | Contoh |
| -------- | ----------------------- | ------ |
| ==       | Sama dengan             | a == b |
| !=       | Tidak sama              | a != b |
| >        | Lebih besar             | a > b  |
| <        | Lebih kecil             | a < b  |
| >=       | Lebih besar sama dengan | a >= b |
| <=       | Lebih kecil sama dengan | a <= b |

#### Contoh:

```cpp
int a = 10, b = 5;
bool hasil = a > b;
```

---

### 2.4 Operator Logika

Digunakan untuk menggabungkan kondisi.

| Operator | Nama | Fungsi                |    |                            |
| -------- | ---- | --------------------- | -- | -------------------------- |
| &&       | AND  | True jika semua benar |    |                            |
|          |      |                       | OR | True jika salah satu benar |
| !        | NOT  | Membalik nilai        |    |                            |

#### Contoh:

```cpp
int umur = 20;
bool punyaSIM = true;

if (umur >= 17 && punyaSIM) {
    cout << "Boleh mengemudi";
}
```

---

### 2.5 Operator Increment & Decrement

Digunakan untuk menambah atau mengurangi nilai 1.

| Operator | Contoh | Arti      |
| -------- | ------ | --------- |
| ++       | a++    | a = a + 1 |
| --       | a--    | a = a - 1 |

#### Contoh:

```cpp
int a = 5;
a++;
--a;
```

---

### 2.6 Operator Ternary

Operator singkat untuk **if else**.

Format:

```cpp
kondisi ? nilai_true : nilai_false;
```

#### Contoh:

```cpp
int nilai = 80;
string hasil = (nilai >= 75) ? "Lulus" : "Tidak Lulus";
```

---

## 3. Contoh Program Lengkap

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    int a = 10, b = 5;

    cout << "Penjumlahan : " << a + b << endl;
    cout << "Perbandingan a > b : " << (a > b) << endl;

    bool login = true;
    cout << "Status Login : " << !login << endl;

    int nilai = 70;
    string status = (nilai >= 75) ? "Lulus" : "Tidak Lulus";
    cout << "Status : " << status << endl;

    return 0;
}
```

---

## 4. Latihan (Disarankan)

1. Buat kalkulator sederhana (+, -, *, /)
2. Cek bilangan genap atau ganjil
3. Cek lulus / tidak lulus dari nilai input

---

