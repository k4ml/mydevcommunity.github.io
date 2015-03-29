---
layout: post
title: 'Adakah anda verify ssh fingerprint apabila ssh kali pertama ke server ?'
date: 2015-03-01
author: kamalmustafa
permalink: /adakah-anda-verify-ssh-fingerprint.html
level: 2
summary: >
            Adakah anda *verify* *fingerprint* apabila ssh buat pertama kali ke server ?

            Tulisan ini akan cuba menjelaskan apakah fungsi sebenar disebalik pengesahan
            *fingerprint* yang selalu anda dapat apabila ssh ke server.
---
Sejujurnya, jawapan saya adalah "tidak", pada kebanyakkan masa.

Apakah yang dimaksudkan dengan *ssh fingerprint* ? Anda mungkin biasa dengan soalan
seperti dibawah:-

```
$ ssh 10.0.3.98 -l ubuntu
The authenticity of host '10.0.3.98 (10.0.3.98)' can't be established.
ECDSA key fingerprint is d0:11:fd:03:6b:08:ad:d4:7b:af:17:48:da:ef:24:1f.
Are you sure you want to continue connecting (yes/no)?
```
<!--more-->
Soalan di atas adalah aplikasi SSH meminta kepastian kita sama ada server dengan ID
'd0:11:fd:03:6b:08:ad:d4:7b:af:17:48:da:ef:24:1f' adalah betul server yang kita hendak
hubungi. Ini untuk mengelakkan cubaan untuk menghubungkan kita ke server yang berbeza
dengan tujuan untuk memintas segala bentuk maklumat perhubungan antara kita dan server
tersebut. Ini sudah tentu sangat bahaya kerana kita menyangka perhubungan kita dengan
server tersebut adalah selamat kerana telah dienkrip oleh SSH.


<div class="admonition-warning">
    Protokol baru HTTP/2 bagaimanapun berbeza dengan HTTP/1.1 yang digunakan sekarang
    kerana ia tidak lagi berasaskan teks, tetapi dalam bentuk binari.
</div>
<div>&nbsp;</div>


Sentiasa ajukan persoalan kepada diri sendiri, bagaimana sesuatu benda itu berfungsi dan jalankan eksperimen untuk
mendapatkan jawapannya.

[nc]:http://metak4ml.blogspot.com/2013/05/craft-http-requests-using-nc.html
[http]:https://www.ietf.org/rfc/rfc2616.txt
