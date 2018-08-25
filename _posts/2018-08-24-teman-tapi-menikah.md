---
title: "Teman Tapi Menikah Itu Judul Film Indonesia Cak!"
description: Niatnya memberi tahu, ternyata tempe. Seng takon lho sopo?
image: https://i0.wp.com/images.harianjogja.com/2018/03/Cuplikan-adegan-di-film-Teman-Tapi-Menikah-Youtube-.jpg 
tags: [nonton bareng, TTM 2018, streaming, bajakan lagi]

---
Hanya catatan ringan: TTM, kalau dijamanku sekolah, ini singkatan dari rangkaian kata **teman tapi mesra**. Lebih dipahami sebagai pertemanan antar dua remaja bejenis kelamin berbeda dengan tingkat intimasi yang lebih dari teman. Tanpa status "pacaran", "_gendak-an_", atau _cem-cem-an_. Tetapi _ngalor-ngidul_ ya berdua saja.
<!--more-->

TTM dulu judul lagu yang dibawakan oleh [duo Ratu](https://id.m.wikipedia.org/wiki/Ratu_(grup_musik)). Sekarang, TTM jadi judul film yang diperankan oleh... siapa ya?  Pokoknya, kali ini _saia_ cuma mau mencoba menyematkan sebuah film Indonesia, yang juga sudah pernah ditayangkan di penyedia layanan _streaming_ Viu dan Hooq. Dan kebablas di-bajak oleh bangsa sendiri, maklumlah, negara agraris.

![Cuplikan Film TTM 2018]({{ page.image }}){:.align-center}

Karena sudah _kadung kevajak_ sekalian saja dijadikan bahan untuk mencoba fitur _embed_ (semat) video yang di-hosting di situs openload dengan memanfaatkan container [video responsive bootstrapp](https://getbootstrap.com/docs/4.1/utilities/embed/)

<div class="embed-responsive embed-responsive-16by9">
<iframe class="embed-respomsive-item" poster="{{ page.image }}" src="https://oload.stream/embed/T2p1vC2mzrQ/%5BThe_Streamer%5D_streamer.knoacc.org_%5BTTM2018-web-dl%5D" frameborder="0" alowfullscreen="allow"></iframe>
</div>

Biasanya, kode semat yang diberikan oleh (misalnya) [Youtube](https://www.youtube.com), perlu mencantumkan nilai `width` dan `height` agar tidak _mletot_ sana-sini. Sayangnya kalau ukuran layar lebih kecil, video sematan akan terpotong.

Ternyata element `iframe` yang di berikan oleh situs video [streaming](https://www.paciran.com/2018/08/19/aplikasi-streaming-bola-eropa-paling-lengkap.html) (baik itu youtube atau lainnya) bisa dibuat _responsive_, maksudnya menyesuaikan layar dan tidak harus memberikan nilai `width` dan `height` seperti yang terlihat di atas.

Jadi, jika situs atau blog sudah terdapat plug-in bootsrapp, bisa menjadikan video lebih enak dilihat. Seperti apa pembungkusnya? Kurang lebih seperti ini:

```html
<div class="embed-responsive embed-responsive-16by9">
<iframe class="embed-respomsive-item" src="http://link.sematan.situs/youtube/dan-lainya" frameborder="0" alowfullscreen="allow"></iframe>
</div> 
```
Selain dipakai untuk membungkus kode sematan, container responsif ini bisa di pakai juga untuk element `video` HTML 5 seperti yang pernah _saia_ pakai dipostinga blog untuk membungkus [video lagu Para Penerka-nya Iwan Fals](https://www.paciran.com/2018/08/23/para-penerka-iwan-fals-noah.html).
### Penutup

[Teman Tapi Menikah]() bukan cuma ada di film! Koncoku yo akeh _mblo_.. :D

Okay, karena sudah _kadung_ terpasang, kita nikmati bareng biar _gak mubazir_. Mau nonton bareng teman? Teman yang mana?


