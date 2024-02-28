# Golang
## const
Dua konsep yang sering digunakan bersama-sama dalam bahasa pemrograman Go: variabel konstan dan iota.

###Variabel Konstan:
Variabel konstan adalah variabel yang nilainya tetap dan tidak dapat diubah selama proses eksekusi program. Dalam Go, konstanta dideklarasikan menggunakan kata kunci `const`. Konstanta dapat didefinisikan untuk berbagai tipe data termasuk `string`, `integer`, dan `boolean`.

Contoh penggunaan variabel konstan dalam Go:

```go
package main

import "fmt"

const pi = 3.14
const aplikasi = "MyApp"

func main() {
    fmt.Println("Nilai Pi:", pi)
    fmt.Println("Nama Aplikasi:", aplikasi)
}
```

Pada contoh di atas, `pi` dan `aplikasi` adalah konstanta. Kedua nilai ini tidak dapat diubah selama eksekusi program.

###iota:
`iota` adalah konstanta bilangan bulat yang secara otomatis diinisialisasi dengan `0` pada setiap blok konstanta di Go. `iota` biasanya digunakan dalam deklarasi konstanta bersama dengan ekspresi aritmatika yang disederhanakan untuk memberikan nilai konstan secara berurutan.

Contoh penggunaan `iota` dalam Go:

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
    fmt.Println("Senin:", Senin)
    fmt.Println("Selasa:", Selasa)
    fmt.Println("Rabu:", Rabu)
    fmt.Println("Kamis:", Kamis)
    fmt.Println("Jumat:", Jumat)
    fmt.Println("Sabtu:", Sabtu)
    fmt.Println("Minggu:", Minggu)
}
```

Dalam contoh di atas, `iota` digunakan dalam blok konstanta untuk memberikan nilai yang berurutan secara otomatis mulai dari `0`. Kita hanya perlu mendeklarasikan `iota` sekali dalam blok konstanta, dan nilainya akan meningkat secara otomatis setiap kali kita mendeklarasikan konstanta baru.

Kombinasi penggunaan `iota` dengan blok konstanta dapat sangat berguna dalam kasus dimana ingin memberikan nilai konstan berurutan pada sekelompok variabel atau konstanta.