---
title: Rangkaian Star Delta
nextjs:
  metadata:
    title: Rangkaian Star Delta
    description: Panduan rangkaian Star Delta.
---

## Dasar Motor Listrik

Motor listrik yang umum ada 2 jenis: 1-phase dan 3-phase. Perbedaan antara keduanya adalah motor listrik 1-phase memiliki 1 konduktor phase dan 1 konduktor netral. Sedangkan, motor listrik 3-phase memiliki 3 konduktor phase dan 1 konduktor netral. Konduktor phase pada motor 3-phase memiliki jarak phase yang sama dan bekerja bersamaan, sehingga butuh daya yang besar dan stabil.

Karena memiliki tiga konduktor fasa, motor listrik 3-phase memiliki daya yang lebih besar dan lebih stabil dibandingkan motor listrik 1-phase. Motor listrik 3-phase juga memiliki putaran yang lebih halus dan memiliki efisiensi yang lebih baik. Ini membuat motor listrik 3-phase lebih cocok untuk aplikasi industri yang membutuhkan daya yang besar dan stabil.

## Star X Delta

Delta:

- Arus (Ampere) besar
- Torsi besar (torsi berbanding lurus dengan arus)

Star:

- Arus kecil
- Torsi kecil

---

Motor 3 fasa akan mengambil arus besar saat dihubung delta, karena 3 lilitan yang ada padanya masing-masing akan menerima tegangan penuh 380 Volt.
{% figure src="/star-delta/rangkaiandelta.jpeg" alt="image" /%}

Sedangkan bila dihubung dengan rangkaian star, maka 2 lilitan akan saling tersambung seri/deret lalu keduanya menerima tegangan 380 Volt. Jadi tegangan 380 Volt dipakai untuk 2 lilitan.
{% figure src="/star-delta/rangkaianstar.jpeg" alt="image" /%}

Sampai disini akan diketahaui : arus saat hubungan delta akan lebih besar daripada saat hubungan star.

Kombinasi keduanya, star (mengurangi arus starting) & delta (torsi kerja besar) yang disebut Star/delta starter adalah solusi ekonomis (dibanding VSD, soft starter, dll) untuk suatu motor 3 phase.

{% figure src="/star-delta/star.jpeg" alt="image" /%}
{% figure src="/star-delta/delta.jpeg" alt="image" /%}
{% figure src="/star-delta/rangkaian.gif" alt="image" /%}

Kemudian, bila motor 3 fasa (terutama yang berdaya besar, lebih dari 2HP misalnya) disambung delta secara langsung (harusnya star, lalu motor berputar, kemudian delta), maka akan membahayakan motor, yaitu kekuatiran motornya terbakar. Kok bisa?, iya karena saat start arusnya akan 2x sampai 3x dari arus nominal. Untuk itulah saat start motor 3 fasa harus dihubung star dulu, lalu delta, agar motornya aman. Oya, andai motornya aman jaya, saat start akan menyebabkan penurunan tegangan yang cukup drastis. Untuk itu, cara menghubungkan yang benar seperti yang telah dijelaskan tersebut selain untuk mengamankan motor, juga agar tidak menyebabkan penurunan tegangan drastis saat motornya start, dimana itu akan menyebabkan lampu-lampu berkedip sesaat ketika motornya start.

## Perhitungan

{% quick-link title="Perhitungan" icon="installation" href="https://warstek.com/stardelta/"  /%}
