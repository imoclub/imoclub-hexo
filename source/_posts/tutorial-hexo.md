---
title: Tutorial Hexo Untuk Membuat Blog Modern 
date: 2020-04-05 21:41:08
tags: Tutorial Hexo
categories: Hexo
keywords: 
description: Apa itu hexo? Berikut akan di jelaskan tutorial hexo terlengkap untuk membuat blog yang modern dan dapat di implementasikan pada hosting Kamu
top_img: /img/digital-marketing.svg
cover: /img/tutorial-hexo.svg
toc: true
toc_number: false
copyright: 
mathjax: 
katex: 
hide: 
---

Apa itu Hexo? Untuk Tutorial Hexo kali ini ditujukan untuk para webmaster yang senang dengan EFISIENSI WAKTU dan PERFORMA SPEED. Karena Hexo merupakan salah satu bagian framework pada jamstack yang bekerja dengan Nodejs sehingga menjadikan Hexo sebagai salah satu Static Site Generator (SSG) terfavorit dan mudah untuk di pahami bahkan bagi pemula sekalipun.
Dan yang paling utama kelebihan dari hexo ini CMS nya ya komputer Kamu sendiri jadi Kamu bisa sesuka hati melakukan eksperimen template sampai update artikel sebanyak-banyak nya.
Kalo Kamu mau lihat referensi tema-tema keren dari Hexo bisa mampir ke Official Hexo ya.

## Tutorial Hexo
Sekarang buat kamu yang mau tutorial lengkap untuk memulai Hexo, maka ikutin aja tiap step yang ada disini dan pembahasan tutorial disini saya tujukan untuk yang benar-benar masih awam sama sekali ya bahkan buat yang gak bisa ngoding sebelumnya. Jadi mohon pengertian nya untuk yang merasa SUHU atau ter MASTER yang ikut baca disini. Sekarang silahkan siapkan bahan-bahan dapur nya dulu:

- Install chocolatey
- Install VScode
- Intall Git
- Install NodeJS
- Install Hexo
- 2 Cangkir Kopi Hitam Pahit

Untuk proses deploy Site kamu nanti akan di pandu lewat Github dulu agar Kamu sekalian punya Subdomain gratis dari github.io tapi untuk referensi proses deploy lainnya bakal saya jelaskan dan kasih referensi lain nya juga. Untuk sekarang langkah awal yang harus Kamu lakukan adalah meneguk KOPI yang udah di buat tadi supaya tutorial hexo berikut ini cepet dipraktekin.

### Install Chocolatey
Apa sih fungsinya? Fungsi ini agar semua proses download package dan software dapat di lakukan dengan cmd atau terminal Kamu. Jadi kegunaannya bukan cuma untuk proses pembuatan blog hexo tapi software open source juga bisa kalian akses dengan mudah tanpa ribet dengan proses download dan ekstrak. Untuk proses instalasi nya silahkan Kamu ikuti intruksi yang ada Situs Chocolatey.

Kalo ada yang males untuk mencet link di atas maka ikuti instruksi berikut.

![Tutorial Hexo](/img/tutorial-membuat-website-dengan-hexo.jpg)

Opsi PERTAMA buka CMD prompt kalian dari start button setelah itu ketik CMD pada kolom pencarian nya dan jangan lupa jalankan pada mode Admin ya kemudian copy paste kode di bawah ini
```
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

Opsi KEDUA jika kalian sudah punya powershell (pada keyboard komputer kalian tekan tombol startbutton+X) maka yang di masukkan adalah kode berikut
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1')) 
```

### Install VScode
Apa itu VScode? itu adalah tools untuk mempermudah proses pengeditan code (NGODING). Ya selamat buat kamu yang ngerasa GAPTEK karena salah satu sisi positif dari memiliki Blog Hexo kamu juga otomatis akan menjadi codingers. Dan yang paling penting ternyata itu gak sesulit yang Kamu bayangin. OK lanjut silahkan copy paste perintah berikut ke CMD kalian
```
choco install vscode 
```

