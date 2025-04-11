# 📘 Catatan Belajar & Dokumentasi Pribadi

Halo! Repository ini saya buat sebagai tempat menyimpan catatan, eksperimen, dan dokumentasi pribadi selama proses belajar di dunia pemrograman, khususnya di bidang ****** ***** ********

# Tujuan

- Menyimpan berbagai materi, catatan, dan hasil praktikum secara rapi.
- Membangun kebiasaan dokumentasi untuk setiap hal yang dipelajari.
- Menjadi pengingat perjalanan saya dalam dunia IT, mulai dari hal kecil hingga mahir.
- Sebagai referensi pribadi dan mungkin bisa bermanfaat juga buat orang lain. <-- meski saya sendiri tidak bermanfaat

---

> Jangan pernah remehkan catatan kecil, karena dari situlah awal kamu jadi besar.

 ███╗   ██╗ █████╗ ██╗   ██╗ █████╗ ███╗  ██╗ 
 ████╗  ██║██╔══██╗██║   ██║██╔══██╗████╗ ██║
 ██╔██╗ ██║███████║██║   ██║███████║██╔██╗██║
 ██║╚██╗██║██╔══██║╚██╗ ██╔╝██╔══██║██║╚████║
 ██║ ╚████║██║  ██║ ╚████╔╝ ██║  ██║██║ ╚███║
 ╚═╝  ╚═══╝╚═╝  ╚═╝  ╚═══╝  ╚═╝  ╚═╝╚═╝  ╚══╝



#LINUX
_Panduan Lengkap Install Linux_
*dual boot

Persyaratan Awal
> Sebelum memulai instalasi, pastikan hal-hal berikut telah dipersiapkan:
1. Laptop atau PC dengan Windows yang sudah terinstal.
2. Koneksi internet (hanya dibutuhkan untuk mengunduh file ISO dan membuat USB bootable).
3. USB flash drive minimal 8 GB.
4. Ruang kosong di hard drive atau SSD minimal 30 GB untuk Linux.
5. Backup semua data penting dari Windows untuk menghindari kehilangan data. <==== harus backup sebab kita tidak tau rejeki apa yang datang

Langkah 1: Unduh Linux
1. Buka situs resmi distro linuxnya
2. Pilih edisi sesuai kebutuhan. <==== kalo mau maen game di windows aja dek gausah make linux, gaguna soalnya
3. Klik salah satu mirror (server) untuk mengunduh file ISO.

Langkah 2: Buat USB Bootable Linux
> Gunakan aplikasi Rufus (Windows) untuk membuat USB bootable.
1. Unduh Rufus dari https://rufus.ie
2. Colokkan USB flash drive ke laptop.
3. Buka Rufus, dan lakukan pengaturan berikut:
- Device: pilih USB kamu
- Boot selection: pilih file ISO Linux Mint yang sudah diunduh
- Partition scheme:
- GPT untuk UEFI
- MBR untuk Legacy BIOS
- File system: FAT32
4. Klik "Start" lalu tunggu hingga selesai.

Langkah 3: Siapkan Partisi untuk Linux
1. Tekan Windows + X, lalu pilih "Disk Management".
2. Klik kanan pada partisi yang memiliki ruang besar (misalnya drive C), lalu pilih "Shrink Volume".
3. Masukkan ukuran yang ingin dipakai untuk Linux , misalnya 40000 MB (40 GB).
4. Klik "Shrink". Akan muncul partisi kosong (unallocated).

Langkah 4: Boot ke USB Linux 
1. Colokkan USB ke laptop.
2. Restart laptop, lalu tekan tombol untuk masuk boot menu (umumnya F12, Esc, F9, atau F2 tergantung merek).
3. Pilih boot dari USB.
4. Pilih opsi "Start Linux (distronya)" untuk masuk ke mode live session.

Langkah 5: Jalankan Instalasi Linux 
1. Setelah desktop Linux muncul, klik ikon "Install Linux".
2. Pilih bahasa yang diinginkan.
3. Pilih layout keyboard.
4. Ceklis opsi "Install multimedia codecs" jika tersedia.
5. Pada bagian installation type, pilih "Something else" agar dapat mengatur partisi secara manual.

Langkah 6: Atur Partisi Linux 
> Cari partisi kosong (unallocated space) yang telah dibuat sebelumnya.
> Buat tiga partisi utama:
1. Root (/)
- Klik partisi kosong > Add
- Size: 30000 MB (30 GB)
- Type: Primary
- File system: Ext4
- mount point: /
2. Swap
- Klik partisi kosong > Add
- Size: 2048–4096 MB (2–4 GB)
- Type: Logical
- Use as: swap area
3. Home (/home) (opsional, bisa disatukan dengan /)
- Sisanya dari ruang kosong
- Type: Logical
- File system: Ext4
- Mount point: /home

Langkah 7: Pilih Lokasi Bootloader
> Pastikan bootloader diinstall di drive utama, biasanya /dev/sda (bukan partisi seperti /dev/sda1).

Langkah 8: Selesaikan Instalasi
1. Pilih zona waktu sesuai lokasi kamu.
2. Masukkan nama pengguna, nama komputer, dan password.
3. Klik "Install Now", lalu konfirmasi perubahan partisi.
4. Tunggu proses instalasi selesai.
5. Setelah selesai, klik "Restart Now".
6. Cabut USB saat diminta.

Langkah 9: Dual Boot Berhasil
1. Saat komputer menyala, kamu akan melihat menu boot (GRUB) yang memungkinkan kamu memilih:
2. Linux (distronya)
3. Windows Boot Manager
4. Kamu bisa memilih salah satu sesuai kebutuhan.






