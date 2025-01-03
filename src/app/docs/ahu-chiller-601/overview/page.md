---
title: AHU Note
nextjs:
  metadata:
    title: AHU Note
    description: Catatan tentang AHU.
---

## Layout dan Gambar

### Layout System 602

{% figure src="/ahu-chiller-601/1.png" alt="image" /%}

### Compressor Chiller

{% figure src="/ahu-chiller-601/2.jpg" alt="image" /%}

{% figure src="/ahu-chiller-601/3.jpg" alt="image" /%}

## Data dan Spesifikasi

### Chiller :

- Merk : HITACHI
- Kapasitas : 90 TR / 120 PK
- Type : RCUP 90 AUZ
- Refrigerant : R 407
- Daya Listrik : 60 Kw
- Arus Listrik : 120 Ampere
- Tahun Pasang : Tahun 2008
- Jumlah Unit : 4 Unit

### Pompa Chiller :

- Merk : ETANG
- Kapasitas : 80 m3/h
- Type : 50 – 315
- Daya Listrik : 8 Kw
- Tahun Pasang : Tahun 2008
- Arus Listrik : 15 Ampere
- Jumlah Unit : 4 Unit

### Pompa Distribusi :

- Merk : ETAG
- Kapasitas : 38 m3/h
- Type : 50 – 200
- Daya Listrik : 2,2 Kw
- Tahun Pasang : Tahun 1984
- Arus Listrik : 4 Ampere
- Jumlah Unit : 6 Unit

### AHU Lantai 1:

- Merk : EZONE
- Kapasitas : 45 TR
- Type : EAW 18 4R+HEAT PIPE
- Daya Listrik : 5 Kw
- Arus Listrik : 9 Ampere
- Tahun Pasang : Tahun 2008
- Jumlah Unit : 5 Unit

### AHU Lantai 2:

- Merk : EZONE
- Kapasitas : 45 TR
- Type : EAW 20 4R+HEAT PIPE
- Daya Listrik : 5,5 Kw
- Arus Listrik : 11 Ampere
- Tahun Pasang : Tahun 2008
- Jumlah Unit : 4 Unit

## Chiller dan AHU Railink

### Pengoperasian Chiller

---

#### 1. Jam 06.00 WIB (Operasi ON)

**ON Chiller**

_Rotasi tiap 2 hari sekali_

- Chiller no 1 ON, Chiller no 2 STANDBY, Chiller no 3 OFF
- Chiller no 1 ON, Chiller no 2 STANDBY, Chiller no 3 OFF
- Chiller no 1 STANDBY, Chiller no 2 OFF, Chiller no 3 ON
- Chiller no 1 STANDBY, Chiller no 2 OFF, Chiller no 3 ON
- Chiller no 1 OFF, Chiller no 2 ON, Chiller no 3 STANDBY
- Chiller no 1 OFF, Chiller no 2 ON, Chiller no 3 STANDBY

**Pengecekan parameter:**

- Kapasitas running: 55%
- Set point temperature: 7.5&deg;C
- Evaporator temperature:
  - LWT: 17&deg;C - 21&deg;C
  - EWT: 17&deg;C - 21&deg;C
- Condensor temperature (Target: 35&deg;C):
  - LWT: 24&deg;C - 27&deg;C
  - EWT: 24&deg;C - 27&deg;C
- Suction temperature: 18&deg;C - 19&deg;C
- Discharge temperature: 60&deg;C - 64&deg;C
- Evaporator pressure:
  - In: 55psi
  - Out: 55psi
- Condensor pressure:
  - In: 58psi
  - Out: 50psi

**4 unit pompa CHWP ON**

**2 unit pompa CWP ON**

---

#### 2. Jam 09.30 WIB (Monitoring)

**Pengecekan parameter:**

- Kapasitas running: 100%
- Set point temperature: 7.5&deg;C
- Evaporator temperature:
  - LWT: 8&deg;C - 11&deg;C
  - EWT: 8&deg;C - 11&deg;C
- Condensor temperature (Target: 35&deg;C):
  - LWT: 25&deg;C - 32&deg;C
  - EWT: 25&deg;C - 32&deg;C
