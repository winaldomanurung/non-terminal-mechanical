---
title: HVAC Troubleshooting
nextjs:
  metadata:
    title: HVAC Troubleshooting
    description: Panduan belajar HVAC Troubleshooting.
---

## Legenda

- Liquid Line = Discharge Line = Pipa Kecil = Red Line = High Side
- Gas Line = Suction Line = Pipa Besar = Blue Line = Low Side

{% figure src="/technical-work/hvac-troubleshooting/31.png" alt="image" /%}

## Compressor Overheat

- Cabut compressor
- Ganti oli compressor
- Sebelum pemasangan lakukan flushing unit indoor dengan R11 dan R22 (R11 khusus digunakan untuk flushing)

## Compressor Short

Butuh penggantian compressor 7525 2 unit

## Compressor Macet

- Bisa dilakukan pembongkaran kompressor, dengan cara digerinda sisi atasnya
- Kuras oli dari dalam kompresor
- Rendam rotor dengan solar untuk membersihkan kerak sambil putar-putar rotor
- Jika rotor sudah lancar dan normal, bisa dilakukan pengelasan

## Motor Fan Condensor Short

- Ganti kanibal dengan motor fan unit lain

## AC Panas

- Cek apakah outdoor menyala
- Jika mati maka lakukan reset overload

## Pompa chiller berbunyi kasar

- Ganti bearing pompa

## Penggantian Evaporator pada AC Gardu Standing Duct

- Siapkan evap baru yang sudah ditest pressure
- Buka cover AC
  {% figure src="/technical-work/hvac-troubleshooting/1.jpg" alt="image" /%}
- Pelepasan pipa high dan low
  {% figure src="/technical-work/hvac-troubleshooting/2.jpg" alt="image" /%}
- Pelepasan pinggir panel
  {% figure src="/technical-work/hvac-troubleshooting/3.jpg" alt="image" /%}
- Pelepasan evap
  {% figure src="/technical-work/hvac-troubleshooting/4.jpg" alt="image" /%}
- Pengelasan pipa low dan high
  {% figure src="/technical-work/hvac-troubleshooting/5.jpg" alt="image" /%}

Setelah itu evaporator bisa dipasang ke unit.

## Terjadi Icing pada AC

### Problem

Inti dari icing pada evap adalah ketika freon di dalam evap tidak bisa menyerap panas dengan baik, karena dari itu maka terbentuk ice
Gampangnya hal ini disebabkan 2 hal: Kurang freon atau kotor
Namun jika ditilik lebih lanjut bisa jadi juga ada kebocoran oli di dalam evap.

### Troubleshoot

Harus tunggu dulu icing nya mencair

Lalu kita juga bisa mengecek blower apakah dia bekerja dengan baik, karena jika blower rusak, maka sirkulasi udara di sekitar evap tidak berjalan dengan baik. Kenapa bisa begitu? Karena air di sekitar evap biasanya mengandung uap air, yang mana harus dihembuskan ataupun kalau mengembun dibuang melalui drainase. Namun ketika tidak dibuang, dia akan menempel di evap dan lama-lama menjadi bunga es.
Lalu kemungkinan terakhir adalah adanya penyumbatan pada pipa kapiler. Pipa kapiler ini punya 2 fungsi: menurunkan tekanan refrigeran dan mengatur aliran refrigeran ke evaporator.

## V-Belt indoor split duct retak

Penggantian v-belt dengan type A39

## Karet coupling pompa condenser rusak

Penggantian karet coupling

{% quick-links %}
{% quick-link title="Surat Penetapan Pelaksana Pekerjaan" icon="theming" href="https://docs.google.com/document/d/1Mv9cSWDqFihYP6fKeHm8bl_aGgj4WXLa/edit?usp=sharing&ouid=112772237280787020683&rtpof=true&sd=true"  /%}
{% /quick-links %}

## Unit off alarm

Lakukan reset dari power listrik

## Fan macet

Bisa jadi kapasitor bermasalah. Kejadian banyak di AOCC.

