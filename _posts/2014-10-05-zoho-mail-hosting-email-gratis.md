---
layout: post
title: "Zoho Mail : Hosting E-mail Gratis dengan Domain Sendiri"
description: "Membuat alamat E-mail dengan nama domain sendiri secara gratis menggunakan layanan Zoho mail."
tags: [internet, email, gratis, zoho, custom domain]
comments: true
share: true
---

Pada awalnya saya ingin membuat tulisan mengenai cara membuat alamat E-mail dengan nama domain kita sendiri di [Outlook.com](http://domains.live.com). Namun, tanggal 3 oktober 2014 lalu saya menemui bahwa sejak bulan April 2014 layanan ini ditutup. Sebagai gantinya pengguna yang ingin menggunakan layanan serupa diminta menggunakan [Office 365](http://http://en.wikipedia.org/wiki/Office_365), yang bersifat premium. Pada akhirnya saya mencoba mencari alternatif di Google dan menemukan [Zoho.com](https://www.zoho.com/company.html) yang menyediakan layanan E-mail hosting juga, tentunya secara gratis.

Oke. Sekarang saya akan memberikan step-by-step cara mendaftar layanan E-mail hosting di Zoho ini.

* Pertama, masuk ke [halaman ini](https://www.zoho.com/mail/zohomail-pricing.html). Di sana akan ada beberapa pilihan harga. Pilih sesuai keinginan Anda (di sini saya memilih yang gratis).
![Daftar Harga]({{site.url}}/images/post/zohomail-1.png)
* Setelah _click_ tombol __sign up__, Anda akan diarahkan ke halaman berikut. Isikan nama domain Anda disana, lalu _click_ __Add Domain__
 ![Daftar Harga]({{site.url}}/images/post/zohomail-2.png)
* Isikan data diri Anda, lalu _click_ __Sign Up__
 ![Daftar Harga]({{site.url}}/images/post/zohomail-3.png)
 Alamant E-mail yang baru Anda buat tadi nantinya akan dijadikan Super Administrator.
* Kemudian buka kotak masuk E-mail Anda untuk melakukan konfirmasi pendaftaran.
![Daftar Harga]({{site.url}}/images/post/zohomail-4.png)
* Selanjutnya, perlu dilakukan konfirmasi kepemilikan nama domain, serta pengaturan MX record domain kita. Untuk melakukan konfirmasi kepemilikan nama domain, dapat dilakukan dengan beberapa cara salah satunya dengan menambah pengaturan di CNAME record domain dengan data berikut. Untuk mendapatkan data ini silahkan masuk ke akun Super Administrator tadi [di sini](http://zoho.com/mail), lalu buka __Control Panel >> Domains__.
![Daftar Harga]({{site.url}}/images/post/zohomail-5.png)
Jika sudah sekarang waktunya untuk mengatur MX record domain kita. Gunakan data berikut ini.

|Host    | Address         |Priority  |
|:-----: |:---------       |:--------:|
|@/Blank |mx.zohomail.com  |10        |
|@/Blank |mx2.zohomail.com |20        |
{: rules="groups"}

Kemarin saat saya mencoba, rentang waktu yang dibutuhkan hingga pengaturan dapat digunakan sekitar 15 menit dan mungkin akan berbeda untuk Anda. 
Apabila ada yang masih belum jelas jangan sungkan untuk bertanya di kolom komentar. Selamat mencoba. :)
