# Golang
## Integer Types:
Berikut adalah daftar lengkap dari tipe data integer yang tersedia dalam bahasa pemrograman Go:

| Tipe Data   | Deskripsi                                                 |
|-------------|-----------------------------------------------------------|
| int         | Integer berukuran 32-bit di platform 32-bit, dan 64-bit di platform 64-bit. Jumlah bitnya bisa berbeda tergantung pada platform.                                    |
| int8        | Integer berukuran 8-bit yang mampu menyimpan nilai antara -128 hingga 127.                     |
| int16       | Integer berukuran 16-bit yang mampu menyimpan nilai antara -32768 hingga 32767.               |
| int32       | Integer berukuran 32-bit yang mampu menyimpan nilai antara -2147483648 hingga 2147483647.      |
| int64       | Integer berukuran 64-bit yang mampu menyimpan nilai antara -9223372036854775808 hingga 9223372036854775807. |
| uint        | Integer tanpa tanda berukuran 32-bit di platform 32-bit, dan 64-bit di platform 64-bit. Jumlah bitnya bisa berbeda tergantung pada platform.                       |
| uint8       | Integer tanpa tanda berukuran 8-bit yang mampu menyimpan nilai antara 0 hingga 255.          |
| uint16      | Integer tanpa tanda berukuran 16-bit yang mampu menyimpan nilai antara 0 hingga 65535.       |
| uint32      | Integer tanpa tanda berukuran 32-bit yang mampu menyimpan nilai antara 0 hingga 4294967295.  |
| uint64      | Integer tanpa tanda berukuran 64-bit yang mampu menyimpan nilai antara 0 hingga 18446744073709551615. |
| uintptr     | Tipe bilangan bulat tanpa tanda yang cukup besar untuk menyimpan nilai dari alamat memori.   |

Dengan menggunakan tipe data integer yang sesuai, untuk menyimpan nilai bilangan bulat dengan presisi dan rentang yang dibutuhkan oleh aplikasi.

Contoh:

```go
package main

import (
    "fmt"
    "math"
)

func main() {
    // int
    var numInt int = 42
    fmt.Println("int:", numInt)

    // int8
    var numInt8 int8 = -128
    fmt.Println("int8:", numInt8)

    // int16
    var numInt16 int16 = -32768
    fmt.Println("int16:", numInt16)

    // int32
    var numInt32 int32 = -2147483648
    fmt.Println("int32:", numInt32)

    // int64
    var numInt64 int64 = -9223372036854775808
    fmt.Println("int64:", numInt64)

    // uint
    var numUint uint = 4294967295
    fmt.Println("uint:", numUint)

    // uint8
    var numUint8 uint8 = 255
    fmt.Println("uint8:", numUint8)

    // uint16
    var numUint16 uint16 = 65535
    fmt.Println("uint16:", numUint16)

    // uint32
    var numUint32 uint32 = 4294967295
    fmt.Println("uint32:", numUint32)

    // uint64
    var numUint64 uint64 = 18446744073709551615
    fmt.Println("uint64:", numUint64)

    // uintptr
    var numUintptr uintptr = math.MaxUintptr
    fmt.Println("uintptr:", numUintptr)
}
```