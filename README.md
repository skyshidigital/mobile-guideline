### PT. Skyshi Digital Indonesia
##### Jl. Tampomas No. 9, Trihanggo, Kec. Gamping,
##### Kab. Sleman, Daerah Istimewa Yogyakarta, Indonesia, 55291.
##### Phone : (0274) 4547428, Email : hello@skyshi.com 

# Mobile Guideline 

## Daftar Isi
- [Penanganan Slow Performance large image Menggunakan React Native](#penanganan-slow-performance-large-image-menggunakan-react-native)
- [Penanganan Splash Screen Pada Android iOS React Native](#penanganan-splash-screen-pada-android-ios-react-native)
- [Penggunanan Empty State pada Android iOS React Native](#penggunanan-empty-state-pada-android-ios-react-native)

    
### Penanganan Slow Performance large image Menggunakan React Native
Apabila aplikasi menampilkan halaman yang mengandung image 
- <p align="justify">Gunakan react-native-fastimage https://github.com/DylanVann/react-native-fast-image untuk men-cache image secara otomatis</p>
- <p align="justify">Tampilkan image dengan ukuran sesuai kebutuhan di sebuah halaman</p>
- <p align="justify">Pindahkan image yang besar ke halaman yang berbeda, contoh ada images di sebuah halaman detil produk, jika ingin melihat detil image lebih besar, maka harus klik dulu image tersebut dan kemudian tampilkan image yang lebih besar di halaman yang berbeda</p>

### Penanganan Splash Screen Pada Android iOS React Native
Penanganan untuk menghindari Splash screen yang blocking (terdapat glitch putih yang disebabkan karena menggunakan 2 splash screen level Native dan React Native). Yaitu dengan penanganan sebagai berikut :
- Initial Route disarankan untuk tidak memiliki beberapa kondisi. Hindari Initial Route, contoh: `Jika user telah login akan di route ke screen A, Jika user belum login akan di route ke screen B.`
- masing-masing OS splash screennya pakai Native dan tambahan library. Referensi mengenai splash screen menggunakan react native : https://github.com/crazycodeboy/react-native-splash-screen

### Penggunanan Empty State pada Android iOS React Native
- Selalu gunakan Empty State untuk setiap components atau sections ketika proses memuat data belum selesai
- Pada halaman homescreen direkomendasikan untuk menggunakan halaman placeholder untuk tiap components atau sections. contoh seperti lampiran berikut: https://prnt.sc/orjsjw, https://prnt.sc/orjt0d

