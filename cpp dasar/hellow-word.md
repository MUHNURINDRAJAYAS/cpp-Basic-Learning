# hello word

Repository ini berisi materi **C++ dari dasar** untuk pemula.  
Cocok untuk:
- 🎓 Mahasiswa
- 🐧 Pengguna Linux & Termux

---

📂 Struktur Folder

```teks
├── hello-word.cpp
├── komentar.cpp
└── input-output.cpp
```
🐧 Pengguna Linux & Termux
```teks
nano hello-word.cpp
```
setelah itu masukan source code lalu save dengan 
menekan Ctrl+x-y-Enter/ok

📥 Source Code (hello-word.cpp)

```cpp
#include <iostream>
using namespace std;
int main() {
    cout << "Hello World C++!" << endl;
    return 0;
}
```
setelah itu compile file nano yg sudah di buat tadi dengan perintah :
```teks
g++ hello-word.cpp hello-word
./hello-word
```

📤 Output

```cpp
Hello World C++!