{% figure src="/technical-work/hvac-troubleshooting/27.jpg" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/28.jpg" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/29.jpg" alt="image" /%}

## Guide

Troubleshooting AC meliputi mechanical side, refrigerant, dan electrical side.

{% figure src="/technical-work/hvac-troubleshooting/10.png" alt="image" /%}

### Step 1: Lihat apakah compressor running

- Apakah compressor running?
- Apakah blower fan running?
- Cek apakah udara keluaran condenser terasa hangat? (Ini merupakah udara panas yang ditarik dari ruangan)
- Cek apakah `liquid line` (pipa kecil) suhunya normal? (Jangan panas ataupun dingin, tapi kira-kira sedikit lebih hangat dari suhu badan)
- Cek apakah ada `liquid line filter dryer`? Kalau ada, apakah suhu in dan outnya sama? (Jika tidak sama, maka `liquid line filter dryer` perlu diganti)

{% callout type="note" title="Compressor tidak running" %}
Jika ternyata compressor tidak running, maka 99% masalah terjadi di electrical side.
{% /callout %}

{% callout type="warning" title="Compressor running" %}
Kalau ternyata compressor running, maka masalah di sistem lain. Lihat ke bagian mechanical side dan refrigerant.
{% /callout %}

### Step 2: Cek apakah thermostat (remote) diatur dengan benar

{% callout type="note" title="Thermostat tidak disetting dengan benar" %}
Ubah settingan sesuai kebutuhan.
{% /callout %}

{% callout type="warning" title="Thermostat benar dan compressor juga running" %}

Lalu pastikan juga bahwa terdapat cukup aliran udara (airflow) di coil evaporator (`low side`), dengan cek:

- air filters
- dampers
- fire dampers
- registers, grille, diffuser
- lihat apakah udara ke return grille terblock, misal oleh furniture
- lihat apakah evaporator kotor
- apakah fan motor tidak bekerja
- apakah fan motor salah speed
- arah putaran fan motor

Airflow bisa kita cek dengan anemometer. (Standar: 1 ton unit, 400 CFM).

Jika salah satu ini terjadi maka akan menyebabkan `low suction pressure`.

---

Pastikan juga bahwa coil condenser (`high side`) tidak kotor. Lihat antara fin apakah terdapat kotoran-kotoran yang mengganggu sirkulasi udara.
Pastikan bahwa condenser fan bekerja dengan arah yang benar.

{% /callout %}

### Step 3: Cek refrigerant

- Gunakan pressure gauge
- Cek untuk superheat dan subcooling

{% figure src="/technical-work/hvac-troubleshooting/11.png" alt="image" /%}

Untuk mengukur pressure kita harus ukur dengan pressure gauge, yang mana blue line untuk low side dan red line untuk high side.

{% figure src="/technical-work/hvac-troubleshooting/12.png" alt="image" /%}

Disini kita bisa lihat bahwa blue line terbaca 68.5 psig, yang mana standarnya dia akan menghasilkan 40°F (4.44°C) di evaporator coil.

Standarnya untuk R22 adalah:

- Low side: 68.5 psig
- High side: 260 psig
- Evap. temp: 40°F (4.44°c)

{% figure src="/technical-work/hvac-troubleshooting/13.png" alt="image" /%}

Di refrigerant R410a juga sama, kita mau menghasilkan 40°F (4.44°C) di evaporator coil, yang mana artinya standarnya 118 psi di low side.

Standarnya untuk R410 adalah:

- Low side: 118 psig
- High side: 410 psig
- Evap. temp: 40°F (4.44°c)

Darimana kita tau standar-standar itu?

Semua refrigerant punya karakteristik hubungan antara pressure dan temperaturenya. Namun, standarnya kita mau punya suhu 40°F (4.44°C) di evaporator coil. Nah ini bisa dicapai jika kita punya proper suction pressure yang mana didapat dari good airflow.

{% figure src="/technical-work/hvac-troubleshooting/15.png" alt="image" /%}

Kita bisa berpatokan dari chart ini:

