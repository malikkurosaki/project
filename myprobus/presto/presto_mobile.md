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

```json
[{"kode_out":"RST","nama_out":"RESTAURANT"},{"kode_out":"MSC","nama_out":"MISCELLANEOUS"},{"kode_out":"all","nama_out":"All Outlet"}]
```

---

__get dep / departement__

- _untuk mendapatkan nama dep_

https://presto-online.barongpos.com/api/getDept

```json
[{"nama_dept":"CRISPY PIZZA","unit_bisnis":"CRISPY PIZZA"},{"nama_dept":"CRISPY KROBOKAN","unit_bisnis":"CRISPY PIZZA"},{"nama_dept":"CRISPY BANDUNG","unit_bisnis":"CRISPY PIZZA"},{"nama_dept":"CRISPY DRUPADI","unit_bisnis":"CRISPY PIZZA"},{"nama_dept":"CRISPY TEUKU UMAR","unit_bisnis":"CRISPY PIZZA"},{"nama_dept":"CRISPY KUTA","unit_bisnis":"CRISPY PIZZA"},{"nama_dept":"all","unit_bisnis":"all"}]
```

---

__Fb Home__

- outlet > kode outlet
- date > tanggal
- dept > nama dept

https://presto-online.barongpos.com/api/homeFb/outlet?date=:date&dept=:dept

```javascript
[{"title":"gross","today":"0","yesterday":"0"},{"title":"net","today":"0","yesterday":"0"},{"title":"bills","today":"0","yesterday":"0"},{"title":"diskon","today":"0","yesterday":"0"},{"title":"compliment","today":"0","yesterday":"0"},{"title":"food","today":"0","yesterday":"0"},{"title":"beverage","today":"0","yesterday":"0"},{"title":"sisha","today":"0","yesterday":"0"},{"title":"other","today":"0","yesterday":"0"},{"title":"avgpax","today":"0","yesterday":"0"},{"title":"avgbill","today":"0","yesterday":"0"}]
```

---

__payment fb__

- outlet > kode outlet

https://presto-online.barongpos.com/api/paymentFb/outlet

```json
[{"id":"cash","type":"Cash IDR","value":"0"},{"id":"foreign_cash","type":"Foreign Cash","value":"0"},{"id":"cc1","type":"Credit Card 1","value":"0"},{"id":"cc2","type":"Credit Card 2","value":"0"},{"id":"arNominal","type":"AR Nominal","value":"0"},{"id":"chargeToRoom","type":"Charge to Room","value":"0"},{"id":"voucherBf","type":"Voucher Breakfast","value":"0"},{"id":"voucherPromo","type":"Voucher Promo","value":"0"},{"id":"clearingDp","type":"Clearing DP","value":"0"},{"id":"forex","type":"Forex Gain\/Loss","value":"0"},{"id":"guestTiping","type":"Guest Tiping","value":"0"}]
```

---

__product sales beverage__

- outlet > kode outlet
- date > tanggal
- dept > nama dept
                                   
https://presto-online.barongpos.com/api/productSales/beverage/outlet?date=:date&dept=:dept

_contoh_

> https://presto-online.barongpos.com/api/productSales/beverage/rst?date=2019-11-27&dept=all

```json
[{"name":"BINTANG","qty":"10","total":"260000","price":"26000"},{"name":"COCA COLA","qty":"9","total":"115000","price":"12777.77777778"},{"name":"NESTLE FREE REFILL","qty":"8","total":"84000","price":"10500"},{"name":"WATER","qty":"6","total":"57000","price":"9500"},{"name":"WATERMELON JUICE","qty":"6","total":"94800","price":"15800"},{"name":"SHAKERATO","qty":"4","total":"32000","price":"8000"},{"name":"AQUA 330 ML","qty":"3","total":"15000","price":"5000"},{"name":"CAPPUCCINO","qty":"3","total":"54000","price":"18000"},{"name":"SPRITE","qty":"3","total":"37500","price":"12500"},{"name":"CARAMEL LATTE","qty":"3","total":"54000","price":"18000"}]
```

---

__product sales food__

- outlet > kode outlet
- date > tanggal
- dept > nama dept

https://presto-online.barongpos.com/api/productSales/food/outlet?date=:date&dept=:dept

_contoh_

> https://presto-online.barongpos.com/api/productSales/food/rst?date=2019-11-27&dept=all

```json
[{"name":"BOX PERSONAL","qty":"60","total":"85550","price":"1425.83333333"},{"name":"BOX REGULAR","qty":"41","total":"51750","price":"1262.19512195"},{"name":"MARGARITA PERS.","qty":"39","total":"331260","price":"8493.84615385"},{"name":"TUNA SALAD","qty":"25","total":"626180","price":"25047.2"},{"name":"CAPRICCIOSA PERSONAL","qty":"16","total":"395100","price":"24693.75"},{"name":"MARGHERITA REGULAR.","qty":"14","total":"569400","price":"40671.42857143"},{"name":"CHEESE CROQUETTE SMALL","qty":"11","total":"110880","price":"10080"},{"name":"CHICKEN SALAD","qty":"11","total":"262900","price":"23900"},{"name":"HAWAIIANA PERS.","qty":"10","total":"199480","price":"19948"},{"name":"PEPPERONI REGULAR.","qty":"10","total":"511200","price":"51120"}]
```

---

__transaction Summary__

- outlet > kode outlet

https://presto-online.barongpos.com/api/transactionSummary/outlet

```json
[{"type":"open","qty":"0","net":"0"},{"type":"paid","qty":"0","net":"0"},{"type":"close","qty":"0","net":"0"},{"type":"void","qty":"0","net":"0"},{"type":"revisi","qty":"0","net":"0"}]
```

---

__sales performance__

- outlet > kode outlet

https://presto-online.barongpos.com/api/salesPerformance/outlet

```json
[{"month":"1","value":"0"},{"month":"2","value":"0"},{"month":"3","value":"0"},{"month":"4","value":"0"},{"month":"5","value":"0"},{"month":"6","value":"0"},{"month":"7","value":"0"},{"month":"8","value":"0"},{"month":"9","value":"0"},{"month":"10","value":"0"},{"month":"11","value":"0"}]
```

---

__sales trafic__

- outlet > kode outlet

https://presto-online.barongpos.com/api/salesTrafic/outlet

```json
[{"date":"Sunday","value":"0"},{"date":"Monday","value":"0"},{"date":"Tuesday","value":"0"},{"date":"Wednesday","value":"0"},{"date":"Thursday","value":"0"},{"date":"Friday","value":"0"},{"date":"Saturday","value":"0"}]
```

---

__report revenue__

- date > tnggal
- outlet > kode outlet
- office > nama dept

https://presto-online.barongpos.com/api/reportDailyRevenue?date=:date&office=:office&outlet=:outlet

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



