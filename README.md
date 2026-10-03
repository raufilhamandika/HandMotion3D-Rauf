# HandMotion3D

Animasi partikel 3D yang bisa dikendalikan dengan gerakan tangan di depan webcam. Proyek ini menggunakan MediaPipe untuk mengenali gestur tangan, lalu mengubah bentuk partikel menjadi kosmos, Saturnus, tulisan "I LOVE YOU", atau hati.

## Gestur

| Gestur | Tampilan |
| --- | --- |
| Tangan terbuka atau gestur lain | Partikel kosmos biru |
| Telunjuk saja tegak | Saturnus |
| Telunjuk dan jari tengah tegak (peace) | Tulisan "I LOVE YOU" |
| Tangan mengepal | Bentuk hati |

Pada mode Saturnus, tulisan, dan hati, posisi tangan juga menggerakkan posisi bentuk di layar.

## Persiapan

- Windows 64-bit
- Miniconda
- Webcam

Buka **Anaconda Prompt (Miniconda3)**, lalu jalankan perintah berikut satu per satu:

```bash
conda create -n space_gesture python=3.11 -y
conda activate space_gesture
python -m pip install numpy==1.26.4 mediapipe==0.10.21 opencv-contrib-python==4.11.0.86 pygame PyOpenGL
```

## Menjalankan

Di Anaconda Prompt yang sudah aktif dengan environment `space_gesture`, buka folder proyek yang sudah diunduh atau di-clone, lalu jalankan:

```bash
cd /d "PATH\TO\HandMotion3D"
python index.py
```

Ganti `PATH\TO\HandMotion3D` dengan lokasi folder proyek di komputermu.

Izinkan akses webcam jika diminta. Tekan **Esc** pada jendela animasi 3D atau **q** pada monitor kamera untuk menutup aplikasi.

## Catatan

- Pastikan prompt menampilkan `(space_gesture)` sebelum menjalankan aplikasi.
- Jika kamera tidak terbuka, tutup aplikasi lain yang sedang menggunakan webcam dan coba lagi.
- `catatan.py` berisi catatan dan cheat sheet tambahan.
