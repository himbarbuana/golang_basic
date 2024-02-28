# Golang
## Data Type

Mendeklarasikan variabel dengan berbagai jenis tipe data. Berikut adalah beberapa tipe data yang bisa digunakan untuk mendeklarasikan variabel di Go:

### 1. Integer Types:

* `int`: Bilangan bulat dengan tanda. Ukuran spesifik tergantung pada platform.

* `int8`, `int16`, `int32`, `int64`: Bilangan bulat dengan tanda dan ukuran tertentu (`8`, `16`, `32`, atau `64` bit).

* `uint`: Bilangan bulat tanpa tanda. Ukuran spesifik tergantung pada platform.

* `uint8`, `uint16`, `uint32`, `uint64`, `uintptr`: Bilangan bulat tanpa tanda dengan ukuran tertentu (`8`, `16`, `32`, `64` bit, atau ukuran pointer).

### 2. Floating Point Types:

* `float32`, `float64`: Bilangan pecahan (desimal) dengan ukuran tertentu (32 atau 64 bit).

### 3. Complex Types:

* `complex64`, `complex128`: Bilangan kompleks dengan bagian real dan imajiner. Masing-masing menggunakan `float32` atau `float64`.

### 4. Boolean Type:

* `bool`: Nilai boolean, `true` atau `false`.

### 5. String Type:

* `string`: Urutan karakter.

### 6. Pointer Types:

* `*T`: Pointer ke tipe `T`.

### 7. Array Types:

* `[n]T`: Array dengan panjang tertentu `n` yang berisi elemen dari tipe `T`.

### 8. Slice Types:

* `[]T`: Slice (potongan) dari elemen-elemen tipe `T`.

### 9. Struct Types:

* `struct`: Kumpulan nilai yang berbeda, setiap nilai memiliki nama (field) yang berbeda.

### 10. Map Types:

* `map[K]V`: Penyajian pasangan kunci-nilai, di mana `K` adalah tipe kunci dan `V` adalah tipe nilai.

### 11. Function Types:

* `func`: Tipe data yang mewakili fungsi.

### 12. Interface Types:

* `interface`: Tipe data yang mendefinisikan kumpulan metode, tetapi tidak memiliki implementasi.

### 13. Channel Types:

* `chan T`: Channel untuk komunikasi antara goroutine.

### 14. Untyped Types:

* `nil`: Nilai default dari `pointer`, `channel`, dan beberapa tipe lainnya.

Berbagai tipe data ini, dapat digunakan membuat variabel untuk menyimpan berbagai jenis data dalam program Go.