### Install Git (GITHUB)
Jika chocolatey kamu sudah terinstall maka mulai sekarang kamu bakal sangat akrab dengan tampilan itu hehehe. Sekarang lanjut untuk install Git kalian hanya perlu copy paste perintah berikut ke CMD kamu.
```
Choco install git
```
Gampang kan? Dan untuk list download software-software lain kalian bisa bukan web resmi nya chocolatey untuk melihat daftar nya. Karena saat ini kita fokus membuat Hexo maka hanya software serta framework yang di perlukan saja yang akan di instruksikan.


### Install Nodejs
Sekarang kita lanjut untuk instalasi Nodejs ya guys. Apa itu Nodejs? Berhubung disini saya hanya memfokuskan Kamu untuk membuat blog hexo tapi gak ada salah nya untuk mempelajari asal usul nya biar gak penasaran ya. Untuk itu silahkan kalian cari pengertian Nodejs di Codepolitan.

Lanjut untuk proses download nya tetap berlangsung di CMD kamu yaitu dengan perintah berikut
```
Choco install nodejs 
```
Udah berjalan lancar? Kalo sudah yang perlu kamu lakukan sekarang adalah meneguk kopi pahitnya lagi OK? lanjut…

## Panduan Instalasi Hexo
Sekarang perhatikan baik-baik ok? Untuk memulai instalasi Hexo maka yang perlu Kamu lakukan adalah membuat Folder di directory C:
Kalo ribet kalian bisa buat folder manual dulu tapi kalo mau lewat CMD maka Kamu bisa menjalankan perintah berikut di CMD (masukin satu-satu per line)
```
cd C:\ mkdir hexo
```
Saat ini kalian udh ada folder hexo maka kita harus masuk ke folder tersebut dengan perintah
```
cd hexo
```
{% note danger %}
**NOTE** :
mkdir untuk membuat folder sedangkan cd adalah perintah untuk masuk ke suatu folder
{% endnote %}

Sekarang kita mulai proses instalasi Hexo nya ya. pada directory kalian saat ini silahkan masukkan perintah berikut
```
npm install -g hexo-cli
```
Hexo sudah di install sekarang lanjut untuk membuat struktur site hexo pertama Anda. Untukdi bawah ini silahkan sesuaikan dengan kemauan kamu ya yang penting di isi huruf kecil aja semua biar gak ribet. contoh nya blog dan sekali lagi masukkan perintah berikut satu-persatu ke CMD nya ya
```
hexo init <contoh> 
cd <contoh> 
npm install 
```
HORE!!!! Situs hexo pertama Kamu udah jadi untuk melihat bagaimana bentuk site mu secara langsung masukkan perintah berikut
```
hexo server 
```
Setelah itu pastiin kamu punya akses internet dlu ya hehehe setelah itu buka browser kamu dan ketik sesuai yang tertera di CMD yaitu localhost:4000 kemudian ENTER. Sip itu lah site hexo pertama kamu, loh koq begini doank mas bro? hehehe tenang itu adalah tema standar jadi sebelum mau punya tema keren ada baiknya Kamu pelajarin kelebihan serta struktur site nya dulu.

## Kelebihan Blog Hexo
Sebelum melanjutkan ke struktur site hexo nya, ada baik nya Kamu mengetahui secara detail apa sih kelebihan dari Hexo ini karena sekilas Kamu membaca tutorial ini pasti ribet banget keliatan nya dan kalo gak tau kelebihan nya sepertinya Kamu bakal males mencoba nya.

IMOclub akan merangkum beberapa kelebihan framework Hexo ini berdasarkan pengalaman pribadi para webmaster yang sudah malang melintang d dunia blogger. Berikut ini alasannya :
1. Hexo merupakan SSG yang memiliki ratusan plugin pendukung sama seperti wordpress dan di antaranya juga ada banyak untuk keperluan optimasi SEO.
2. Hexo merupakan framework yang di bangun dari NodeJS sehingga untuk urusan speed saat web Kamu live sangat lah cepat(hitungan nya nomor 2 jika Kamu sudah memiliki web dari Gatsby).
3. Hexo sangatlah fleksibel sehingga Kamu dapat meletakkan nya menjadi bagian dari web utama di hosting mu.
4. Berdasarkan pengalaman di SERP dan SEO, Hexo sangatlah cepat untuk di indeks karena di generate menjadi HTML dan jika Kamu mengincar keyword menengah serta melakukan optimasi hanya dengan ONPAGE maka untuk menduduki pajewan sangatlah mudah dengan Hexo ini.
5. Dari sisi security jelas Hexo sangatlah aman akan hasil generate nya berbentuk HTML dan database utamanya adalah komputer mu sendiri.

