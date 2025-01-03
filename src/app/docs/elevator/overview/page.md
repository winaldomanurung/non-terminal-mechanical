---
title: Lift
nextjs:
  metadata:
    title: Lift
    description: Catatan tentang Lift.
---

## Layout

### Railink

{% quick-links %}
{% quick-link title="Lift Railink (1)" icon="theming" href="https://drive.google.com/file/d/1ohXQNZO4bNXs1X6ffKIBMcfqCTzpTbS0/view?usp=sharing"  /%}
{% quick-link title="Lift Railink (2)" icon="theming" href="https://drive.google.com/file/d/1mrOwc8iYrkFPSjpnbCKjsO5ERbaAJgxc/view?usp=sharing"  /%}
{% quick-link title="Lift Railink (3)" icon="theming" href="https://drive.google.com/file/d/1PJ5hBCJnluPAFp09r18Ys51fzyH8jvIP/view?usp=sharing"  /%}
{% quick-link title="Lift Railink (4)" icon="theming" href="https://drive.google.com/file/d/1Xrw_Yck5Zy3FTmpdgnM1du4qZgUWg9ES/view?usp=sharing"  /%}
{% /quick-links %}

## Wiring

### Contactor

{% quick-links %}
{% quick-link title="Wiring (KLS-MCU)" icon="theming" href="https://drive.google.com/file/d/12qBy0lLUiCYztl9MH5vxjEZl2U0_CbLn/view?usp=sharing"  /%}
{% quick-link title="Port (KLS-MCD)" icon="theming" href="https://drive.google.com/file/d/1K0BR6OZ-6HeIqkXdnQIhmMgB0zqwWjf3/view?usp=drive_link"  /%}
{% quick-link title="Door Operator" icon="theming" href="https://drive.google.com/file/d/1BCdU4hxki5MCvTxuiZOHnFlLruPrrQfI/view?usp=drive_link"  /%}
{% quick-link title="Inverter" icon="theming" href="https://drive.google.com/file/d/13lGPsa_O6eb7_EOC4SucEFqFMK4b8joU/view?usp=sharing"  /%}
{% /quick-links %}

{% figure src="/lift/1.png" alt="image" /%}

Disini digunakan 4 contactor dengan tegangan coil 110 VDC.

- KMB (Main): Schneider LC1D09FD
- KAD (Safety): Schneider LC1D09FD
- KMF (Brake): CAD32FD
- KMY (Motor): Schneider LC1D09FD

Saat lift berjalan:

- KMB energized **95VDC**
- KAD energized **95VDC**
- KMF energized **98VDC**
- KMY energized **95VDC**

Saat lift berhenti/standby:

- KMB not energized
- KAD energized **95VDC**
- KMF not energized
- KMY not energized

### Main Control Board

<!-- {% figure src="/lift/13.png" alt="image" /%} -->

{% figure src="/lift/2.png" alt="image" /%}
{% figure src="/lift/8.png" alt="image" /%}

{% figure src="/lift/3.png" alt="image" /%}
{% figure src="/lift/12.png" alt="image" /%}

{% figure src="/lift/4.png" alt="image" /%}
{% figure src="/lift/10.png" alt="image" /%}

{% figure src="/lift/5.png" alt="image" /%}
{% figure src="/lift/7.png" alt="image" /%}

{% figure src="/lift/6.png" alt="image" /%}
{% figure src="/lift/9.png" alt="image" /%}

<!-- {% figure src="/lift/11.png" alt="image" /%} -->

### Main Control Interface Board

Main Control Interface Board ini merupakan penghubung komponen lain dengan Main Control Board. LED-LED yang ada di dalam Main Control Board (yang diawali dengan X) juga commandnya dari sini:

