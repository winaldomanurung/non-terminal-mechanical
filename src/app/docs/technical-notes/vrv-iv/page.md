---
title: VRV-IV
nextjs:
  metadata:
    title: VRV-IV
    description: Catatan tentang VRV-IV.
---

## Component

{% figure src="/technical-work/vrv-iv/22.png" alt="image" /%}
{% figure src="/technical-work/vrv-iv/23.png" alt="image" /%}

### Inverter Fan

{% figure src="/technical-work/vrv-iv/1.jpg" alt="image" /%}

### Electronic expansion valve (Y1E)

{% figure src="/technical-work/vrv-iv/2.jpg" alt="image" /%}

**Cooling Operation**

- Fully close: 0 pulse (when thermostat OFF)
- Fully open: 3000 pulse (when thermostat ON)

### High pressure sensor

{% figure src="/technical-work/vrv-iv/3.jpg" alt="image" /%}

Digunakan untuk mencegah proses aktivasi proteksi ketika terjadinya kenaikan tidak wajar pada high pressure dan melindungi compressore dari kenaikan pressure yang bersifat lonjakan (transient).

{% figure src="/technical-work/vrv-iv/26.png" alt="image" /%}

Ketika pressure refrigerant dibawah 3.04 MPa maka akan dianggap normal. Namun, ketika pressure sudah melebihi 3.55 MPa, compressor akan dikurangi kapasitas kerjanya.

### Thermistor (subcooling heat exchanger gas pipe) (R6T)

{% figure src="/technical-work/vrv-iv/4.jpg" alt="image" /%}

Thermistor ini menggunakan type A dengan acuan resistansi sebagai berikut:

{% figure src="/technical-work/vrv-iv/28.png" alt="image" /%}

Dia merupakan thermistor type NTC, yang mana ketika temperature naik, resistance nya turun.

Dia diconnect dengan terminal X30A di wiring.

### Thermistor (heat exchanger liquid pipe) R4T

{% figure src="/technical-work/vrv-iv/5.jpg" alt="image" /%}

Thermistor ini menggunakan type A dengan acuan resistansi sebagai berikut:

{% figure src="/technical-work/vrv-iv/28.png" alt="image" /%}

Dia merupakan thermistor type NTC, yang mana ketika temperature naik, resistance nya turun.

Dia diconnect dengan terminal X30A di wiring.

### Thermistor (subcooling heat exchanger liquid pipe) (R5T)

{% figure src="/technical-work/vrv-iv/6.jpg" alt="image" /%}

Thermistor ini menggunakan type A dengan acuan resistansi sebagai berikut:

{% figure src="/technical-work/vrv-iv/28.png" alt="image" /%}

Dia merupakan thermistor type NTC, yang mana ketika temperature naik, resistance nya turun.

Dia diconnect dengan terminal X30A di wiring.

### Thermistor (suction pipe)

{% figure src="/technical-work/vrv-iv/7.jpg" alt="image" /%}

Thermistor ini menggunakan type A dengan acuan resistansi sebagai berikut:

{% figure src="/technical-work/vrv-iv/28.png" alt="image" /%}

Dia merupakan thermistor type NTC, yang mana ketika temperature naik, resistance nya turun.

Dia diconnect dengan terminal X30A di wiring.

### Thermistor (outdoor air)

{% figure src="/technical-work/vrv-iv/8.jpg" alt="image" /%}

Thermistor ini menggunakan type E dengan acuan resistansi sebagai berikut:

{% figure src="/technical-work/vrv-iv/24.png" alt="image" /%}

Dia merupakan thermistor type NTC, yang mana ketika temperature naik, resistance nya turun.

Dia diconnect dengan terminal X18A di wiring.

### Inverter fan 2

{% figure src="/technical-work/vrv-iv/9.jpg" alt="image" /%}

### High pressure switch (for M1C compressor) kanan

{% figure src="/technical-work/vrv-iv/10.jpg" alt="image" /%}

### High pressure switch (for M2C compressor) kiri

{% figure src="/technical-work/vrv-iv/11.jpg" alt="image" /%}

### Thermistor (M2C compressor body)

{% figure src="/technical-work/vrv-iv/12.jpg" alt="image" /%}

### Thermistor (M1C discharge pipe dan M2C discharge pipe)

{% figure src="/technical-work/vrv-iv/14.jpg" alt="image" caption="M1C discharge pipe" /%}

{% figure src="/technical-work/vrv-iv/13.jpg" alt="image" caption="M2C discharge pipe"/%}

Thermistor ini menggunakan type H dengan acuan resistansi sebagai berikut:

{% figure src="/technical-work/vrv-iv/24.png" alt="image" /%}

Dia merupakan thermistor type NTC, yang mana ketika temperature naik, resistance nya turun.

Dia diconnect dengan terminal X19A di wiring.

### Thermistor (M1C compressor body dicabut)

{% figure src="/technical-work/vrv-iv/15.jpg" alt="image" /%}

### Low pressure sensor

{% figure src="/technical-work/vrv-iv/16.jpg" alt="image" /%}

Digunakan untuk melindungi compressore dari penurunan pressure yang bersifat lonjakan (transient).

{% figure src="/technical-work/vrv-iv/29.png" alt="image" /%}

Ketika pressure refrigerant diatas 0.40 MPa maka akan dianggap normal. Namun, ketika pressure turun dibawah 0.35 MPa, compressor akan dikurangi kapasitas kerjanya.

### EEV injection

{% figure src="/technical-work/vrv-iv/17.jpg" alt="image" /%}

### Solenoid valve (oil return 1)

