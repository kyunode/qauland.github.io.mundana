---
layout: post
title:  "Hal-hal yang bisa dilakukan dengan Markdown"
author: hyropk
categories: [ jekyll, markdown ]
image: https://images.unsplash.com/photo-1528784351875-d797d86873a1?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80
---

Banyak hal yang bisa Anda lakukan dengan Markdown. Markdown digunakan untuk memformat bagian teks, seperti menebalkan (**bold**), memiringkan (_italic_), dan sebagainya. Mempelajari Markdown tidaklah serumit mempelajari bahasa kode yang lain, misalnya JavaScript. 

Agar lebih gampang, sebaiknya Anda membuka kode sumber dari artikel ini untuk mengetahui seluruh kode Markdown yang digunakan di sini. Kode sumber dari artikel ini bisa Anda dapatkan di dalam folder `_posts`.


## Pemformatan spesial

Selain **bold** dan _italic_, Anda juga dapat menggunakan pemformatan lain dalam Markdown, seperti:

+ ~~tercoret (strikethrough)~~
+ \*_escaped characters_\*


## Menulis kode

Kode dapat ditulis dalam dua cara: sebaris dan multi-baris.

Kode sebaris ditulis dengan menambahkan _back-tick_ (\`) pada awal dan akhir kode.

`<main role="main" class="site-content"></main>`

Kode multi-baris ditulis dengan menambahkan tiga _back-ticks_ sebelum dan sesudah kode ditulis. Anda juga dapat menyatakan bahasa kode agar kode terlihat lebih bagus.

```
.my-link {
    text-decoration: underline;
}
```

```html
<!-- Content -->
<main role="main" class="site-content">
    <button class="navbar-toggler collapsed" type="button" data-toggle="collapse" data-target="#navbarColor02" aria-controls="navbarColor02" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
</main>
```

## Menambahkan gambar

Untuk menambahkan gambar ke dalam artikel, gunakan format `![teks-alternatif](url-gambar.ekstensi)`.

![walking]({{ site.baseurl }}/assets/images/8.jpg)

## Daftar to-do

- [ ]  Ya 1

- [x]  Ya 2

## Reference lists

The quick brown jumped over the lazy.

Another way to insert links in markdown is using reference lists. You might want to use this style of linking to cite reference material in a Wikipedia-style. All of the links are listed at the end of the document, so you can maintain full separation between content and its source or reference.

## Full HTML

Perhaps the best part of Markdown is that you're never limited to just Markdown. You can write HTML directly in the Markdown editor and it will just work as HTML usually does. No limits! Here's a standard YouTube embed code as an example:

<p><iframe style="width:100%;" height="315" src="https://www.youtube.com/embed/aShSUqSbhss?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe></p>
