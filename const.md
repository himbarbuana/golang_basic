# Golang
## Variabel Konstan
Variabel konstan, atau biasa disebut sebagai konstanta, adalah variabel di dalam Go yang nilainya tetap dan tidak dapat diubah selama program berjalan. Konstanta digunakan untuk menyimpan nilai yang diketahui pada saat kompilasi dan tidak diharapkan berubah selama eksekusi program. Dalam Go, konstanta dideklarasikan menggunakan kata kunci `const`.

Berikut adalah cara mendefinisikan dan menggunakan variabel konstan dalam Go:

Mendefinisikan Variabel Konstan:

Konstanta dideklarasikan menggunakan kata kunci `const` diikuti dengan nama konstan, tipe data opsional, dan nilai konstan.

```go
const namaKonstan = nilai
```

Contoh:

```go
const pi = 3.14
const hariDalamSeminggu = 7
```

### Tipe Data Konstan:

Jika tipe data tidak disediakan secara eksplisit, Go akan menentukan tipe data konstan secara otomatis berdasarkan nilai yang diberikan.

### Penggunaan Konstan:
Konstan dapat digunakan di seluruh program dengan cara yang sama seperti variabel biasa.

Contoh:

```go
package main

import "fmt"

const pi = 3.14

func main() {
    fmt.Println("Nilai pi:", pi)
}
```

### Penggunaan Konstan dengan Tipe Data Enumerasi:
Dalam Go, konstan juga dapat digunakan untuk membuat enumerasi dengan menggunakan iota.

```go
package main

import "fmt"

const (
    Senin = iota
    Selasa
    Rabu
    Kamis
    Jumat
    Sabtu
    Minggu
)

func main() {
    fmt.Println("Hari ini adalah hari ke", Senin+1)
}
```

Dalam contoh di atas, `Senin`, `Selasa`, dan seterusnya merupakan konstanta yang diurutkan dengan nilai awal `0` dan meningkat secara bertahap dengan setiap konstanta berikutnya karena penggunaan `iota`.

### Keuntungan Variabel Konstan:
1. Ketegasan Nilai: 
   - Konstanta menyediakan nilai yang tetap dan tidak dapat diubah, sehingga meningkatkan kejelasan dan keamanan program.

2. Efisiensi Kompilasi: 
   - Nilai konstan ditentukan selama kompilasi, sehingga tidak ada overhead untuk menentukan nilainya selama runtime.
Dengan menggunakan variabel konstan, Anda dapat menyimpan nilai-nilai yang tetap dan memastikan bahwa nilai-nilai tersebut tidak akan berubah selama eksekusi program, meningkatkan kejelasan dan keamanan program Anda.
