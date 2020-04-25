---
title: Rekomendasi Plugin Hexo Untuk Optimasi SEO
tags: Plugin Hexo
categories: Hexo
keywords: 
description: Salah satu kelebihan dari hexo adalah banyak nya plugin untuk keperluan optimasi, berikut ini rekomendasi plugin hexo terbaik
top_img: /img/quantum.svg
cover: /img/plugin-hexo.svg
toc: true
toc_number: false
copyright: 
mathjax: 
katex: 
hide: 
---

Hexo memiliki banyak kelebihan jika Kamu ingin memiliki platform blogging yang canggih, cepat dan modern, salah satu yang akan di bahas IMOclub disini adalah faktor terpenting untuk keperluan optimasi blog Kamu yaitu dengan menginstall beberapa rekomendasi plugin hexo berikut ini.
Sebelum itu ada baiknya Kamu mengetahui seberapa penting plugin pada hexo apalagi jika Kamu adalah seorang webmaster dari platform blogger.

## Apa Itu Plugin Hexo?
Jika Kamu pengguna wordpress pasti sudah tidak asing dengan istilah plugin karena tanpa plugin sudah tentu wordpress Kamu tidak akan teroptimasi dengan baik. 
Sama hal nya dengan Hexo, dan dengan adanya plugin ini tentu akan membuat Kamu yang biasa memakai platform Blogspot akan semakin CINTA sama Hexo ini.

Plugin berfungsi untuk keperluan optimasi mulai dari mempercantik tampilan sampai hal yang terpenting untuk optimasi SEO karena akan berasa percuma jika Kamu memilih platform yang tidak ada kelebihannya di mata SERP google. 

Dan berita baiknya Hexo menyediakan banyak plugin untuk keinginan optimasi Kamu, namun karena plugin nya juga lumayan banyak maka IMOclub akan merangkum beberapa plugin penting yang IMOclub juga pakai pada Blog ini. 

## Rekomendasi Plugin Hexo 
Jika Kamu mau melihat daftar lengkap kumpulan plugin Hexo maka silahkan langsung kunjung [Official Plugin Hexo](https://hexo.io/plugins/). Jika sebelumnya Kamu baru saja belajar dari artikel Tutorial Hexo di blog ini tentu Kamu akan kebingungan karena ada banyak plugin yang menurut mu bagus digunakan.

Olehkarena itu berikut IMOclub akan memberikan rekomendasi terbaiknya, namun ada baiknya juga Kamu harus melakukan eksperimen sendiri untuk plugin-plugin lain yang di sediakan Hexo. 

Untuk proses install plugin nya sangatlah mudah tinggal ketik perintah di bawah ini di terminal VScode atau CMD Kamu. 
```
npm install (plugin yang ingin Kamu install)
```

### Hexo Deploy Git
Plugin ini sangatlah membantu untuk memudahkan Kamu yang ingin Hexo nya tampil live di laman github Kamu sendiri. Untuk proses install nya cukup ketikkan perintah berikut
```
npm install hexo-deployer-git --save
```
Copy Paste juga perintah di bawah ini ke _config.yml Blog Kamu
```
# Deployment
## Docs: https://hexo.io/docs/deployment.html
deploy:
  type: git
  repo: https://github.com/<username>/<username>.github.io.git
  branch: master
```

### Hexo JSON Feed Generator
Ini juga amatlah penting jika Kamu ingin memudahkan dan mempercepat google untuk merayapi Blog Hexo Kamu. Plugin ini berfungsi sama seperti RSS FEED. 
Copy Paste perintah berikut untuk proses install nya
```
npm i -S hexo-generator-json-feed
```
Lalu copy paste juga perintah berikut ke _config.yml Blog Kamu
```
jsonContent:
  meta: true
  drafts: false
  file: content.json
  keywords: undefined
  dateFormat: undefined
  pages:
    title: true
    slug: true
    date: true
    updated: true
    comments: true
    path: true
    link: true
    permalink: true
    excerpt: true
    keywords: false
    text: true
    raw: false
    content: false
    author: true
  posts:
    title: true
    slug: true
    date: true
    updated: true
    comments: true
    path: true
    link: true
    permalink: true
    excerpt: true
    keywords: false
    text: true
    raw: false
    content: false
    author: true
    categories: true
    tags: true
```

### Hexo All Minifier
Plugin ini berfungsi seperti WP Rocket pada wordpress yaitu meminify HTML, CSS, JAVASCRIPT dan juga IMAGE. Dan plugin ini akan otomatis meminify tiap Kamu menjalankan perintah "Hexo Server" maupun "Hexo Generate". 
Copy Paste perintah berikut ke CMD Kamu untuk menginstall plugin ini. 
```
npm install hexo-all-minifier --save
```

Dan jangan lupa copy paste perintah di bawah ini ke config.yml Kamu. 
```
all_minifier: true
```
pengaturan lengkap jika Kamu mau melakukan custom silahkan ke docs nya langsung dengan mengklik titel di atas. 

### Hexo SEO Friendly Sitemap
Plugin ini merupakan manifestasi dari plugin wordpress yaitu YOAST untuk generate sitemap yang sesuai standar SEO. Copy paste perintah berikut ke CMD Kamu. 
```
npm install hexo-generator-seo-friendly-sitemap --save
```

Cukup copy paste perintah berikut ke config.yml Kamu.
```
sitemap:
    path: sitemap.xml
    tag: false
    category: false
```

### Hexo Algolia Search
Tidak seperti platform lainnya yang jika ingin menambahkan fitur search post akan ada secara otomatis. Di Hexo Kamu perlu menginstall plugin ini jika ingin hasil di menu pencarian akan sesuai dengan index semua tipe postingan artikel Kamu. 
Copy paste perintah berikut ke CMD Kamu untuk menginstall nya.
```
npm install hexo-algoliasearch --save
```
Dan masukkan perintah berikut ke config.yml Kamu:
```
plugins:
  - hexo-algoliasearch
```

### Hexo Auto Canonical
Yap plugin ini berfungsi untuk mengenerate semua link di blog Kamu secara canonical yang penting juga untuk keperluan SEO di Hexo.
Copy paste perintah berikut untuk menginstall:
```
npm install --save hexo-auto-canonical
```
Lalu masukkan perintah berikut bukan ke config.yml Kamu tapi ke bagian HEAD pada blog Kamu:
Untuk EJS,
```
<%- autoCanonical(config, page) %>
```
Untuk jade,
```
| !{ autoCanonical(config, page) }
```

## Kesimpulan
sebenarnya masih banyak rekomendasi plugin hexo lainnya yang bisa Kamu sesuaikan dengan tema pilihan maupun buatan Kamu sendiri tinggal ke official nya saja untuk mempelajari nya. Untuk list plugin di atas merupakan list wajib yang ada di tema Kamu terutama jika untuk mengoptimalkan SEO. Artikel selanjutnya IMOblog akan membahas cara custom schema untuk lebih mengoptimalkan blog Kamu di mata search engine. 
