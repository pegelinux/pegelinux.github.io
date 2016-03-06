---
layout   : page
title    : Kontribusi
share    : true
comments : false
permalink: /kontribusi/
---

Salah satu kekuatan terbesar dari pengguna GNU/Linux ada pada bentuk komunitasnya, maka tak heran sampai sekarang GNU/Linux tetap eksis. Untuk menjaga agar komunitas ini tetap eksis, kami membuka peluang sebesar-besarnya kepada siapa saja yang ingin berkontribusi pada komunitas ini.
Kontribusi dapat diberikan dalam bentuk apapun, salah satu nya adalah dengan memberikan artikel untuk ditampilkan pada situs ini. Artikel yang diberikan harap sesuai dengan tema situs ini, yaitu tentang GNU/Linux, Perkembangan IT/Teknologi, dan hal-hal lain yang berhubungan dengan komputer dengan tidak menyinggung SARA dan memperhatikan norma-norma yang berlaku di Indonesia. Untuk yang familiar dengan Git, berikut ini merupakan langkah-langkah yang dapat dilakukan untuk dapat memberikan kontribusi berupa artikel:

### 1. _Fork_ repositori pegelinux
_Fork_ repositori pegelinux pada <https://github.com/pegelinux/pegelinux.github.io/>

### 2. Tambahkan artikel
Buat dokumen baru yang berisi artikel pada folder _drafts dengan format tanggal-url.md untuk format markdown
atau tanggal-url.html untuk format html. Contoh `2013-05-22-sample-post-images.md`

### 3. Isi metadata
Pada dokumen yang telah dibuat, tambahkan metadata front matter pada bagian teratas artikel

{% highlight yaml linenums %}
---

# Layout post, dapat ditulis post untuk tema putih, atau dark-post untuk gelap
layout: post 
# Judul Artikel
title: Blogging Like a Hacker
# Informasi tentang penulis
author:
  # Nama Penulis
  name:    Komunitas PegeLinux
  # Situs penulis, atau bisa juga ditulis mailto:email jika tidak memiliki situs
  site:    http://pegelinux.github.io
  # Avatar penulis, tambahkan gambar pada folder /images/avatar/namafile.jpg 
  avatar:  namafile.jpg
  # Informasi tentang penulis, bisa satu atau dua baris
  bio:     "Komunitas pengiat GNU/Linux dan FLOSS.."
  # Email penulis
  email:   pegelinux.mail@gmail.com
  # Twitter penulis jika ada.
  twitter:  # if no twitter in this config, the twitter follow button will be removed
  # GitHub penulis jika ada.
  github: pegelinux
---
{% endhighlight %}

### 4. Buat _Pull Request_
Lakukan _pull request_ untuk artikel yang telah dibuat, untuk caranya dapat dilihat
pada <https://help.github.com/articles/using-pull-requests/>