## Penjelasan Struktur Site Hexo
. 
+-- _config.yml 
+-- package.json 
+-- scaffolds 
+-- source | 
+-- _drafts | 
+-- _posts 
+-- themes 

Struktur site kamu akan seperti itu dan sekarang coba buka langsung pada folder kalian atau untuk mempermudah proses editing sekaligus langsung buka aja lewat VScode lalu pilih File dan Open Folder dan tujukan pada folder site kamu di buat tadi.
Yang harus kalian mengerti adalah membedakan mana folder yang harus di edit dan tidak. Jadi untuk struktur di atas yang bisa Kamu akses hanyalah di bagian /source yaitu segala artikel draft, post, page dan lainnya akan muncul di situ. Sedangkan untuk editting layout sitenya harus Kamu sesuaikan dengan tema masing-masing yang kamu inginkan nantinya.

OK setelah itu kita lanjutkan dengan menginstall tema ya, saya akan contohkan untuk membuat blog dengan tema ICARUS ya yang contoh nya bisa kalian lihat DISINI.
Dan jika kalian mau mencoba tema lainnya kalian bisa langsung buka DISINI dan cari source code Github nya yang biasa ada di footer demo situs yang kamu inginkan.

Sekarang yang akan kita lakukan adalah proses clone tema nya. Kalo kalian CMD kalian sempat tertutup sebelum nya maka silahkan ikut perintah berikut
```
cd C:\hexo\<nama folder kalian>
```
Setelah itu lanjutkan lagi dengan peritah berikut untuk mengcloning tema nya
```
git clone https://github.com/ppoffice/hexo-theme-icarus themes/hexo-theme-icarus
```
Setelah selesai maka buka VScode kamu dan klik di file _config.yml nya dan cari yang ada bagian seperti di bawah ini
{% note danger %}
Extensions
Plugins: https://hexo.io/plugins/
Themes: https://hexo.io/themes/
theme: **landscape**
{% endnote %}

Kemudian ganti tulisan landscape di atas menjadi nama theme yang kalian cloning tadi yaitu hexo-themes-icarus. Setelah itu coba buka CMD kalian dan masukkan perintah
```
hexo server
```
Dan lihat apa sudah berubah tema nya? Kalo sudah selamat tapi belum selesai di situ karena akan percuma sekali kalau hanya berupa localhost bukan? Sok kita lanjut lagi

## Configurasi Blog Hexo
Sekarang kamu sudah berhasil membuat situs Hexo tapi bagaimana cara membuat postingan nya ya? OK tenang sekarang buka kembali CMD kalian dan ikuti intruksi berikut ini
```
hexo new post "blog hexo saya"
```
Silahkan ganti "blog hexo saya" dengan nama yang kalian mau dan ingat di atas adalah struktur nama URL nya bukan TITEL blog ok? Jadi cukup tuliskan singkat saja dan yang paling penting silahkan sesuaikan permalink nya di _config.yml dan cari kemudian ganti permalink menjadi seperti di bawah ini.
{% note success %}
url: https://example,com 
root: / 
permalink: :title/ 
permalink_defaults: 
{% endnote %}
Oh iya untuk URL nya di biarkan aja dulu seperti itu ya. Untuk membuka postingan yang sudah Kamu buat tadi silahkan masuk ke VScode dan buka folder /source>_posts ya di situlah kamu bisa mengedit artikel kamu dan jangan lupa mampir ke panduan penulisan MARKDOWN ya, gak sulit koq sangat enak banget malah menurut saya.

Biasanya untuk setiap tema yang Kamu cloning itu sudah ada panduan lengkap untuk melakukan editing sesuai dengan struktur tema mereka jadi lebih baik untuk custom theme icarus ini kalian bisa langsung praktekkan config nya di BLOG ICARUS.

