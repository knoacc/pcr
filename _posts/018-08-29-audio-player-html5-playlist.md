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
Niatnya, ingin membuat sebuah playlist dengan 3 lagu Padi:

1. Sobat - [link](/assets/audio/padi-sobat.m4a)
2. Bidadari - [link](/assets/audio/padi-bidadari.m4a)
3. Mahadewi - [link](/assets/audio/padi-mahadewi.m4a)

Sayangnya, setelah di coba beberapa kali tetap saja tidak bisa. Bohong besarr....

Yasudahlah.. Pakai tag audio saja

<audio controls><source src="/assets/audio/padi-sobat.m4a" preload="meta" type="audio/m4a" /></audio>
<audio controls><source src="/assets/audio/padi-bidadari.m4a" preload="meta" type="audio/m4a" /></audio>
<audio controls><source src="/assets/audio/padi-mahadewi.m4a" preload="meta" type="audio/mp4" /></audio>

**Cekrek!**

### Maafkan aku sobat...

Jika berhasil, ya, jika berhasil, _yo uapik sanget toh_.

Mmm... sudah hampir 2 jam terlewati hanya untuk tulisan ini. Dan menghabiskan waktu se-sore kemarin untuk mencoba di localhost. Lumayanlah, bisa membunuh waktu dengan hal berguna yang sebenarnya _gak guna banget_.

![Nguyup Kopi](ngopi.jpg)

_Uyup sek kopine..._ Next time, pakai javascript saja. Ada dua yang perlu di coba: 

1. Contoh audio player via [jsfidle](http://jsfiddle.net/vkMqR/2374/)
2. Contoh audio player via [codepen](http://codepen.io/markhillard/pen/Hjcwu)