- Suction temperature: 3&deg;C - 5&deg;C
- Discharge temperature: 57&deg;C - 62&deg;C
- Evaporator pressure:
  - In: 58psi
  - Out: 58psi
- Condensor pressure:
  - In: 58psi
  - Out: 50psi

---

#### 3. Jam 14.00 WIB (Monitoring)

**Pengecekan parameter:**

- Kapasitas running: 100%
- Set point temperature: 7.5&deg;C
- Evaporator temperature:
  - LWT: 8&deg;C - 11&deg;C
  - EWT: 8&deg;C - 11&deg;C
- Condensor temperature (Target: 35&deg;C):
  - LWT: 25&deg;C - 32&deg;C
  - EWT: 25&deg;C - 32&deg;C
- Suction temperature: 0.5&deg;C - 5&deg;C
- Discharge temperature: 57&deg;C - 62&deg;C
- Evaporator pressure:
  - In: 58psi
  - Out: 58psi
- Condensor pressure:

  - In: 58psi
  - Out: 50psi

---

### Pengoperasian Cooling Tower

Pergantian setiap 2 hari sekali.

- CT No. 2 dan 3 Ops (No. 1 Standby)
- CT No. 1 dan 2 Ops (No. 3 Standby)
- CT No. 1 dan 2 Ops (No. 3 Standby)
- CT No. 1 dan 3 Ops (No. 2 Standby)
- CT No. 1 dan 3 Ops (No. 2 Standby)
- CT No. 2 dan 3 Ops (No. 1 Standby)
- CT No. 2 dan 3 Ops (No. 1 Standby)

### Pengoperasian AHU

AHU nomor 1, 3, 5, 7, 8, dan 9 ON

### Part dan Spesifikasi

- Penggantian Karet Couple Pompa CHWP

  Penggantian dilakukan apabila ketika pompa menyala bunyinya sudah agak kasar.

  {% figure src="/technical-work/chiller-dan-ahu-note/9.jpg" alt="image" /%}

  {% figure src="/technical-work/chiller-dan-ahu-note/10.jpg" alt="image" /%}

  {% figure src="/technical-work/chiller-dan-ahu-note/11.jpg" alt="image" /%}

  {% figure src="/technical-work/chiller-dan-ahu-note/12.jpg" alt="image" /%}

**V-Belt**

| Lokasi   | Type        |
| -------- | ----------- |
| AHU No.1 | -           |
| AHU No.2 | -           |
| AHU No.3 | -           |
| AHU No.4 | -           |
| AHU No.5 | -           |
| AHU No.6 | -           |
| AHU No.7 | -           |
| AHU No.8 | SPA 1557 LW |
| AHU No.9 | SPZ 987 LW  |

## Chiller dan AHU 601

### Spesifikasi

Chiller 601 menggunakan merk Hitachi dengan kapasitas 90TR. \
Setiap chiller menggunakan `2 buah compressor` dan `2 buat PHE (Plate Heat Exchanger)`

### Pengoperasian Chiller

---

#### 1. Jam 06.00 WIB (Operasi ON)

**ON Chiller**

- Chiller blok 1, 2, 3 ON
- Chiller blok 3 STANDBY

No.2 ON, No.3 Standby, No.1 OFF
No.3 ON, No.2 Standby, No.1 OFF
No.3 ON, No.2 Standby, No.1 OFF
No.2 ON, No.3 Standby, No.1 OFF
No.2 ON, No.3 Standby, No.1 OFF
No.3 ON, No.2 Standby, No.1 OFF
No.3 ON, No.2 Standby, No.1 OFF

#### 2. Jam 09.30 WIB (Monitoring)

**Pengecekan parameter:**

- Chiller blok 1

  - In : 10⁰c
  - Out : 8⁰c
  - AHU
    - Supply : 14,5⁰c
    - Return : 23.7⁰c

- Chiller blok 2

  - In : 9°c
  - Out : 8°c
  - AHU
    - Supply : 13,6⁰c
    - Return : 23.6⁰c

- Chiller blok 3 (Standby)

  - AHU
    - Supply : 17,5⁰c
    - Return : 25.8⁰c

