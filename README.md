# 💰 Kalkulator Subsidi BUDI95

Kalkulator web mudah untuk mengira penjimatan subsidi petrol RON95 di bawah program BUDI95 kerajaan Malaysia.

## Tentang

Aplikasi ini membantu pengguna memahami berapa banyak wang yang mereka jimatkan dengan subsidi BUDI95 dengan membandingkan harga petrol bersubsidi dan tidak bersubsidi.

## Ciri-ciri

- 💵 Kira penjimatan dengan subsidi kerajaan
- 📊 Perbandingan harga (bersubsidi vs tidak bersubsidi vs kadar lama)
- 🎯 Butang jumlah pantas (RM 10 - RM 60)
- 📱 Responsif untuk semua saiz skrin
- ⚡ Tidak memerlukan sambungan internet selepas dimuat turun

## Cara Guna

1. Buka fail `budi95-calculator.html` dalam pelayar web
2. Masukkan jumlah bayaran dalam RM atau klik butang jumlah pantas
3. Lihat hasil kiraan:
   - Liter yang anda dapat
   - Jumlah penjimatan dengan subsidi
   - Perbandingan harga

## Kadar Harga Semasa

- **Dengan Subsidi (BUDI95)**: RM 1.99/L
- **Tanpa Subsidi**: RM 2.60/L
- **Kadar Lama**: RM 2.05/L

## Teknologi

- HTML5
- CSS3 (dengan gradient dan animasi)
- Vanilla JavaScript (tiada dependency)

## Pemasangan

Tiada pemasangan diperlukan. Hanya muat turun fail `budi95-calculator.html` dan buka dalam pelayar web moden (Chrome, Firefox, Safari, Edge).

## Kemaskini Harga

Jika kadar subsidi berubah, edit nilai pemalar dalam fail HTML (baris 254-256):

```javascript
const PRICE_SUBSIDIZED = 1.99;      // Harga bersubsidi
const PRICE_NON_SUBSIDIZED = 2.60;  // Harga tanpa subsidi
const PRICE_OLD_RATE = 2.05;        // Kadar lama
```

## Lesen

Projek sumber terbuka untuk kegunaan awam.
