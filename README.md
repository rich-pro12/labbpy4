# labbpy4

Richie Pranata

312410451

TI.24.A.5

``` pyhton
def hitung_nilai_akhir(tugas, uts, uas):
    """Menghitung nilai akhir berdasarkan bobot yang ditentukan."""
    return (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)
```
Tujuan: Fungsi ini digunakan untuk menghitung nilai akhir mahasiswa berdasarkan nilai tugas, UTS (Ujian Tengah Semester), dan UAS (Ujian Akhir Semester).
Parameter:

tugas: Nilai tugas mahasiswa.

uts: Nilai UTS mahasiswa.

uas: Nilai UAS mahasiswa.

Proses: Menghitung nilai akhir dengan rumus yang sudah ditentukan, di mana tugas memiliki bobot 30%, UTS 35%, dan UAS 35%.

Return: Mengembalikan nilai akhir yang dihitung.

```pyhton
def tampilkan_header():
    """Menampilkan header tabel dengan format yang lebih menarik"""
    print("\n" + "=" * 93)
    print(f"|{'| DAFTAR NILAI MAHASISWA |':^91}|")
    print("=" * 93)
    print(f"| {'NO':<4} | {'NAMA':<12} | {'NIM':<20} | {'TUGAS':<8} | {'UTS':<8} | {'UAS':<8} | {'NILAI AKHIR':<10} |")
    print("=" * 93)
```
Tujuan: Menampilkan header tabel yang akan digunakan untuk menampilkan data mahasiswa.

Output: Menggunakan karakter = untuk membuat batas tabel dan menampilkan nama kolom dalam format yang teratur.

Format: Menggunakan f-string untuk mengatur lebar kolom agar lebih mudah dibaca.

```pyhton
def tampilkan_data_mahasiswa(data_mahasiswa):
    """Menampilkan data mahasiswa dalam format tabel"""
    for index, mahasiswa in enumerate(data_mahasiswa, start=1):
        print(f"| {index:<4} | {mahasiswa['Nama']:<12} | {mahasiswa['NIM']:<20} | "
              f"{mahasiswa['Tugas']:<8.2f} | {mahasiswa['UTS']:<8.2f} | {mahasiswa['UAS']:<8.2f} | "
              f"{mahasiswa['Nilai Akhir']:<10.2f}  |")
    print("=" * 93)
```
Tujuan: Menampilkan data mahasiswa dalam format tabel.

Parameter:data_mahasiswa: List yang berisi dictionary dengan data mahasiswa.

Proses: Menggunakan enumerate untuk mendapatkan indeks dan data mahasiswa, kemudian mencetak data dengan format yang teratur.

Output: Menampilkan setiap mahasiswa dengan nilai tugas, UTS, UAS, dan nilai akhir, serta menambahkan batas tabel di akhir.

# flowchart
[foto!]()
