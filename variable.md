# Golang
## Variable
Variabel digunakan untuk menyimpan dan memanipulasi data. Setiap variabel memiliki tipe data tertentu yang menentukan jenis data yang dapat disimpan di dalamnya. Di Go (Golang), untuk mendeklarasikan variabel bisa dengan menggunakan kata kunci `var`, diikuti dengan nama variabel dan tipe datanya. Berikut adalah cara membuat variabel di Go:

### 1. Deklarasi Variabel Tunggal:

Mendeklarasikan variabel tunggal dengan cara: 

```go
var namaVariabel tipeData
```

Contoh:

```go 
var nama string
```

```go 
var umur int
```

### 2. Inisialisasi Variabel:

Inisialisasi variabel merujuk pada memberikan nilai awal kepada variabel pada saat variabel tersebut dideklarasikan. Ini adalah langkah penting dalam penggunaan variabel karena memberikan nilai awal memungkinkan variabel untuk memiliki nilai yang telah ditetapkan sebelum digunakan dalam program.

Dalam beberapa bahasa pemrograman, seperti Go, inisialisasi variabel dapat dilakukan bersamaan dengan deklarasi variabel atau setelah variabel dideklarasikan.

Mendeklarasikan dan langsung menginisialisasi variabel dengan nilai awal menggunakan tanda sama dengan `(=)`. 

Berikut adalah contoh inisialisasi variabel dalam Go:


```go
var namaVariabel tipeData = nilai
```

Contoh:

```go
var nama string = "Himbar"
```

```go
package main

import "fmt"

func main() {
    // Inisialisasi variabel bersamaan dengan deklarasi
    var umur int = 17
    fmt.Println("Umur:", umur)

    // Inisialisasi variabel setelah deklarasi
    var nama string
    nama = "Himbar"
    fmt.Println("Nama:", nama)
}
```

Pada contoh tersebut, variabel `umur` diinisialisasi bersamaan dengan deklarasinya dengan nilai `17`, sementara variabel `nama` diinisialisasi setelah dideklarasikan dengan nilai `"Himbar"`. Dalam kedua kasus tersebut, variabel memiliki nilai awal yang telah ditetapkan sebelum digunakan dalam program.

### 3. Deklarasi dan Inisialisasi Tanpa Tipe Data:
Go memiliki kemampuan untuk menentukan tipe data secara otomatis berdasarkan nilai yang diberikan (inferensi tipe). Ini dapat digunakan dalam kasus inisialisasi variabel tanpa menyebutkan tipe datanya.

```go
var namaVariabel = nilai
```

Contoh:

```go
var umur = 25
```

Menggunakan sintaks pendek untuk mendeklarasikan dan menginisialisasi variabel tanpa menyertakan tipe datanya secara eksplisit. Hal ini disebut sebagai `"type inference"` atau `"penalaran tipe"`. Dalam kasus ini, tipe data variabel akan ditentukan oleh kompilator berdasarkan nilai yang diberikan.

Berikut adalah contoh deklarasi dan inisialisasi variabel tanpa tipe data secara eksplisit dalam Go:

```go
package main

import "fmt"

func main() {
    // Pendeklarasian dan inisialisasi variabel tanpa tipe data
    nama := "Himbar Buana"
    umur := 17
    
    fmt.Println("Nama:", nama)
    fmt.Println("Umur:", umur)
}
```

Dalam contoh di atas, tipe data dari variabel `nama` akan ditentukan sebagai `string` berdasarkan nilai `"Himbar Buana"`, sedangkan tipe data dari variabel `umur` akan ditentukan sebagai `int` berdasarkan nilai `17`.

Pendeklarasian dan inisialisasi variabel tanpa tipe data secara eksplisit dapat membuat kode menjadi lebih ringkas dan mudah dibaca. Namun, penggunaannya sebaiknya dibatasi pada kasus-kasus dimana tipe data variabel dapat dengan jelas ditentukan dari nilai yang diberikan.

### 4. Pendeklarasian Singkat (Short Variable Declaration):
Go juga mendukung pendeklarasian singkat, dengan menggunakan `:=` untuk mendeklarasikan dan menginisialisasi variabel secara singkat.

Dengan menggunakan sintaks ini, bisa mendeklarasikan variabel baru dan menginisialisasinya dengan nilai tertentu dalam satu baris kode tanpa perlu menyertakan tipe data secara eksplisit. Go akan menentukan tipe data variabel secara otomatis berdasarkan nilai yang diberikan.

Berikut adalah contoh penggunaan Short Variable Declaration dalam Go:

```go
namaVariabel := nilai
```

Contoh:

```go
nama := "Himbar"
```

Pendeklarasian singkat hanya bisa digunakan dalam fungsi, dan tidak untuk variabel global.

### 5. Variabel Konstan:
Konstan adalah variabel yang nilainya tetap dan tidak dapat diubah setelah diberikan nilai awal. Mendeklarasikan variabel konstan menggunakan kata kunci `const`:

```go
const namaVariabel tipeData = nilai
```

Contoh:

```go
const pi = 3.14

```

### 6. Multiple Variable Declaration:
Mendeklarasikan beberapa variabel sekaligus dengan tipe data yang sama:

```go
var (
    namaVariabel1 tipeData
    namaVariabel2 tipeData
    ...
)
```

Contoh:

```go
var (
    umur int
    tinggi float64
)
```

### 7. Variabel Blank Identifier (_):

Variabel blank identifier `(_)` digunakan ketika ingin membuang nilai yang tidak diperlukan. Ini digunakan saat membutuhkan nilai kembali tetapi tidak ingin menggunakannya:

```go
_ = nilai
```

Contoh:

```go
_, err := fungsiYangMengembalikanDuaNilai()
```

### 8. Merubah Nilai Variable
Mengubah nilai variabel dengan cara memberikan nilai baru ke variabel tersebut. Dalam Go, untuk melakukan ini caranya cukup sederhana. Berikut adalah contoh cara mengubah nilai variabel:

```go
package main

import "fmt"

func main() {
    // Deklarasi dan inisialisasi variabel
    var nama string = "Himbar"
    fmt.Println("Nama awal:", nama)
    
    // Mengubah nilai variabel
    nama = "Buana"
    fmt.Println("Nama setelah diubah:", nama)
}

```


### 9. Contoh:

```go
package main

import "fmt"

func main() {
    // Deklarasi variabel
    var nama string
    var umur int
    
    // Inisialisasi variabel
    nama = "Himbar Buana"
    umur = 17
    
    // Mendeklarasikan dan menginisialisasi variabel
    var pekerjaan = "Programmer (Aamiin)"
    
    // Pendeklarasian dan inisialisasi singkat
    kota := "Bandung"
    
    // Menampilkan nilai variabel ke dalam console
    fmt.Println("Nama:", nama)
    fmt.Println("Umur:", umur)
    fmt.Println("Pekerjaan:", pekerjaan)
    fmt.Println("Kota:", kota)
}
```
