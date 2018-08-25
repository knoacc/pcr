---
title: "Teman Tapi Menikah Itu Judul Film Indonesia Cak!"
description: Niatnya memberi tahu, ternyata tempe. Seng takon lho sopo?
image: http://i0.wp.com/images.harianjogja.com/2018/03/Cuplikan-adegan-di-film-Teman-Tapi-Menikah-Youtube-.jpg 
tags: [nonton bareng, TTM 2018, streaming, bajakan lagi]

---
Hanya catatan ringan: TTM, kalau dijamanku sekolah, ini singkatan dari rangkaian kata **teman tapi mesra**. Lebih dipahami sebagai pertemanan antar dua remaja bejenis kelamin berbeda dengan tingkat intimasi yang lebih dari teman. Tanpa status "pacaran", "_gendak-an_", cem-cem-an tetapi _ngalor-ngidul_ ya berdua saja.
<!--more-->

TTM dulu judul lagu dibawakan duo Ratu. Sekarang, TTM jadi judul film yang diperankan oleh... siapa ya?  Pokoknya, kali ini _saia_ cuma mau mencoba menyematkan sebuah film Indonesia, yang juga sudah pernah ditayangkan di penyedia layanan _streaming_ Viu dan Hooq. Dan kebablas di-bajak oleh bangsa sendiri, maklumlah, negara agraris.

Karena sudah _kadung kevajak_ sekalian saja dijadikan bahan untuk mencoba fitur _embed_ (semat) video yang di-hosting di situs openload dengan memanfaatkan container video responsive bootstrapp.

<div class="embed-responsive embed-responsive-16by9">
<iframe class="embed-respomsive-item" poster="{{ page.image }}" src="https://oload.stream/embed/T2p1vC2mzrQ/%5BThe_Streamer%5D_streamer.knoacc.org_%5BTTM2018-web-dl%5D" frameborder="0" alowfullsxreen="allow"></iframe>
</div>

Biasanya, kode semat yang diberikan oleh (misalnya) Youtube, perlu mencantumkan nilai `width` dan `height` agar tidak _mletot_ sana-sini. Sayangnya kalau ukuran layar lebih kecil, video sematan akan terpotong. Ternyata element `iframe` yang di berikan oleh situs video streaming (baik itu youtube atau lainnya) bisa dibuat _responsive_, maksudnya menyesuaikan layar dan tidak harus memberikan nilai `width` dan `height` seperti yang terlihat di atas.

Jadi, jika sudah situs atau blog terdapat plug-in bootsrapp, bisa menjadikan video lebih enak dilihat. Sperti apa pembungkusnya? Kurang lebih seperti ini:

```html
<div class="embed-responsive embed-responsive-16by9">
<iframe class="embed-respomsive-item" src="http://link.sematan.situs/youtube/dan-lainya" frameborder="0" alowfullsxreen="allow"></iframe>
</div> 
```

### Penutup

Teman Tapi Menikah bukan cuma ada di film! Koncoku yo akeh _mblo_.. :D

Okay, karena sudah _kadung_ terpasang, kita nikmati bareng biar _gak mubazir_. Mau nonton bareng teman?


