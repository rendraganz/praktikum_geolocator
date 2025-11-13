
## MUHAMMAD RENDRA IRAWAN || 362458302036

### praktikum_geolocator

**Tugas 1**: Geocoding (Alamat dari Koordinat)
Saat ini kita hanya menampilkan Lat/Lng. Buatlah agar aplikasi menampilkan alamat
(nama jalan, kota, dll) dari koordinat yang didapat.
Petunjuk:
1. Anda sudah menambahkan paket geocoding di pubspec.yaml.
![import pubspec](media/import_geo.png)

2. Import paketnya: import ’package:geocoding/geocoding.dart’;
![import di main](media/panggil_geo.png)

3. Buat variabel String? currentAddress; di MyHomePageState.
![buat variabel baru](media/var_baru.png)

4. Buat fungsi baru getAddressFromLatLng(Position position).
![fungsi getAddressFromLatLng](media/getAddress.png)

5.  Panggil fungsi getAddressFromLatLng( currentPosition!) di dalam getLocation
dan startTracking (di dalam .listen()) setelah setState untuk currentPosition.
![panggil di getLocation](media/getLocation.png)
![panggil di startTracking](media/startTracking.png)

6. Tampilkan currentAddress di UI Anda, di bawah Lat/Lng.
![tampil di UI](media/panggil_ui.png)

**Tugas 2**: Jarak Real-time ke Titik Tetap
Manfaatkan fungsi Geolocator.distanceBetween dari Langkah 4.
1. Buat variabel String? distanceToPNB; di MyHomePageState.
![variabel distanceToPNB](media/var_latlong.png)

- Saya ambil latitude dan longitude dari Poliwangi.
![latlong poliwangi](media/latlong_poli.png)

2. Di dalam startTracking (di dalam .listen()), panggil fungsi untuk menghitung jarak:
![panggil fungsi dilisten](media/panggil_listen.png)


3. Simpan hasilnya di distanceToPNB menggunakan setState. (Dalam bentuk meter).
![setState](media/set_state.png)

4. Tampilkan distanceToPNB di UI agar jaraknya ter-update secara real-time saat Anda bergerak
![tampilan UI](media/ui.png)

5. Hasil Akhir.
- Versi Meter
![Versi meter](media/ui_meter.jpg)

- Versi KiloMeter
Ubah pada bagian setState
![new state](media/set_km.png)

- Hasilnya
![Versi km](media/ui_km.jpg)

- Posisi saya (warkop setia kawan)
![titik awal](media/titik_awal.jpg)


