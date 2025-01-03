---
title: Chiller dan AHU Railink
nextjs:
  metadata:
    title: Chiller dan AHU Railink
    description: Catatan tentang Chiller dan AHU Railink.
---

## Layout

{% quick-links %}
{% quick-link title="Cooling Tower (Top)" icon="theming" href="https://drive.google.com/file/d/1sagtXASByzueKcIszLIAT7Mhr0_RbfE-/view?usp=sharing"  /%}
{% quick-link title="Cooling Tower (Front)" icon="theming" href="https://drive.google.com/file/d/1ZW4z0yKiti5xj1EcAWt728HKw5ZIoFl-/view?usp=sharing"  /%}
{% quick-link title="Cooling Tower (Side)" icon="theming" href="https://drive.google.com/file/d/16jjh4iILT5V-n1DVh_A98CbRSeT7oPVt/view?usp=sharing"  /%}
{% quick-link title="Chiller (Top)" icon="theming" href="https://drive.google.com/file/d/1qDtWxmeRanwx3pwC1h3XnlfnA7j3YMFC/view?usp=sharing"  /%}
{% quick-link title="Chiller (Front)" icon="theming" href="https://drive.google.com/file/d/1i8bUEhTyBLOA-6Lf2qoiP8DxOpshlPTI/view?usp=sharing"  /%}
{% quick-link title="Chiller (Side)" icon="theming" href="https://drive.google.com/file/d/1aOto-fJzo-IZJIAcuvYbNn3rC8oCp8Pn/view?usp=sharing"  /%}
{% /quick-links %}

## Cara Kerja

Jadi di chiller ada dua hal yang mengalir, refrigerant dan air (water). Refrigerant digunakan untuk mendinginkan air dan air digunakan untuk mendinginkan ruangan.

Hal ini diawali dengan proses kompresi refrigerant pada compressor. Kenapa kompresi perlu dilakukan?

Disini sebenarnya terkait dengan yang namanya boiling point.

{% figure src="/chiller-dan-ahu-railink/1.png" alt="image" /%}

Disini kita bisa lihat bahwa ketika pressure semakin tinggi makan boiling point juga ikut meninggi.

Sebelumnya kita harus mengenal yang namanya superheat dan subcooling.

- Superheat: Terjadi ketika kita memanaskan uap pada suhu diatas suhu boiling pointnya.
- Subcooling: Terjadi ketika kita mendinginkan uap pada suhu dibawah suhu kondensasinya (suhu dimana uap berubah menjadi liquid).

Katakanlah refrigerant boils pada suhu 40F pada pressure yang rendah di evaporator. Karena di evap dia menyerap panas, maka kita memanaskan vapor (uap) hingga misalnya 50F. Temperature ini sudah melebihi boiling pointnya, makanya disebut superheat.

Formulanya:
Superheat = Current Temperature - Boiling Point
Pada contoh ini superheatnya senilai 10F.

Superheat ini penting dalam HVAC karena dia memastikan refrigerant dalam bentuk liquid sudah mendidih (boiled) sebelum meninggalkan evaporator dan masuk ke compressor, karena kalau refrigerant masuk compressor dalam bentuk liquid, dia akan merusak compressor. Jadi superheat terjadi di evaporator.

Lalu katakanlah refrigerant masuk ke condenser pada pressure tinggi (karena sudah masuk compressor) dan suhu 140F. Katakanlah dia memiliki condensation point di 120F. Ketika condenser mendinginkan refrigeran ke suhu 120F, maka dia akan berubah jadi liquid. Namun, proses cooling tidak berhenti disitu. Hal inilah yang dinamakan subcooling.

Subcooling = Boiling Point - Current Temperature

Jadi ketika misalnya refrigerant diturunkan suhunya oleh condenser ke 105F, terjadi subcooling 15F. Ini penting karena subcooling memastikan refrigerant dalam bentuk liquid lah yang masuk ke expansion valve.

Key takeaways: superheat occurs in the evaporator to protect the compressor, and subcooling occurs in the condenser to protect the expansion device.

