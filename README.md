# Implementasi Algoritma Dijkstra pada Python

Algoritma Dijkstra adalah algoritma serakah yang digunakan untuk menemukan jalur terpendek dari satu simpul sumber ke semua simpul lainnya dalam sebuah graf berbobot. Grafik dapat berarah atau tidak berarah, siklik atau asiklik, tetapi bobot pada semua sisinya harus nonnegatif.

## Langkah-langkah:

### 1. Inisialisasi:
- Buatlah set sptSet untuk melacak simpul-simpul yang sudah termasuk dalam pohon jalur terpendek. Mulailah dengan set kosong.
- Tetapkan jarak ke semua simpul sebagai INFINITE. Jarak simpul sumber diset ke 0.

### 2. Iterasi:

- Selama sptSet tidak mencakup semua simpul:
  - Pilih simpul u yang tidak berada di sptSet dan memiliki jarak minimum.
  - Tambahkan u ke sptSet.
  - Perbarui jarak semua simpul yang berdekatan dengan u:
    - Untuk setiap simpul v yang berdekatan dengan u, jika jarak(u) + bobot(u, v) < jarak(v), maka perbarui jarak(v) menjadi jarak(u) + bobot(u, v).

## Ilustrasi:
![image](https://user-images.githubusercontent.com/22562694/120260452-8d455d80-c2b3-11eb-9d84-6b8b46dffc2c.png)

Gambar di atas menunjukkan contoh algoritma Dijkstra yang bekerja.
- `a` adalah simpul sumber.
- Jarak ke semua simpul lainnya dari sumber diberi label tak terhingga positif.
- Bobot sisi ditandai dengan warna hijau muda.

## Output:
```
The shortest distance of  a  from the source vertex a is: 0
The shortest distance of  b  from the source vertex a is: 3
The shortest distance of  c  from the source vertex a is: 3.5
The shortest distance of  d  from the source vertex a is: 4.5
```

## Kesimpulan:
Algoritma Dijkstra adalah alat yang ampuh untuk menemukan jalur terpendek dalam graf berbobot. Algoritmanya efisien dan mudah diterapkan. Algoritma ini memiliki banyak aplikasi di berbagai bidang seperti sistem navigasi, routing jaringan, dan analisis data.
