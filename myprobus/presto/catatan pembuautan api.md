# catatan pembuatan api standarisasi

### project
1 . penentuan layout
2 . nama setiap layout 
3 . pencocokan api
4 . penamaan api

sangat disarankan dan diharapkan agar pencocokan nama api dan nama layout ... untuk prosses pengerjaan projet untuk memangkas waktu

### do not
cotoh :

- nama layout : Report Overview
- apinya : https://presto-online.barongpos.com/api/homeFb/:outlet?date="date&dept=:dep
- pinya : https://presto-online.barongpos.com/api/ajaxSellProduct?date=:date&outlet=:outlet&tipe=:tipe

antara api dan nama tidak berhubungan sama sekali , jika hanya mengerjakan project yang membutuhkan api 1,
tidak lah masalah , jika da 10 api , akan sangan memakan waktu dan sumberdaya pengingatan yang seharusnya,
bisa dialihkan untuk mengerjakan hal lainnya 

### do

contoh : 

- nama layout : Report Overview
- https://presto-online.barongpos.com/api/ReportOverview?outlet=:outlet&date=:date&dept=:dep

diharapkan untuk kedepan bisa dikerjakan dengn serapi mungkin , dan seefesien mungkin , aga bisa mempercepat pengerjaan project
dan terapkan standarnya 

dan perjayalah , selain di php itu pengerjaan dan pemecahan API sangat sangat ribet, nguras waktu dan pikiran 
dari pembentukan class dr setiap api , pembuatan objek dari isi api secara manual, sampai pencocokan setiap detailnya secara manual ke 
layout, setitik kesalahan di api , bisa berakibat trcker bug sampai 2 hari , pembuautan api asal asalan project yang seharusnya bisa
dikerjakan sebulan bisa molor 2 bulan hanya untuk mencocokan api yang tidak sistematik dan asal jadi , 
setiap kejadian akan di record dan menjadikan kita lebih profetional dengan standar kerja
