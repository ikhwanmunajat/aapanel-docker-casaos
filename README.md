Penerapan Docker aaPanel

Image docker ini dirilis secara resmi oleh aaPanel

Dikelola oleh: aaPanel

Saat ini platform arsitektur x86_64 dan ARM tersedia untuk diunduh


fresh tag berarti panel sudah terpasang tetapi lib dasar belum terpasang, dan pemasangan perangkat lunak pertama akan lebih lambat

lib tag adalah memasang panel dan pustaka dasar, pemasangan menggunakan mirror ini untuk memasang perangkat lunak lebih cepat


lnmp tag adalah memasang panel dan pustaka dasar, dan integrasi LNMP terintegrasi 【Nginx1.22+MySQL5.7+PHP7.4】*tab arm adalah 【MySQL5.6】


lamp tag adalah memasang panel dan pustaka dasar, dan integrasi LAMP terintegrasi 【Apache2.4+MySQL5.7+PHP7.4】*tab arm adalah 【MySQL5.6】

##Cara Menggunakan, Copy pada Docker CLI CasaOS kode berikut:

$docker run -d -p 8886:7800 -p 22:21 -p 443:443 -p 80:80 -p 889:888 -v ~/website_data:/www/wwwroot -v ~/mysql_data:/www/server/data -v ~/vhost:/www/server/panel/vhost aapanel/aapanel:lib

Sekarang Anda dapat mengakses aaPanel di http://youripaddress:8886/ ⁠ dari sistem host Anda.

Entri instalasi default: aapanel

Nama pengguna default: aapanel

Kata sandi default: aapanel123

Kata sandi root default: aapanel123

Analisis penggunaan pelabuhan

Panel Kontrol : 7800
Phpmyadmin : 888

Analisis penggunaan Dir

Data situs web: /www/wwwroot
Data MySQL: /www/server/data
File Vhost: /www/server/panel/vhost

Catatan: setelah penyebaran selesai, harap segera ubah nama pengguna dan kata sandi di pengaturan panel dan tambahkan entri instalasi