Lalu, kembali ke pertanyaan kenapa perlu dilakukan kompresi?

Katakanlah setelah keluar dari evaporator suhu refrigerant 50F(10C) dan pressure 142. Disini dia udah uap semua. Katakanlah kita biarkan dia tanpa melewati compressor dan langsung masuk condenser. Kita ingat bahwa condenser akan mendinginkan refrigeran agar dia berubah jadi liquid. Nah untuk mengubah jadi liquid berarti condenser harus menurunkan suhu katakanlah -10C (intinya di bawah suhu refrigerant sekarang yang berbentuk uap), maka akan sangat sulit bagi condenser untuk melakukannya. Hal ini karena kebanyakan condenser hanya memanfaatkan kipas fan untuk mendinginkan refrigerant. Kecuali kita tinggal di kutub utara, maka akan sangat sulit untuk membuat suhu refrigerant jadi -10C. Untuk itulah kita butuh kompressor. Disini dia meningkatkan P dan T katakanlah di 539 dan 60C. Untuk mengubahnya jadi liquid katakanlah kita hanya butuh mengubah refrigeran menjadi 40C suhunya. Hal ini bisa dilakukan dengan bantuan kipas di suhu Indonesia.

---

Jadi, proses chiller dimulai dengan proses compression pada compressor:

{% figure src="/chiller-dan-ahu-railink/2.png" alt="image" /%}

Disini P dan T refrigerant akan naik dan berubah bentuk menjadi vapor. Disini kita bisa lihat ada beberapa sensor tekanan:

{% figure src="/chiller-dan-ahu-railink/3.png" alt="image" /%}

Dan juga ada pressure transmitter:
{% figure src="/chiller-dan-ahu-railink/4.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/5.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/6.png" alt="image" /%}

Kita juga bisa melihat yang namanya valve connector.

{% figure src="/chiller-dan-ahu-railink/7.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/8.png" alt="image" /%}

Kita bisa lihat dari compressor terdapat dua output:

{% figure src="/chiller-dan-ahu-railink/9.png" alt="image" /%}

…yang mana keduanya masuk ke oil separator:

{% figure src="/chiller-dan-ahu-railink/10.png" alt="image" /%}

…dan dialirkan ke condensor:

{% figure src="/chiller-dan-ahu-railink/11.png" alt="image" /%}

Dari kondenser dialirkan lagi melalui ball valve:

{% figure src="/chiller-dan-ahu-railink/12.png" alt="image" /%}

…masuk ke dryer:

{% figure src="/chiller-dan-ahu-railink/13.png" alt="image" /%}

…sebelum akhirnya masuk expansion valve:

{% figure src="/chiller-dan-ahu-railink/14.png" alt="image" /%}

…dan masuk ke evaporator:

{% figure src="/chiller-dan-ahu-railink/15.png" alt="image" /%}

Dari evap dia akan masuk lagi ke compressor:

{% figure src="/chiller-dan-ahu-railink/16.png" alt="image" /%}

Untuk aliran refrigerant siklusnya seperti itu. Lalu bagaimana dengan aliran airnya?

Supply air (berasal dari CT dan CWP) masuk ke evaporator untuk didinginkan:

{% figure src="/chiller-dan-ahu-railink/17.png" alt="image" /%}

Dan keluar untuk di supply lagi ke AHU:

{% figure src="/chiller-dan-ahu-railink/18.png" alt="image" /%}

Dia keluar dari ruangan chiller:

{% figure src="/chiller-dan-ahu-railink/19.png" alt="image" /%}

Dia di return lagi dari ruangan masuk ke ruang chiller dan masuk ke pompa chiller CHWP:

{% figure src="/chiller-dan-ahu-railink/20.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/21.png" alt="image" /%}

Keluar dari pompa CHWP dia masuk ke evap chiller:

{% figure src="/chiller-dan-ahu-railink/22.png" alt="image" /%}

Lalu ada juga supply line untuk condenser:

{% figure src="/chiller-dan-ahu-railink/23.png" alt="image" /%}

Setelah melalui condenser untuk mendinginkan refrigerant, dia akan keluar lagi:

{% figure src="/chiller-dan-ahu-railink/24.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/25.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/26.png" alt="image" /%}

…masuk ke cooling tower:

{% figure src="/chiller-dan-ahu-railink/27.png" alt="image" /%}

Dimana dia akan didinginkan dengan bantuan fan dan air:

{% figure src="/chiller-dan-ahu-railink/28.png" alt="image" /%}

Lalu didistribusi lagi:

{% figure src="/chiller-dan-ahu-railink/29.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/30.png" alt="image" /%}
{% figure src="/chiller-dan-ahu-railink/31.png" alt="image" /%}

Ke pompa distribusi CWP:

{% figure src="/chiller-dan-ahu-railink/32.png" alt="image" /%}

…dan dialirkan ke condenser.

## Spesifikasi

- Type Chiller 1: EWWD460I-SS06 CH-17NO2547
- Type Chiller 2: EWWD460I-SS06 CH-16l02142
- Type Chiller 3: EWWD460I-SS06 CH-16l02143

### Sensor dan Transducer

Perbedaan sensor dan transducer:
{% figure src="/chiller-dan-ahu-railink/sensor.png" alt="image" /%}

Untuk chiller sendiri ada sensor dan transducer:

- Transducer 1-8 Bar (`1 ea`)
- Transducer 0-30 Bar (`2 ea`)
- NTC 4mm 10 MT (Negative Coefisien Temperature) (`7 ea`)
  Ketika temperatur air pendingin naik maka resistansi pada sensor ini akan menurun dan sebaliknya bila temperatur air pendingin ini turun maka resistansinya akan naik.
  {% figure src="/chiller-dan-ahu-railink/ntc.png" alt="image" /%}

- HP Switch PSC-B6S 19.8 Bar RMO (`2 ea`)
  Sensor untuk pressure
  {% figure src="/chiller-dan-ahu-railink/psc.png" alt="image" /%}

### Module Expansion Valve

### Module Display Unit

### Oil Filter FR3A/3100/3200/4300

### Compressor Oil Filter Gasket/O-Ring Kit

### Adjustable Phase Protector

### Water Flow Switch

### Filter Core Drier

### Dasi Oil Compressor - B

### Daikin Refrigerant R-134A

### Condensor: Provides CBCC2731070

- Capacity: 970 kW
- Weight: 302 kg
- Tube Side

  - Pressure: 16 bar
  - Temperature: -10&deg;C/+105&deg;C
  - Pressure Test: 17.6 bar
  - Volume: 40L
  - Fluid: Water

- Shell Side
  - Pressure: 35 bar
  - Temperature: -10&deg;C/+120&deg;C
  - Pressure Test: 30.5 bar
  - Volume: 100L
  - Fluid: R134A

### Evaporator

### Oil Separator

- Pressure: 23.5 bar
- Temperature: -10&deg;C - 120&deg;C
- Pressure Test: 25.9 bar
- Volume: 44 L

## Pengoperasian Chiller

### 1. Jam 06.00 WIB (Operasi ON)

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

### 2. Jam 09.30 WIB (Monitoring)

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

### 2. Jam 14.00 WIB (Monitoring)

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

## Pengoperasian Cooling Tower

- CT No. 2 dan 3 Ops (No. 1 Standby)
- CT No. 1 dan 2 Ops (No. 3 Standby)
- CT No. 1 dan 2 Ops (No. 3 Standby)
- CT No. 1 dan 3 Ops (No. 2 Standby)
- CT No. 1 dan 3 Ops (No. 2 Standby)
- CT No. 2 dan 3 Ops (No. 1 Standby)
- CT No. 2 dan 3 Ops (No. 1 Standby)

## Pengoperasian AHU

AHU nomor 1, 3, 5, 7, 8, dan 9 ON

## Share

Ketika tegangan drop, butuh ampere yang lebih tinggi
Penggantian oil setiap 8000 hours atau 3 tahun, mana yang tercapai terlebih dahulu
Untuk Ampere 10% diatas dan 5% dibawah rata-rata.