| LED | Usage                                     | Responsibility |
| --- | ----------------------------------------- | -------------- |
| X0  | Not found                                 | -              |
| X1  | Not found                                 | -              |
| X2  | Slow UP (Perintah UP inspection)          | -              |
| X3  | Slow DOWN (Perintah DOWN inspection)      | -              |
| X4  | UP single-floor forced slow               | -              |
| X5  | DOWN single-floor forced slow             | -              |
| X6  | UP leveling                               | -              |
| X7  | DOWN leveling                             | -              |
| X8  | Motor power supply detection              | T4.2 (Line350) |
| X9  | Band-type brake contactor detection       | T4.3 (Line351) |
| X10 | Left band-type brake switch detection     | T4.5 (Line352) |
| X11 | Right band-type brake switch detection    | T4.6 (Line353) |
| X12 | Motor temperature detection               | -              |
| X13 | Door area signal detection                | -              |
| X14 | Advance opening relay detection           | -              |
| X15 | Fire returning switch                     | -              |
| X16 | Emergency leveling input                  | -              |
| X17 | Door lock relay detection                 | T4.4 (Line322) |
| X18 | UP double-floor forced slow               | -              |
| X19 | DOWN double-floor forced slow             | -              |
| X20 | Safety circuit detection                  | -              |
| X21 | Rear car door lock circuit                | -              |
| X22 | Landing door lock                         | -              |
| X23 | Seal contactor input                      | -              |
| X24 | Bypass detection                          | -              |
| X25 | Rope head weighing full load detection    | -              |
| X26 | Rope head weighing over load detection    | -              |
| X27 | Earthquake                                | -              |
| X28 | Not Found                                 | -              |
| X29 | Not Found                                 | -              |
| X20 | Not Found                                 | -              |
| X31 | Not Found                                 | -              |
| X32 | Not Found                                 | -              |
| X33 | Not Found                                 | -              |
| X34 | Not Found                                 | -              |
| X35 | Rear landing door lock circuit            | -              |
| X36 | Another way high pressure detection point | -              |

### Trafo

{% figure src="/lift/35.jpg" alt="image" /%}

### Noise Filter

{% figure src="/lift/36.jpg" alt="image" /%}

### Door Operator / Inverter

- Model: PM-DCU004
  {% figure src="/lift/14.jpg" alt="image" /%}

### Junction Box

- Board: KLS-TCD-01A
  {% figure src="/lift/15.jpg" alt="image" /%}
  {% figure src="/lift/klstcd.png" alt="image" /%}

- Emergency Lighting Power Supply
  {% figure src="/lift/16.jpg" alt="image" /%}

- Relay KAE
  {% figure src="/lift/17.jpg" alt="image" /%}

- Terminal
  {% figure src="/lift/18.jpg" alt="image" /%}

### Sensor Levelling

{% figure src="/lift/19.jpg" alt="image" /%}
{% figure src="/lift/20.jpg" alt="image" /%}

### Main Sheave

{% figure src="/lift/21.jpg" alt="image" /%}
{% figure src="/lift/27.jpg" alt="image" /%}
{% figure src="/lift/39.jpg" alt="image" /%}

Di main sheave ini, disambungkan kabel mekanisme brake manual
{% figure src="/lift/24.jpg" alt="image" /%}
{% figure src="/lift/25.jpg" alt="image" /%}
{% figure src="/lift/26.jpg" alt="image" /%}

### Sling Door

Ukuran 4mm
{% figure src="/lift/22.jpg" alt="image" /%}
{% figure src="/lift/23.jpg" alt="image" /%}

### Guide Shoe

Bisa dikencangkan dari baut (geser) atau dengan menyetting spring.
{% figure src="/lift/28.png" alt="image" /%}
{% figure src="/lift/28.jpg" alt="image" /%}
{% figure src="/lift/30.jpg" alt="image" /%}

### Counterweight

{% figure src="/lift/31.jpg" alt="image" /%}

### Limit Switch

{% figure src="/lift/32.jpg" alt="image" /%}
{% figure src="/lift/33.jpg" alt="image" /%}

