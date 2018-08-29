---
title: "Membunuh Waktu: Membuat Playlist Lagu-lagu Padi, Online Boss!"
description: Dengan tingkat kesenggangan waktu yang begitu tak terbatas,
banner_image: player.jpg
image: nganu
tags: [audio player, html, playlist, padi band]
---
Seperti biasa, karena _saking nganggure_, Saia butuh kegiatan yang membuat jari (secara spesifik: dua jempol) sibuk. Setelah dua hari tak ada hal baru dalam keseharian _saia_; ngopi, _jandon_, main game [War Robots](https://warrobots.net/en) atau [PUBG](http://www.pubgmobile.com/en-US) sambil tiduran tentu saja. Akhirnya ketemu juga yang belum pernah saya coba: **Membuat sebuah _audio player_ sederhana dengan fitur playlist**. 
<!--more-->

Tujuannya tentu saja agar bisa memainkan beberapa file audio sekaligus sesuai dengan urutan yang ditentukan dalam playlist. Secara sederhana, jika hanya memakai tag `audio` HTML5 saja hanya bisa [memainkan satu file audio saja](https://www.knoacc.org/2012/10/menambah-audio-ke-blog-web-dengan-html5.html) dalam satu tag. Dan harus menekan kembali tombol play lagi jika ingin memutar file audio lainnya. Tidak nyaman tentu saja.

Setelah mencoba beberapa metode yang ada di internet, ada satu cara yang relatif mudah. Dan hasil percobaan yang saia coba implementasikan di halaman lain yang memuat beberapa lagu dari band Indonesia: Padi, dari album pertama.

### Embed

Untuk melakukannya termasuk mudah dan sudah mampu menampung playlist `.m3u`, sebagai contohnya:

```html
<embed name="music_playlist"
src="/music/music_playlist.m3u"
width="150"
height="90"
loop="false"
autostart="true"
```

Untuk itu ada 3 hal yang perlu di lakukan:
1. Siapkan juga file audio secara on-line. Upload beberapa file di hosting website kamu.
2. Membuat file **m3u** yang memuat daftar file audio/mp3 yang ingin dimainkan.
3. Buat juga file HTML dengan kode untuk memainkan lagu dalam playlist.

Sekarang **Kerjakan!**, _ojo plonga-plongo koyo wedhus kopok_ dhus, wedhus..

### 1. Upload file Mp3

Unggah ke lokasi tertentu di website kamu, entah dengan dengan cara apa terserah. Entah dengan FTP upload atau fitur Web upload jika tersedia.

Jika memakai [CDN](https://en.wikipedia.org/wiki/Content_delivery_network) sebaiknya tempatkan dalam folder yang termasuk dalam daftar _cache_ atau masuk dalam file _statis_ agar tidak menghabiskan jatah bamdwith bulanan. Dalam percobaan ini _saia_ tempatkan di lokasi `/assets/audio/`

### 2. Membuat file `m3u`

Jangan gunakan file **m3u** yang dibuat secara otomatis oleh audio player semacam [WinAmp](http://www.winamp.com/index.html) atau [AIMP](https://aimp.ru). Karena playlist yang dibuat tidak akan bisa diputar secara online.

1. Buat dulu file teks baru dengan [notepad++](https://notepad-plus-plus.org/download/v7.5.8.html) atau [editor teks lainnya](https://mi.knoacc.org/aplikasi-editor-kode-sumber-terbaik-web-developer-progammer).
2. Buat daftar lokasi file mp3 yang ingin dimainkan. Bisa dengan _absolut path_ seperti: `https://www.paciran.com/assets/audio/lagu.mp3` atau _relative path_ seperti: `/assets/audio/lagu.mp3`. Ingat, sisipkan satu baris baru setiap _path_.
3. Simpan file dengan akhiran `.m3u`, misalnya: `daftarlagu.m3u` 
Lihat contoh isi file **m3u** (_relative path_) berikut:

```plain
/assets/audio/padi-sobat.mp3

/assets/audio/padi-menanti-sebuah-jawaban.mp3

/assets/audio/padi-mahadewi.mp3
```

Upload juga file `contoh_playlist.m3u` yang sudah jadi ke web hosting milikmu.

### 3. Kode HTML untuk menyematkan playlist

Tambahkan kode untuk menyematkan playlist ke file HTML agar lagu bisa dimainkan. Gunakan saja kode seperti yang ada [di atas](#embed).

Atau bisa juga menggunakan kode di bawah. Bedanya ada perubahan `autostart="true"` biar lagu bisa langsung diputar, sedangkan jika _kepingin lagune_ bisa terus diputar terus-menerus, rubah juga nilai `loop="true"` dari kode di bawah:

```html
<embed name="playlist_lagu"
src="/assets/audio/contoh_playlist.m3u"
width="800"
height="90"
loop="false"
hidden="false"
autostart="true"/>

```

### Maafkan aku sobat...

Jika berhasil, hasilnya kurang lebih seperti yang tampil di bawah ini:

<div style="max-width:100%"><audio name="playlist_lagu"
src="/assets/audio/contoh_playlist.m3u"
width="800"
height="90"
loop="false"
hidden="false"
autostart="true" /></div>

Mmm... sudah hampir 2 jam terlewati hanya untuk tulisan ini. Dan menghabiskan waktu se-sore kemarin untuk mencoba di localhost. Lumayanlah, bisa membunuh waktu dengan hal berguna yang sebenarnya _gak guna banget_.

![Nguyup Kopi](ngopi.jpg)

_Uyup sek kopine..._
