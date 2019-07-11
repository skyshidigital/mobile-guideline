Mobile Guideline 
=================

### Daftar Isi

- [Penanganan Slow Performance large image Menggunakan React Native](#penanganan-slow-performance-large-image-menggunakan-react-native)
    
### Penanganan Slow Performance large image Menggunakan React Native
Apabila aplikasi menampilkan halaman yang mengandung image 
- <p align="justify">Gunakan react-native-fastimage https://github.com/DylanVann/react-native-fast-image untuk men-cache image secara otomatis</p>
- <p align="justify">Tampilkan image dengan ukuran sesuai kebutuhan di sebuah halaman</p>
- <p align="justify">Pindahkan image yang besar ke halaman yang berbeda, contoh ada images di sebuah halaman detil produk, jika ingin melihat detil image lebih besar, maka harus klik dulu image tersebut dan kemudian tampilkan image yang lebih besar di halaman yang berbeda</p>
