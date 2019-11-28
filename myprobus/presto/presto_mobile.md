# Preto Mobile

### url presto app
> https://presto-online.barongpos.com/home
>
> superadministrator@app.com
>
> password

### Api

__get outlet__

- _untuk mendapatkan nama outlet_

https://presto-online.barongpos.com/api/getOutlets

---

__get dep / departement__

- _untuk mendapatkan nama dep_

https://presto-online.barongpos.com/api/getDept

---

__Fb Home__

- outlet

https://presto-online.barongpos.com/api/homeFb/outlet

---

__payment fb__

- outlet

https://presto-online.barongpos.com/api/paymentFb/outlet

---

__product sales beverage__

- outlet > kode outlet
- date > tanggal
- dept > nama dept

https://presto-online.barongpos.com/api/productSales/beverage/outlet?date=:date&dept=:dept

---

__product sales food__

- outlet > kode outlet
- date > tanggal
- dept > nama dept

https://presto-online.barongpos.com/api/productSales/food/outlet?date=:date&dept=:dept

---

__transaction Summary__

- outlet > kode outlet

https://presto-online.barongpos.com/api/transactionSummary/outlet

---

__sales performance__

- outlet > kode outlet

https://presto-online.barongpos.com/api/salesPerformance/outlet

---

__sales trafic__

- outlet > kode outlet

https://presto-online.barongpos.com/api/salesTrafic/outlet

---

__report revenue__

- outlet > kode outlet
- office > nama dept

https://presto-online.barongpos.com/api/reportDailyRevenue?date=:date&office=:office?outlet=:outlet

---

__report Product Favorite__

- date > tanggal
- outlet > nama dept

https://presto-online.barongpos.com/api/reportProductFav?date=:date&outlet=:outlet

---

__report kasir__

- date > tanggal
- seOutlet > nama dept

https://presto-online.barongpos.com/api/reportKasir?date=:date&setOutlet=:setOutlet

---

__ajax best outlet__

- data > tanggal 
- outlet > kode outlet
- tipe 
  - wtd
  - ytd
  - mtd
- default ytd

https://presto-online.barongpos.com/api/ajaxBestOutlet?date=:date&outlet=:outlet&tipe=:tipe

--- 

__ajax sales product__

- date > tanggal
- outlet > kode outlet
- tipe 
  - mtd
  - dtd
- default mtd

https://presto-online.barongpos.com/api/ajaxSellProduct?date=:date&outlet=:outlet&tipe=:tipe

---

__ajax analisis by time__

- date > tanggal
- outlet > kode outlet
- tipe 
  - mtd
  - dtd
- default mtd

https://presto-online.barongpos.com/api/ajaxAnalisisByTime?date=:date&outlet=:outlet&tipe=:tipe

---

__ajax avarage__

- date > tanggal
- outlet kode outlet
- tipe 
  - ydt
  - dtd
- default ytd

https://presto-online.barongpos.com/api/ajaxAnalisisAverage?date=:date&outlet=:outlet&tipe=:tipe