- Chiller blok 4
  - In : 9°c
  - Out : 7°c
  - AHU
    - Supply : 15.1c
    - Return : 26.6 ⁰c

### Pengoperasian

AHU nomor 1, 3, 5, 7, 8, dan 9 ON

### Part dan Spesifikasi

- Penggantian Bearing Motor AHU Blok 1 Bawah (24 Sept 24)

- Penggantian V-Belt 4pcs AHU Blok 2 dan Blok 4 Bawah Tipe 1250 (24 Sept 24)
  {% figure src="/technical-work/chiller-dan-ahu-note/1.jpg" alt="image" /%}

- Penggantian Bearing Pompa Distribusi type 6305 (2 pcs) dan Motor Pompa Distribusi type 6205 (1 pcs) dan 6206 (1 pcs) di gedung 601 Blok 2 (20 Sept 24)

**Bearing Pompa Distribusi**

| Lokasi | Type    | Jumlah |
| ------ | ------- | ------ |
| Blok 1 | 6305    | 2      |
| Blok 2 | XPB1500 | 2      |
| Blok 3 | XPB1500 | 2      |
| Blok 4 | XPB1500 | 2      |

**Bearing Motor Pompa Distribusi**

| Lokasi | Type          | Jumlah  |
| ------ | ------------- | ------- |
| Blok 1 | 6205 dan 6206 | 1 dan 1 |
| Blok 2 | XPB1500       | 2       |
| Blok 3 | XPB1500       | 2       |
| Blok 4 | XPB1500       | 2       |

**Bearing Motor AHU**

| Lokasi | Type          | Jumlah  |
| ------ | ------------- | ------- |
| Blok 1 | 6205 dan 6206 | 1 dan 1 |
| Blok 2 | XPB1500       | 2       |
| Blok 3 | XPB1500       | 2       |
| Blok 4 | XPB1500       | 2       |

{% figure src="/technical-work/chiller-dan-ahu-note/2.jpg" alt="image" /%}
{% figure src="/technical-work/chiller-dan-ahu-note/3.jpg" alt="image" /%}

- Penggantian bearing motor Fan Condensor AC Presisi no 2 di Gedung AOCC sebanyak 3 unit Fan Condensor dengan type Bearing 6002 sebanyak 6 pcs. Unit operasi kembali 🙏🏼 (17 Sept 24)
  {% figure src="/technical-work/chiller-dan-ahu-note/4.jpg" alt="image" /%}

- Gd.AOCC R.SERVER: AC PRECISSION NO.3.
  1.Pemasangan 2 unit mator fan condensor ex .rewanding dan penggantian bearing (fan no.1 dan no. 2).

  2.pengantian Bearing motor fan no. 3.
  Type bearing 6002 .Saat ini unit stan by. (14 Sept 24)

  {% figure src="/technical-work/chiller-dan-ahu-note/5.jpg" alt="image" /%}

  - Penggantian 2pcs V-Belt ahu blok 1 bawah Gd.601 (type xpb1250)

  {% figure src="/technical-work/chiller-dan-ahu-note/6.jpg" alt="image" /%}

  {% figure src="/technical-work/chiller-dan-ahu-note/7.jpg" alt="image" /%}

  {% figure src="/technical-work/chiller-dan-ahu-note/8.jpg" alt="image" /%}

- Penggantian 2pcs V-Belt ahu blok 2 atas Gd.601 (type xpb1500)

  {% figure src="/technical-work/chiller-dan-ahu-note/13.jpg" alt="image" /%}

  {% figure src="/technical-work/chiller-dan-ahu-note/14.jpg" alt="image" /%}

  {% figure src="/technical-work/chiller-dan-ahu-note/15.jpg" alt="image" /%}

**V-Belt**

| Lokasi       | Type    |
| ------------ | ------- |
| Blok 1 Atas  | XPB1500 |
| Blok 1 Bawah | XPB1250 |
| Blok 2 Atas  | XPB1500 |
| Blok 2 Bawah | XPB1250 |
| Blok 3 Atas  | XPB1500 |
| Blok 3 Bawah | XPB1250 |
| Blok 4 Atas  | XPB1500 |
| Blok 4 Bawah | XPB1250 |
