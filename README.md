# Pertemuan 03 Seleksi Python
Nama: Siti Rohmah
NIM: 2225250203
Kelas: 3A
## Tujuan
1.	Seleksi if untuk di gunakan untuk membuat keputusan berdasarkan kondisi benar apakah suatu bilangan bernilai Ganjil atau genap.
2.	Seleksi if-else di gunakan ketika tepat satu dari dua alternatif harus di jalankan. Cabang if berjalan saat kondisi True dan cabang else berjalan  saat kondisi False. Contohnya saat menentukan bilangan Ganjil dan genap.
3.	Kondisi majemuk di gunakan ketika menggabungkan dua kondisi atau lebih kondisi sederhana. Kondisi ini menggunakan operator logika (and, or, not). Contohnya saat menentukan kelulusan bersyarat.
4.	Nested if adalah struktur if di dalam cabang if atau else. Digunakan ketika pemeriksaan kedua hanya masuk akal setelah hasil pemeriksaan pertama di ketahui. Contohnya saat membandingkan dua bilangan.
## cara menjalankan
print("Analisis Persamaan Kuadrat")
a = float(input("Koefisien a: "))
b = float(input("Koefisien b: "))
c = float(input("Koefisien c: "))
if a == 0:
    print("Bukan persamaan kuadrat.")
else:
    diskriminan = b ** 2 - 4 * a * c
    print(f"Diskriminan = {diskriminan:.2f}")

    if diskriminan > 0:
        x1 = (-b + diskriminan ** 0.5) / (2 * a)
        x2 = (-b - diskriminan ** 0.5) / (2 * a)
        print(f"Persamaan kuadrat memiliki dua akar real: x1 = {x1:.2f}, x2 = {x2:.2f}")
    elif diskriminan == 0:
        x = -b / (2 * a)
        print(f"Persamaan kuadrat memiliki satu akar real: x = {x:.2f}")
    else:
        print("Persamaan kuadrat tidak memiliki akar real.")

## Algoritma tugas
1. Baca a, b, dan c sebagai float.
2. Periksa apakah a sama dengan 0.
3. Jika a bukan 0, hitung D = b ** 2 - 4 * a * c.
4. Periksa apakah D lebih besar dari 0.
5. Jika tidak, periksa apakah D sama dengan 0; selain itu D negatif.

## Hasil Pengujian
* 01_genap_ganjil.py.
Masukkan bilangan bulat: 8
8 adalah bilangan genap.
Masukkan bilangan bulat: 13
13 adalah bilangan ganjil.
Masukkan bilangan bulat: 0
0 adalah bilangan genap.
Masukkan bilangan bulat: -7
-7 adalah bilangan ganjil.
* 02_bandingkan_dua_bilangan.py.
Bilangan pertama: 7
Bilangan kedua: 4
Bilangan pertama lebih besar.
Bilangan pertama: 2
Bilangan kedua: 9
Bilangan pertama lebih kecil.
Bilangan pertama: 5
Bilangan kedua: 5
Kedua bilangan sama.
Bilangan pertama: -3
Bilangan kedua: -8

* 03_kelulusan_bersyarat.py.
Nilai akhir: 75
Kehadiran (%): 90
Lulus
Nilai akhir: 59
Kehadiran (%): 90
Belum lulus
Nilai akhir: 75
Kehadiran (%): 79
Belum lulus
Nilai akhir: 60
Kehadiran (%): 80
Lulus

* 04_jenis_segitiga.py.
Sisi a: 3
Sisi b: 3
Sisi c: 3
Segitiga sama sisi
Sisi a: 5
Sisi b: 5
Sisi c: 8
Segitiga sama kaki
Sisi a: 3
Sisi b: 4
Sisi c: 5
Segitiga sembarang
Sisi a: 1
Sisi b: 2
Sisi c: 3
Ketiga sisi tidak membentuk segitiga

* tugas/analisis_persamaan_kuadrat.py.
Analisis Persamaan Kuadrat
Koefisien a: 1
Koefisien b: -5
Koefisien c: 6
Diskriminan = 1.00
Persamaan kuadrat memiliki dua akar real: x1 = 3.00, x2 = 2.00
Analisis Persamaan Kuadrat
Koefisien a: 1
Koefisien b: 2
Koefisien c: 1
Diskriminan = 0.00
Persamaan kuadrat memiliki satu akar real: x = -1.00
Analisis Persamaan Kuadrat
Koefisien a: 1
Koefisien b: 0
Koefisien c: 1
Diskriminan = -4.00
Persamaan kuadrat tidak memiliki akar real.
Analisis Persamaan Kuadrat
Koefisien a: 0
Koefisien b: 2
Koefisien c: 3
Bukan persamaan kuadrat.

## Refleksi
Setelah melakukan praktik/latihan, kesalahan logika yang saya temukan yaitu Indentation Error, itu terjadi karena saya tidak menambahkan spasi (tidak menjorok ke dalam) pada baris kode setelah if.