### Buffer Car

{% figure src="/lift/34.jpg" alt="image" /%}

### Manual Brake

{% figure src="/lift/37.jpg" alt="image" /%}

### Fuse

{% figure src="/lift/38.jpg" alt="image" /%}

### Sling

Mati - Counterweight - Main Sheave - Pulley Bawah 1 - Pulley Bawah 2 - Mati

## Dasar Operasi

Supaya lift bisa bekerja, harus ditemukan `signal normal` yang mana dipenuhi dengan:

- Safety
- Komunikasi luar dan dalam
- Pintu luar dan dalam

### Safety

Disini kita harus cek apakah semua safety sudah terbaca dengan baik.

Case terakhir adalah safety brake di main sheave itu lemah. Dia menyebabkan `signal normal` berubah menjadi `signal fault`, tapi ga ditampilkan di dalam LED MCB. Jadi, misal ada case seperti ini, coba cek untuk brake switch di main sheave atau safety governor.

### Komunikasi Luar dan Dalam

Ini bisa kita lihat dari LED MCB yaitu CAN1 dan CAN2. Kita pastikan bahwa keduanya berkedip cepat.

<!-- | LED | Usage     | Responsibility |
| --- | --------- | -------------- |
| X0  | Not found | -              |
| X1  | Not found | -              | -->

### Pintu Luar dan Dalam

Ini kita lihat dari LED MCB DL dan HDL. DL itu untuk door dalam dan HDL untuk door luar.

## Operasi Maintenance LED KLS-MCD-01A

## Operasi Normal LED KLS-MCD-01A

### Standby lantai 1

| X0  | X1  | X4  | X6  | X7  | X17 |
| --- | --- | --- | --- | --- | --- |

### Standby lantai 2

| X0  | X1  | X4  | X5  | X6  | X7  | X17 |
| --- | --- | --- | --- | --- | --- | --- |

### Standby lantai 3

| X0  | X1  | X5  | X6  | X7  | X17 |
| --- | --- | --- | --- | --- | --- |

### Lantai 1 > Lantai 2

Belum

### Lantai 1 > Lantai 3

Belum

### Lantai 2 > Lantai 3

| X0  | X1  | X4  | X5  | X8  | X9  | X10 | X11 | X17 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |

### Lantai 2 > Lantai 1

Belum

### Lantai 3 > Lantai 1

| X0  | X1  | X4  | X5  | X8  | X9  | X10 | X11 | X17 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |

### Lantai 3 > Lantai 2

| X0  | X1  | X4  | X5  | X8  | X9  | X10 | X11 | X17 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |

### Buka Pintu Lantai 1

### Buka Pintu Lantai 2

| X0  | X1  | X4  | X5  | X6  | X7  |
| --- | --- | --- | --- | --- | --- |

### Buka Pintu Lantai 3

| X0  | X1  | X5  | X6  | X7  |
| --- | --- | --- | --- | --- |

## Operasi Fuse

- QF1: **97 VAC**
- QF2: **110 VAC**
- QF3: **15 VDC**

## Do's and Don'ts

### Do's

- Ada alternatif untuk menyalakan signal XLed, yaitu dengan jumper. Caranya adalah dengan jumper LED apa yang mau kita nyalakan dengan COM nya. Misal kita mau nyalakan X8, maka kita cari port yang responsible dengan X8 (T4.2) dan lakukan jumper dengan COM (T4.1).

### Don'ts

- Kita pernah coba bypass contactor KMB, KAD, KMF, dan KMY. Hal ini mengakibatkan car bablas naik ke atas.
  {% figure src="/lift/39.png" alt="image" /%}

## Istilah

- Car door: Pintu dalam
- Landing door: Pintu luar

| Istilah         | Arti              |
| --------------- | ----------------- |
| Car door        | Pintu dalam       |
| Landing door    | Pintu luar        |
| Band-type brake | Main sheave brake |
