---
title: Kontaktor
nextjs:
  metadata:
    title: Kontaktor
    description: Panduan belajar kontaktor.
---

## Catatan

Untuk type tegangan coil kontaktor Schneider AC:

- B7 = 24 VAC
- D7 = 42 VAC
- E7 = 48 VAC
- F7 = 110 VAC
- M7 = 220 VAC
- Q7 = 380 VAC

Untuk type tegangan coil kontaktor Schneider DC:

- BL = 24 VDC
- FD = 110 VDC
- MD = 220 VDC

Kenapa tegangan coil ini menjadi penting? Karena misal coil 220V dan 380V itu berbeda tegangan kerjanya dan juga jumlah lilitan kawatnya berbeda.

Misal `LC1D50AM7`. Artinya ini adalah kontaktor dengan type 50 Ampere dan tegangan coilnya 220V AC.

## Cara Cek Kondisi Kontaktor

Dasar:

- Cek nyambung: Hambatan sekitar 200 Ohm
- Cek tidak nyambung: Hambatan 0 Ohm

### Buka baut kontaktor

{% figure src="/kontaktor/1.png" alt="image" /%}

### Cabut coil kontaktor

{% figure src="/kontaktor/2.png" alt="image" /%}

### Cek kondisi coil (gulungan contactor)

Pertama-tama kita cek fisik coil (yang dilapis solasi putih), apakah ada tanda-tanda kebakar.
{% figure src="/kontaktor/3.png" alt="image" /%}
Kalau tidak ada tanda-tanda kebakar, maka cek coil dengan menggunakan ohmmeter. Kalau ternyata ada hambatan sekitar 200 Ohm berarti bagus.
{% figure src="/kontaktor/4.png" alt="image" /%}

### Cek koneksi antara pole A1 dan A2 dengan sambungan ke coil

Kita cek A2 dulu.
{% figure src="/kontaktor/5.png" alt="image" /%}
Kita cek A1.
{% figure src="/kontaktor/6.png" alt="image" /%}
Pastikan sambungan terkonek.
{% figure src="/kontaktor/7.png" alt="image" /%}

## What do you learn?

- Coil dites dengan menggunakan hambatan. Kenapa ga dites dengan menggunakan kontinuitas? Kontinuitas digunakan untuk mengecek sambungan langsung, misal koneksi kabel atau pole NC ke NC ketika tidak energized. Sedangkan coil merupakan beban, dia tidak diukur dengan kontinuitas. Namanya beban, dia merupakan load yang diukur dengan Ohm.
- Cara menentukan ukuran kontaktor itu intinya dari Ampere:
  {% figure src="/kontaktor/8.png" alt="image" /%}
- Penggunaan kontaktor dalam rangkaian star-delta
  {% figure src="/kontaktor/9.png" alt="image" /%}
  {% figure src="/kontaktor/10.png" alt="image" /%}
