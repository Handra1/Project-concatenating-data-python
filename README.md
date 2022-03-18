# Project-concatenating-data-python
This project about learning concatenating data in python (In Indonesia)

Data mungkin tidak hanya ada dalam 1 file atau tabel monolitik untuk kita load (muat). Misalnya:
1. Dataset 5 juta baris dapat dipecah menjadi 5 dataset terpisah, masing-masing dengan sejuta baris. Hal tersebut digunakan untuk mempermudah penyimpanan dan sharing data.
2. Data baru setiap hari.
Hal terpenting dari kasus diatas yaitu untuk mengkombinasikan data tersebut dan membuatnya menjadi single dataset yang clean. Sehingga data tersebut bisa kita gunakan untuk melakukan analisis. Ketika kita ingin melakukan proses concatenation data, kita dapat menggabungkan 2 dataframes menjadi 1 dataframe.
Kita bisa melakukan proses concatenating data di pandas dengan menggunakan fungsi concat.
Sekarang kita memiliki 1 dataframe dengan gabungan dari 2 data tersebut. Dapat kita perhatikan juga jika hasil proses concatenating dataframe tetap menjaga original label index baris. Namun hal tersebut bisa menjadi konsekuensi ketika kita ingin menampilkan baris berdasarkan label index.
Jika kita menampilkan semua baris dengan kondisi index baris adalah 0, maka kita mendapatkan semua multiple baris. Disini saya menggunakan method loc untuk mendapatkan subset label index baris.
Agar tidak mendapatkan multiple rows seperti tadi, maka kita menambahkan parameter ignore_index=True pada saat proses penggunaan fungsi concat.
Maka sekarang kita memiliki penomoran label baris index yang beragam.
