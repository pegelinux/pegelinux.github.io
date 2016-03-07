---
layout:     post
title:      PegeLinux Menggunakan Domain dot ID
date:       2016-03-07 06:45:29
summary:    Mengarahkan Domain Asali dari GitHub Pages Ke Domain pegelinux.id
categories: tutorial
author:
  # Nama Penulis
  name:    Ali
  # Situs penulis, atau bisa juga ditulis mailto:email jika tidak memiliki situs
  site:    https://situsali.com
  # Avatar penulis, tambahkan gambar pada folder /images/avatar/namafile.jpg 
  avatar:  http://ali.my.id/images/ali.gif
  # Informasi tentang penulis, bisa satu atau dua baris
  bio:     "Komunitas pengiat GNU/Linux dan FLOSS.."
  # Email penulis
  email:   admin@situsali.com
  # Twitter penulis jika ada.
  twitter:  alisoftware
  # GitHub penulis jika ada.
  github: aliterm
---

Hari ini tanggal 7 Maret 2016 s/d 21 Maret 2016 di [Rumahweb](http://gratis.rumahweb.co.id/) sedang mengadakan promo gratis satu tahun _domain_ `.id`, Nah dalam kesempatan itu saya coba mengambil _domain_ dengan nama [pegelinux.id](http://pegelinux.id) sebagai pengganti dari _domain_ [pegelinux.Github.io](http://pegelinux.Github.io).

Adapun caranya adalah sebagai berikut:

1. Buat berkas dengan nama `CNAME` wajib dengan huruf kapital semua.
2. Isikan berkas itu dengan domain Anda, misalnya `pegelinux.id`.<br/>
![alt CNAME](http://ali.my.id/images/post/pegelinux-id-domain-1.png "CNAME")
3. Kemudian masuk ke `domain panel` ubah `A Record` dari _domain_ Anda tersebut menjadi: 

| name | IP             |
|------|----------------|
| @    | 192.30.252.153 |
| @    | 192.30.252.154 |

<br/>
Ini berurusan dengan tempat Anda membeli _domain_. Dalam contoh di sini saya menggunakan pengaturan _domain_ bawaan [Digital Ocean](https://m.do.co/c/734a86fa5365).<br/>
![alt A Record](http://ali.my.id/images/post/pegelinux-id-domain-2.png "A record")

4. Jika sudah selesai bisa langsung Anda `git add CNAME`, `git commit -m "menambahkan CNAME"` dan `git push -u origin master`.

5. Jika sudah selesai cek di _setting_ repositori Anda. Sudah seperti gambar berikut:<br/>
![alt A Record](http://ali.my.id/images/post/pegelinux-id-domain-3.png "pegelinux.id")

Langkah terakhir yakni tes apakah GitHub _pages_ Anda sudah mengarah ke domain Anda tersebut, apa belum. Semoga bermanfaat.😊

Sumber: http://ali.my.id/tutorial/2016/03/07/github-domain/