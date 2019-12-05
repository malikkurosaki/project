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

__semua data adalah string__

contoh : 

`[{"data":"10"}] jangan [{"data":10}]`

__usahakan tidak ada null__

contoh : 

`[{"data":null}]`

__usahakan tidak ada bouble (koma)__

contoh :

`[{"data":"10.00"}]`

__setiap api adalah per layout single dimentional__

contoh : 

```javascript
[{"key":"val"},{"key":"val"}] seterusnya

// jangan

{"object":[{"key:"value"}]}

// jangan

{{"key":"value"},{"key":"value"}}
```

jika berhadapan dengan int atau integer atau angka , maka defaultnya untuk nilai terkecil adalah "0" noll , bukan " ", (kosong) atau empty, karena mesin tidak mengerti angka yang empty , empty hanya untuk list, dan default angka adalah `0`

sebisa mungkin hal sepele kita antisipasi sedini mungkin , jangan sampai ketika setelah di tangan client , terjadi error padahal bisa antisipasi sejak dini