{% figure src="/technical-work/vrv-iv/18.jpg" alt="image" /%}

### Solenoid valve (oil return 2)

{% figure src="/technical-work/vrv-iv/19.jpg" alt="image" /%}

## Operasi

{% figure src="/technical-work/vrv-iv/20.png" alt="image" /%}

Kita mulai dari compressor. Disini ada dua buah compressor yang mana masing-masing punya **thermistor discharge** R21T dan R22T, yang mana berfungsi untuk mendetect temperature pipa discharge compressor, sebagai fungsi proteksi terhadap compressor.

Setelah melalui thermistor discharge, dia akan masuk ke **high pressure switch** S1PH dan S2PH. Switch ini digunakan untuk mencegah terjadinya overpressure. Jadi ketika ada error dan terjadi kenaikan pressure, dia akan memutus di 4MPa atau lebih, untuk melindungi compressor.

Jika lolos dari HPS, refrigerant akan melewati oil separator untuk dipisahkan dari oil yang tercampur dan melalui filter dan check valve. Selanjutnya dia akan masuk ke proteksi selanjutnya, yaitu **high pressure sensor** S1NPH, yang juga digunakan untuk mendeteksi high pressure.

Setelah melalui high pressure sensor, refrigerant akan didinginkan dengan menggunakan fan M1F dan M2F, dan akan dipantau oleh **thermistor outdoor air** R1T. Proses ini terjadi di condensing unit. Karena dia didinginkan, maka fase refrigerant yang tadinya gas akan berubah menjadi liquid.

Refrigerant kembali dipantau oleh **thermistor heat exchanger liquid pipe** R4T. Dia berfungsi untuk mendeteksi temperature dari liquid pipe dengan range jarak antara heat exchanger dan main EEV. Hasil pantauan ini akan digunakan untuk `menentukan jumlah refrigerant yang akan di-recover atau di-discharge oleh EEV dan juga mengatur ON/OFF thermostat` supaya temperature udara discharge sesuai dengan temperature yang diset user.

Setelahnya, refrigerant melewati filter dan masuk ke **electronic expansion valve (main)** Y1E, yang digunakan untuk mengatur flow rate dari refrigerant, dan mengatur SH control ketika mode cooling (fully open during cooling operation).

Next, refrigerant melewati `heat sink PCB`, dan setelahnya akan dicabang yaitu menuju **electronic expansion valve (secondary)** Y2E dan **double tube heat exchanger**.

Kita lanjut ke **double tube heat exchanger** dulu. Double tube heat exchanger ini digunakan untuk proses subcooling refrigerant liquid dari EEV (main).

Selanjutnya, refrigerant dipantau oleh **thermistor (subcooling heat exchanger liquid pipe)** R5T untuk mendeteksi temperature dari liquid pipe antara EEV (main) dan subcooling heat exchanger (double tube heat exchanger).

Selanjutnya, dia masuk ke filter dan stop valve sebelum akhirnya masuk ke **indoor unit**.

Di dalam indoor unit, refrigerant masuk ke filter dan **electronic expansion valve** untuk diturunkan suhu dan tekanannya, makanya dia berubah jadi biru.

Refrigerant akan keluar dari EEV dan melewati filter lagi sebelum ke heat exchanger (evaporator coil). Setelah mengambil panas ruangan, refrigerant akan menuju outoodr lagi, dan dipantau oleh **thermistor (suction pipe)** R3T untuk dideteksi temperaturenya.

---

Untuk cabang satunya lagi, **electronic expansion valve (secondary)**, yang mana digunakan untuk mengatur supaya **outlet superheated degree of `subcooling heat exchanger (double tube heat exchanger)` constant**.

Refrigeran akan masuk ke double tube heat exchanger dan bertukar kalor disana. Lalu refrigeran dipantau oleh **thermistor (subcooling heat exchanger gas pipe)** R6T, yang mana digunakan untuk mendeteksi temperature dari gas pipe di sisi evaporation side (keluaran) dari subcooling heat exchanger (double tube heat exchanger).

---

Disini refrigeran dari kedua cabang bergabung dan melwati filter sebelum masuk ke **low pressure sensor** S1NPL, yang digunakan untuk mendeteksi low pressure.

Setelahnya refrigerant akan menemui cabang yang akan digunakan untuk membagi refrigerant ke compressor 1 dan compressor 2 dan mengulangi siklus yang sama.

Disini juga ada **solenoid valve** Y3S dan Y4S yang mana digunakan untuk mengatur jumlah oil dari oil separator yang akan dialirkan kembali ke compressor.

{% figure src="/technical-work/vrv-iv/21.png" alt="image" /%}

## Wiring

{% figure src="/technical-work/vrv-iv/25.png" alt="image" /%}

## More Info

{% quick-links %}

{% quick-link title="Specification" icon="installation" href="https://drive.google.com/file/d/12iCQFlprJD2_PmTuOIRq3sDUqv1zufGE/view?usp=sharing"  /%}
{% quick-link title="Troubleshooting" icon="presets" href="https://drive.google.com/file/d/12lzPJneBJy_8FIwmx7Yy0WXFZcS-R3sS/view?usp=sharing"  /%}
{% quick-link title="Service Manual" icon="plugins" href="https://drive.google.com/file/d/12mfow8bRxNR5XJYno5B2eK9pFcMUI4WY/view?usp=sharing"  /%}
{% quick-link title="Error Code" icon="theming" href="https://drive.google.com/file/d/12ka9JfKgYX4Lo_QZsieSSXrXIRNv-9e3/view?usp=sharing"  /%}

{% /quick-links %}