{% figure src="/technical-work/hvac-troubleshooting/6.png" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/7.png" alt="image" /%}

Ketika kita sudah mengecek pressure, kita perlu cek **superheat**. Superheat akan memberitahu kita bahwa ada cukup refrigerant di dalam evaporator. Kita berpatokan untuk nilai superheatnya di `charging chart` yang ada di dalam unit, dan kalau emang ga ada `charging chart` kita coba untuk maintain superheat diantara 8°F-12°F.

- Untuk mengetahui superheat, kita harus tahu `actual evaporator pressure` (low side pressure) (suction pressure)
- Lalu kita convert pressure ke dalam temperature (lihat di chart)
- Kita lakukan pembacaan `temperature of the gas leaving the evaporator`
- Kita kurangkan `actual evaporator pressure` dengan `temperature of the gas leaving the evaporator`

Contoh:

R22

- `low side pressure`: 68 psig
- `pressure converted to temperature`: 40°F
- `temperature of the gas leaving the evaporator`: 50°F
- `subtract temperature`: 10°F

Kalau masih belum paham, kita lihat gambar ini:

{% figure src="/technical-work/hvac-troubleshooting/8.png" alt="image" /%}

Disini kita bisa lihat bahwa suhu di evaporator adalah 40°F (4.44°C), sedangkan suhu keluaran dari evaporator adalah 50°F (10°C). Titik X disebut dengan `pre-determined point` karena disinilah refrigerant dalam bentuk liquid berakhir. Ketika awal masuk evaporator, terdapat 75% L dan 25% V. Seiring berjalannya di evaporator refrigerant akan semakin berkurang kadar liquidnya hingga akhirnya semua menjadi 100% V di titik X.
Selama hijau tua, dia T nya adalah 40°F. Intinya di hijau tua itu adalah fase boiling, dan as long as it is boiling, suhunya adalah 40°F (4.44°C). Namun, setelah titik X, dia naik temperaturnya hingga akhirnya 50°F di fase superheating (ungu), ini merupakan temperature diatas saturation temperature.

Oke, bagaimana cara pengecekannya di real life?
{% figure src="/technical-work/hvac-troubleshooting/16.png" alt="image" /%}

Kita butuh probe (kanan) yang disambungkan ke avometer.
{% figure src="/technical-work/hvac-troubleshooting/17.png" alt="image" /%}

Kita sambungkan red line dan blue line ke unit.

Convert pembacaan blue line ke temperature: 68 psi -> 40°F

Kita bisa lihat pembacaan keluaran evaporator adalah 50°F.

Tinggal kita kurangi 50°F - 40°F = 10°F.

Karena masih di dalam range 8°F-12°F, maka masih aman.

Hal yang sama juga terjadi di refrigerant lainnya:
{% figure src="/technical-work/hvac-troubleshooting/18.png" alt="image" /%}

{% callout type="note" title="Pressure dan superheat low" %}

Jika memang pressure dan superheat masih low, maka masih ada problem di airflow, khususnya di evaporator, jadi balik ke point sebelumnya.

Selain itu, cek juga untuk room temperature. Jika room temperature is very low, maka ada problem di airflow juga. Biasanya kita ingin room temperature di 72°F (22.22°C)-75°F (23.88°C). Jika dia turun sampai 68°F (20°C)-70°F (21.11°C), bisa jadi ada masalah di low side/suction pressure, yang menyebabkan superheat menjadi low.

Suction pressure low dan superheat low ini mengindikasikan bahwa refrigerant tidak boiling dengan waktu yang cukup cepat sehingga membuat pressure turun.

{% figure src="/technical-work/hvac-troubleshooting/19.png" alt="image" /%}

Kita ingin di X itu refrigerant dalam bentuk oil. Engineer sudah mendesign agar refrigerant boiling at this point. Jika `udara` keluaran evaporator ga di standar (ex: 75°F (23.88°C)), melainkan sangat rendah di 68°F (20°C), maka tidak ada cukup heat untuk boil the refrigerant fast enough, yang akan menyebabkan pre-determined point nya akan menjauh jadi di X baru.

{% figure src="/technical-work/hvac-troubleshooting/20.png" alt="image" /%}

```shell
Case:
Pressure low, low superheat
=>
Suction line filter dryer is clogged
# or
# Indicates that the charge is high
```

Jika suction pressure low, maka cek suction line filter dryer. Apakah dia clogged? Karena kalau kondisinya clogged, dia akan menghambat flow refrigerant dan suction pressure nya akan naik sebelum masuk dryer (di evaporator) yang dampaknya akdalah suction pressure akan low setelah keluar dryer (menuju compressor). Maksudnya gimana?

{% figure src="/technical-work/hvac-troubleshooting/21.png" alt="image" /%}

Ketika suction line filter dryer kondisinya bagus, maka hasil pembacaan pressure sebelum dan sesudahnya adalah sama.

{% figure src="/technical-work/hvac-troubleshooting/22.png" alt="image" /%}

Namun, ketika kondisi SLFD clogged, maka pembacaan pressure akan turun setelah melewati SLFD.

Masalahnya adalah, kebanyakan kita mengecek langsung di condensing unit (sebelum masuk compressor):
{% figure src="/technical-work/hvac-troubleshooting/23.png" alt="image" /%}

Padahal seharusnya kita ukur di sebelum dan sesudah SLFD untuk mengecek pressure difference. Tanpa pengecekan ini, dan langsung mengukur di condensing unit (masukkan compressor) kita jadi mikir bahwa unit kurang refrigerant. Lalu kita lakukan penambahan refrigerant. Kelebihan refrigerant ini akan menyebabkan `pre-determined point` menjauh dari yang seharusnya. Apa dampaknya? Liquid masuk kembali ke compressor. Hal ini akan berdampak buruk pada compressor. Kenapa bisa gitu? Ketika liquid refrigerant masuk ke dalam compressor, dia akan bercampur oil, dan oil jadinya ikut di sirkulasikan di dalam sistem. Compressor jadi tidak ada oil, dan bisa macet.

```shell
Case:
Pressure low, high superheat
=>
Indicates that the charge is low
```

Katakanlah misalnya, pressure sebelum dan sesudah SLFD sama-sama low, maka pre-determined point nya akan berpindah naik:
{% figure src="/technical-work/hvac-troubleshooting/24.png" alt="image" /%}

Apa artinya? Dengan PDP berpindah lebih depan, maka artinya proses superheating akan berlangsung di area yang lebih banyak, yang mana nantinya superheatnya akan jadi lebih tinggi.

{% figure src="/technical-work/hvac-troubleshooting/25.png" alt="image" /%}

Jika superheat tinggi, maka artinya kita mengalami kekurangan refrigerant.

Apa yang harus kita lakukan?

Find and repair the leak. Baru setelah itu kita charge the system. Ada 3 cara untuk charge the system:

- superheat
- subcooling
- by weight

```shell
Case:
Unit is overcharged with low airflow
=>
The suction pressure would be normal or slightly high with low superheat
```

- Overcharge => pressure up
- Overcharge with low airflow => pressure down because it's not boiling fast enough but PDP moving down

Overcharging akan memindahkan PDP down, mengecilkan area superheat.
Refrigerant yang terlalu banyak dalam sistem pendingin dapat menyebabkan suhu evaporator yang tinggi, yang disebabkan oleh tekanan refrigerant yang tinggi. Selain itu, pengisian refrigerant yang terlalu banyak dapat merusak kompresor karena bekerja terlalu keras.

Efek lain dari kelebihan refrigerant saat mengisi refrigerant adalah kemampuan menarik cairan, atau kompresor menarik refrigerant yang masih cair. Pada prinsipnya kompresor tidak boleh memompa refrigerant cair karena dapat merusak kompresor.

Disini kita lihat pressure suction bagus. Suhu evap coil juga bagus. Tapi, suhu refrigeran keluaran evap hanya 42.

{% figure src="/technical-work/hvac-troubleshooting/26.png" alt="image" /%}

PDP nya down, menyebabkan superheat kecil.

{% /callout %}

{% callout type="warning" title="Jika superheat aman, maka kita lanjut ke subcooling" %}
Kalau nilai superheat aman dan sesuai dengan standar, maka kita lanjut ke pengukuran subcool.
{% /callout %}

### Step 4: Cek condenser

Jika high side pressure tinggi, maka kita harus cek condenser, apakah ada kotoran atau apapun yang menghambat flow udara yang melewatinya.
Jika memang ada kotoran, kita bisa berihkan dengan menggunakan coil cleaner.

Setelah itu kita juga bisa cek:

- apakah motor fan condenser rusak
- apakah ada hambatan udara
- apakah motor fan condenser benar putaran arahnya
- apakah motor fan condenser terlalu lambat putarannya

Setelah cek semuanya, jika pressure masih tinggi, maka cek superheat dan subcooling.

Jika pressure tinggi, dan superheat low dan subcooling high, maka unit is overcharged, yang artinya ada terlalu banyak refrigerant di dalam sistem.

**Case Low Side Pressurenya Tinggi**

We charge by subcooling when we have a TXV as a metering device, expansion device. Metering device ada 5:

- thermostat expansion valve
- electronic expansion valve
- automatic expansion valve
- capillary tube
- piston

Jika superheatnya high, dibarengi dengan high suction pressure, maka bisa jadi high room temperature atau high return air temperature.

Jika suction pressurenya sedikit low, maka cek kondisi suction line filter dryer. Jika suction line filter dryernya clogged, maka dia akan menghambat flow dari refrigerant dan suction pressurenya akan meningkat sebelum mencapai dryer dan juga di evaporator. Hal ini akan menyebabkan low pressure setelah dryer dan juga di compressor suction.

{% figure src="/technical-work/hvac-troubleshooting/30.png" alt="image" /%}

Disini kita bisa lihat outlet dari suction line filter fryer menurun dari 70 psig ke 63 psig. Sebelum masuk filter dryer, pressurenya naik, dan bersamaan dengan itu temperature juga naik di evaporator jadi 42°F (5°C), padahal kita pengen di evap sekitar 40°F (4.5°C).

Jika suction pressurenya high dan discharge/high pressurenya low maka ini bisa jadi karena valve yang rusak di compressor. Jika seperti ini, maka perlu dilakukan penggantian compressor.

Ini semua case kalau compressor running. Kalau ngga, maka masuk ke electrical side.
Cek apakah compressor hot, atau condenser motor nya hot.

### Step 5: Cek electrical

Kita cek dulu apakah ada power masuk ke kontaktor ataupun ke breaker.

Kita harus cek baiik dari **line side** ataupun **control side**.

Cara termudah adalah dengan push contactor supaya energized. Ketika kita push contactor dan tidak ada yang terjadi, maka bisa kita simpulkan problemnya ada di line side. Kita ambil avometer kita dan cek voltagenya.

Namun, jika setelah kita push contactor dan ternyata compressor running, maka bisa kita simpulkan problem ada di control side (24 Volts).

Jika saat kita push, ternyata memang kondisi contactor sudah energized, maka masalahnya bisa jadi di line side ataupun emang compressornya udah jelek. Disini berarti 24V nya oke. Namun, disini bisa jadi juga ternyata contactornya yang emang udah bad contact. Untuk pengecekan contactor kita bisa lakukan dengan mengecek L1 dan L2, pembacaan voltagenya harus 220 V. L1 dan T1 pembacaan voltagenya harus 0 (tidak ada beda potensial), dan L2 dan T2 pembacaan voltagenya harus 0 (tidak ada beda potensial). Jika L1 dan T1 serta L2 dan T2 ada beda potensial maka contactor sudah bad contact.

Misal di L1 dan T1 ada pembacaan 10V, maka ini artinya ada 10V yang tidak terhantarkan (bad contact). Makanya kita harus mendapatkan pembacaan 0V yang artinya semua voltage bisa dihantarkan dari L1 ke T1.

---

Jika kita sudah ada indikasi bahwa line side yang bermasalah, maka kita bisa cek apakah ada **fuse yang terputus** atau ada **MCB yang turun**. Jika emang ada, hal ini bisa disebabkan oleh **bad compressor** atau **bad condenser fan motor**. Kita harus melakukan pengecekan short ground pada compressor dan fan.

Jika kita menemukan ada **fuse yang terputus** atau ada **MCB yang turun**, maka kita bisa lakukan pengecekan short, open, dan ground.

- Short atau ground bisa menyebabkan fuse putus atau circuit breaker trip. Ini merupakan indikasi grounded compressor atau grounded condenser fan motor. Short artinya ada path yang shortened, allowing more electrons to flow, yang mana menyebabkan ampere naik. Dengan naiknya ampere, maka breaker atau fuse akan blow.

---

Jika kita dapati compressor tidak running, jika compressornya merupakan single phase compressor maka kita harus melakukan discharge capacitor terlebih dahulu. Kita bisa melakukannya dengan menggunakan resistor atau obeng.
{% figure src="/technical-work/hvac-troubleshooting/32.png" alt="image" /%}
Ini kita lakukan dengan posisi kabel masih tersambung.

Selanjutnya kita disconnect kabel dari capacitor dan cek microfarads nya capacitor. Bagaimana ceknya? Kita bisa gunakan multimeter. Hasil pembacaan yang baik adalah dengan toleransi kurang lebih 10%. Jika capacitor terdapat oli, swollen atau kaya bekas terbakar, maka kita harus ganti, gausah cek microfarad (kapasitansi) lagi.

Penggantian capacitor harus sesuai spec kapasitansi dan voltagenya. Jika kapasitansi terlalu besar maka bisa menyebabkan winding compressor terbakar. Jika terlalu rendah, maka kita gabisa mengirimkan enough power ke compressor, yang menyebabkan compressor tidak bisa running.

Jika compressornya merupakan compressor 3 phase, maka kita ga perlu capacitor. Sama juga untuk motor condenser dan motor evaporator. Kalau mereka merupakan 3 phase, maka ga perlu capacitor.

Jadi, jika capacitornya bagus atau compressornya 3 phase, maka kita disconnect kabel dari compressor dan cek electrical connections for continuity.

Di compressor 3 phase, semua connections akan memiliki nilai resistansi yang sama. Jadi kita cek ketiga electrical connections antara 3 windings:
{% figure src="/technical-work/hvac-troubleshooting/34.png" alt="image" /%}

Disini kita bisa lihat sebuah compressor 3 phase dengan Y/star connection (sangat jarang yang menggunakan delta connection). Kita cabut wirenya:
{% figure src="/technical-work/hvac-troubleshooting/35.png" alt="image" /%}

Kita cek resistance:

{% figure src="/technical-work/hvac-troubleshooting/36.png" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/37.png" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/38.png" alt="image" /%}

Disini kita bisa lihat resistance nya selalu sama. Ini menandakan motor compressor masih bagus.

Di compressor 1 phase, kita discharge capacitor lalu cek capacitor. Kalo emang udah oke maka kita lanjut check for continuity (resistance on windings). Di dalam single phase compressor akan ada 2 windings dengan 3 connections (C, R, dan S), yang merupakan Common, Run, dan Start.

{% figure src="/technical-work/hvac-troubleshooting/39.png" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/40.png" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/41.png" alt="image" /%}

Berarti bentukan windingnya adalah seperti ini:

{% figure src="/technical-work/hvac-troubleshooting/42.png" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/43.png" alt="image" /%}
{% figure src="/technical-work/hvac-troubleshooting/44.png" alt="image" /%}

- Nilai yang paling besar adalah RS.
- Yang terkecil adalah RC
- Sisanya adalah CS.

{% figure src="/technical-work/hvac-troubleshooting/45.png" alt="image" /%}

Start winding akan memiliki highest reading resistance.