## Instalasi Plugin Hexo
Sama halnya seperti wordpress di hexo juga ada istilah plugin hanya saja proses aplikasi dan jenis nya memang gak sebanyak wordpress tapi sudah cukup powerful kok. Kalo kamu ikutin docs nya dari icarus di atas juga di jelaskan bagaimana cara nya menginstall plugin dan jika kalian mau eksplorasi sendiri dan sesuaikan dengan kebutuhkan blog hexo kamu maka langsung aja searching di list plugin official nya.

Dan disini saya ingatkan untuk file yang bernama _config.yml kamu akan mendapati 2 file dengan nama tersebut yaitu di folder utama blog kamu dan yang satu lagi ada di folder themes yang kamu cloning.

Jadi ikuti dan bedakan bagian config mana yang di intruksi kan ubah sesuai bagian config.yml nya. Dan untuk plugin ini biasa nya setelah menginstall nya akan di minta untuk menambahkan perintah dan itu kamu masukkan pada _config.yml di folder blog utama Kamu OK? Saya akan contohkan untuk 1 plugin penting yang akan melanjutkan tutorial ini sampai bisa menjadi Site Alive pada Github, jadi buka kembali CMD Kamu dan arahkan ke folder blog utama hexo Kamu dan masukkan perintah berikut untuk menginstall plugin deployer ke Github nya.
```
npm install hexo-deployer-git --save
```
Setelah terinstall buka VScode Kamu dan klik pada _config.yml di folder blog utama hexo Kamu. dan cari kemudian ganti seperti di bawah ini
{% note success %}
You can use this: 
deploy: 
type: 
git repo: <repository url> 
branch: [branch] 
message: [message]
{% endnote %}

### Membuat Subdomain Di Github
Cara pengisian plugin di atas gak akan berfungsi kalo Kamu belum punya akun github jadi silahkan ikuti tutorial membuat akun berikut ini dan membuat subdomain di github secara gratis untuk mendeploy Site Hexo kamu ok?
Saya yakin untuk proses SIGN UP saya gak perlu jelasin secara detail ya kan? hehehe jadi silahkan Daftar akun Github terlebih dahulu dan selesaikan sampai bisa mengakses dashboard nya. Setelah itu liad pada gambar di bawah ini yaitu membuat repository yang nantinya akan bisa menjadi subdomain Kamu.

Setelah itu buat nama nya sesuai dengan username yang Kamu daftarkan contohnya seperti gambar di bawah ini dimana username saya adalah crezenity

ikuti sesuai yang saya tandain di atas di mana jika Kamu punya username bernama contoh maka nama repo nya harus contoh.github.io ngerti ya?
Jika sudah maka yang perlu Kamu lakukan cukup salin URL repo yang baru Kamu buat tadi misal: https://github.com/crezenity/crezenity.github.io
Setelah itu lanjut ke pengisian plugin deployer git sebelumnya jadi untuk contoh kamu ikuti seperti di bawah ini dan yang harus Kamu ganti hanyalah nama URL nya saja.
```
You can use this: 
deploy: 
type: git 
repo: [<repository url>](https://github.com/crezenity/crezenity.github.io) 
branch: master 
message: "{{ now('YYYY-MM-DD HH:mm:ss') }}" 
```

### Live Hexo Di Subdomain Github
Kalo sebelumnya kamu udh edat edit blog kamu sekarang saatnya mendeploy nya supaya kamu bisa memandangnya selain dari localhost hehehe. Jadi sebenarnya cara nya cukup mudah yaitu dengan memasukkan kedua perintah di bawah ini satu-persatu
```
hexo generate 
hexo deploy
```
Biasanya karena kamu buat repo private maka akan diminta verifikasi email dan password di CMD kamu jadi cukup isi aja dan setelah itu buka hasilnya sesuai nama subdomain Kamu misalnya: contoh.github.io
OK gimana ribet gak?

## Kesimpulan
Kalo kamu ada pertanyaan coba lempar di kolom komentar aja ya dan harap maklum dengan tutor nya kalo masih belum jelas. Untuk proses deploy lainnya seperti netlify atau ke hosting kamu sendiri bakal saya buat di lain kesempatan di blog ini berhubung saat ini udah menunjukkan jam 3 PAGI hehehe.
Thanks guys silahkan di share kalo menurut kamu bermanfaat ya.

