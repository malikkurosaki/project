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

_contoh_

https://presto-online.barongpos.com/api/homeFb/all?date=2019-11-28&dept=all

```javascript
[{"title":"gross","today":"0","yesterday":"0"},{"title":"net","today":"0","yesterday":"0"},{"title":"bills","today":"0","yesterday":"0"},{"title":"diskon","today":"0","yesterday":"0"},{"title":"compliment","today":"0","yesterday":"0"},{"title":"food","today":"0","yesterday":"0"},{"title":"beverage","today":"0","yesterday":"0"},{"title":"sisha","today":"0","yesterday":"0"},{"title":"other","today":"0","yesterday":"0"},{"title":"avgpax","today":"0","yesterday":"0"},{"title":"avgbill","today":"0","yesterday":"0"}]
```

---

__payment fb__

- outlet > kode outlet

https://presto-online.barongpos.com/api/paymentFb/outlet?date=:date&dept=:dept

_contoh_

https://presto-online.barongpos.com/api/paymentFb/all?date=2019-11-28&dept=all

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

https://presto-online.barongpos.com/api/transactionSummary/outlet?date=:date&dept=:dept

_contoh_

https://presto-online.barongpos.com/api/transactionSummary/all?date=2019-11-28&dept=all

```json
[{"type":"open","qty":"0","net":"0"},{"type":"paid","qty":"0","net":"0"},{"type":"close","qty":"0","net":"0"},{"type":"void","qty":"0","net":"0"},{"type":"revisi","qty":"0","net":"0"}]
```

---

__sales performance__

- outlet > kode outlet
- date > tanggal
- dept > nama dept

https://presto-online.barongpos.com/api/salesPerformance/outlet?date=:date&dept=:dept

_contoh_

https://presto-online.barongpos.com/api/salesPerformance/all?date=2019-11-28&dept=all

```json
[{"month":"1","value":"0"},{"month":"2","value":"0"},{"month":"3","value":"0"},{"month":"4","value":"0"},{"month":"5","value":"0"},{"month":"6","value":"0"},{"month":"7","value":"0"},{"month":"8","value":"0"},{"month":"9","value":"0"},{"month":"10","value":"0"},{"month":"11","value":"0"}]
```

---

__sales trafic__

- outlet > kode outlet
- date > tanggal
- dept > nama dept

https://presto-online.barongpos.com/api/salesTrafic/outlet?date=:date&dept=:dept

_contoh_

https://presto-online.barongpos.com/api/salesTrafic/all?date=2019-11-28&dept=all

```json
[{"date":"Sunday","value":"0"},{"date":"Monday","value":"0"},{"date":"Tuesday","value":"0"},{"date":"Wednesday","value":"0"},{"date":"Thursday","value":"0"},{"date":"Friday","value":"0"},{"date":"Saturday","value":"0"}]
```

---

__report revenue__

- date > tnggal
- outlet > kode outlet
- office > nama dept

https://presto-online.barongpos.com/api/reportDailyRevenue?date=:date&office=:office&outlet=:outlet

_contoh_

https://presto-online.barongpos.com/api/reportDailyRevenue?date=2019-11-28&office=all&outlet=all

```json
[{"today":"","mtd":"","lmd":"","ytd":"","title":""},{"today":5289120,"mtd":305083736,"lmd":309686879,"ytd":2472797345,"title":"FOOD"},{"today":1176214,"mtd":53020313,"lmd":53334085,"ytd":437290654,"title":"BEVERAGE"},{"today":0,"mtd":498000,"lmd":747000,"ytd":2461429,"title":"OTHERS"},{"today":6465334,"mtd":358602049,"lmd":363767964,"ytd":2912549428,"title":"SUBTOTAL NET REVENUE"},{"today":323142,"mtd":17897441,"lmd":18143283,"ytd":145443040,"title":"SERVICE"},{"today":678842,"mtd":37624710,"lmd":38153678,"ytd":305674982,"title":"TAX"},{"today":"","mtd":"","lmd":"","ytd":"","title":""},{"today":7467318,"mtd":414124200,"lmd":420064925,"ytd":3363667450,"title":"TOTAL GROSS REVENUE"},{"today":"","mtd":"","lmd":"","ytd":"","title":""},{"today":3874407,"mtd":264408286,"lmd":278550084,"ytd":2348768428,"title":"PAID BY CASH"},{"today":3592911,"mtd":148775824,"lmd":141365351,"ytd":1001396374,"title":"PAID BY CREDIT ARD"},{"today":0,"mtd":40590,"lmd":145090,"ytd":1481123,"title":"PAID BY VOUCHER"},{"today":0,"mtd":0,"lmd":24200,"ytd":10623967,"title":"AR CCOUNT"},{"today":0,"mtd":0,"lmd":0,"ytd":0,"title":"CHARGE TO ROOM"},{"today":0,"mtd":0,"lmd":0,"ytd":771898,"title":"DISCOUNT PAYMENT"},{"today":"","mtd":"","lmd":"","ytd":"","title":""},{"today":7467318,"mtd":413224700,"lmd":420084725,"ytd":3363041790,"title":"TOTAL PAYMENT"}]

```

---

__report Product Favorite__

- date > tanggal
- outlet > nama dept

https://presto-online.barongpos.com/api/reportProductFav?date=:date&outlet=:outlet

_contoh_

https://presto-online.barongpos.com/api/reportProductFav?date=2019-11-28&outlet=all


```json
[{"kode":"RST.0210       ","nama_product":"BOX PERSONAL","qty":2184,"price":"1.488"},{"kode":"RST.0211       ","nama_product":"BOX REGULAR","qty":1963,"price":"2.516"},{"kode":"RST.0001       ","nama_product":"MARGARITA PERS.","qty":877,"price":"13.222"},{"kode":"RST.0018       ","nama_product":"MARGHERITA REGULAR.","qty":734,"price":"44.086"},{"kode":"RST.0004       ","nama_product":"PEPPERONI PERS.","qty":564,"price":"25.429"},{"kode":"RST.0217       ","nama_product":"TUNA SALAD","qty":518,"price":"27.446"},{"kode":"RST.0292       ","nama_product":"CAPRICCIOSA PERSONAL","qty":518,"price":"28.091"},{"kode":"RST.0021       ","nama_product":"PEPPERONI REGULAR.","qty":394,"price":"57.394"},{"kode":"RST.0290       ","nama_product":"HAM & MUSHROOM PERSONAL","qty":362,"price":"29.762"},{"kode":"RST.0024       ","nama_product":"HAWAIIANA REGULAR.","qty":348,"price":"50.201"},{"kode":"RST.0218       ","nama_product":"CHICKEN SALAD","qty":325,"price":"27.244"},{"kode":"RST.0123       ","nama_product":"WATER","qty":298,"price":"11.332"},{"kode":"RST.0124       ","nama_product":"COCA COLA","qty":296,"price":"15.333"},{"kode":"RST.0025       ","nama_product":"BBQ CHICKEN REGULAR.","qty":261,"price":"55.131"},{"kode":"RST.0007       ","nama_product":"HAWAIIANA PERS.","qty":242,"price":"22.551"},{"kode":"RST.0037       ","nama_product":"CHEESE CROQUETTE SMALL","qty":239,"price":"10.557"},{"kode":"RST.0038       ","nama_product":"CHEESE CROQUETTE LARGE","qty":236,"price":"21.685"},{"kode":"RST.0232       ","nama_product":"ICE LEMON TEA","qty":230,"price":"5.339"},{"kode":"RST.0293       ","nama_product":"CAPRICCIOSA REGULAR","qty":226,"price":"53.049"},{"kode":"RST.0023       ","nama_product":"FRENCH FRIES LARGE","qty":207,"price":"22.516"},{"kode":"RST.0236       ","nama_product":"BURGER MANIA","qty":197,"price":"37.738"},{"kode":"RST.0137       ","nama_product":"BINTANG","qty":193,"price":"32.842"},{"kode":"RST.0291       ","nama_product":"HAM & MUSROOM REGULAR","qty":187,"price":"56.230"},{"kode":"RST.0008       ","nama_product":"BBQ CHICKEN PERS.","qty":184,"price":"24.831"},{"kode":"RST.0022       ","nama_product":"MEAT LOVE REGULAR.","qty":172,"price":"58.980"},{"kode":"RST.0220       ","nama_product":"CHEESE CROQUETTE DEAL","qty":164,"price":"11.872"},{"kode":"RST.0006       ","nama_product":"FRENCH FRIES SMALL","qty":155,"price":"10.998"},{"kode":"RST.0005       ","nama_product":"MEAT LOVE PERS.","qty":154,"price":"26.827"},{"kode":"RST.0258       ","nama_product":"CHEESE CAKE STRAWBERRY","qty":146,"price":"20.499"},{"kode":"RST.0066       ","nama_product":"CAPPUCCINO","qty":136,"price":"19.322"},{"kode":"RST.0238       ","nama_product":"MILO","qty":134,"price":"13.831"},{"kode":"RST.0244       ","nama_product":"OREO SHAKE","qty":129,"price":"21.341"},{"kode":"RST.0222       ","nama_product":"FRENCH FRIES DEAL","qty":125,"price":"12.999"},{"kode":"RST.0010       ","nama_product":"TUNA PERS.","qty":121,"price":"21.062"},{"kode":"RST.0060       ","nama_product":"BLACK COFFEE","qty":121,"price":"9.226"},{"kode":"RST.0011       ","nama_product":"CHOCO BANANA PERS.","qty":119,"price":"20.997"},{"kode":"RST.0295       ","nama_product":"CHEESE REGULAR","qty":111,"price":"60.872"},{"kode":"RST.0027       ","nama_product":"TUNA REGULAR.","qty":108,"price":"51.639"},{"kode":"RST.0020       ","nama_product":"VEGI REGULAR.","qty":106,"price":"43.784"},{"kode":"RST.0130       ","nama_product":"WATERMELON JUICE","qty":104,"price":"17.696"},{"kode":"RST.0257       ","nama_product":"TIRAMISU","qty":101,"price":"22.326"},{"kode":"RST.0229       ","nama_product":"ESPRESSO","qty":95,"price":"11.059"},{"kode":"RST.0039       ","nama_product":"CHICKEN CROQUETTE SMALL","qty":88,"price":"10.752"},{"kode":"RST.0125       ","nama_product":"DIET COKE","qty":87,"price":"14.740"},{"kode":"RST.0240       ","nama_product":"HAZELNUT CAPPUCINO","qty":86,"price":"18.966"},{"kode":"RST.0219       ","nama_product":"BEEF BOLOGNESE LASAGNA","qty":84,"price":"39.840"},{"kode":"RST.0228       ","nama_product":"ORANGE JUICE","qty":83,"price":"17.380"},{"kode":"RST.0136       ","nama_product":"TEA SOSRO ORIGINAL","qty":83,"price":"3.125"},{"kode":"RST.0227       ","nama_product":"CARAMEL PUDDING","qty":82,"price":"17.443"},{"kode":"RST.0040       ","nama_product":"CHICKEN CROQUETTE LARGE","qty":82,"price":"20.084"},{"kode":"RST.0294       ","nama_product":"CHEESE PERSONAL","qty":73,"price":"26.998"},{"kode":"RST.0131       ","nama_product":"LIME JUICE","qty":72,"price":"17.262"},{"kode":"RST.0126       ","nama_product":"SPRITE","qty":72,"price":"15.583"},{"kode":"RST.0061       ","nama_product":"CAFFE LATTE","qty":70,"price":"18.635"},{"kode":"RST.0035       ","nama_product":"FRENCH PIZZA REGULAR","qty":67,"price":"46.025"},{"kode":"RST.0003       ","nama_product":"VEGI PERS.","qty":62,"price":"17.461"},{"kode":"RST.0243       ","nama_product":"STRAWBERRY SHAKE","qty":60,"price":"20.133"},{"kode":"RST.0242       ","nama_product":"MACHA LATTE","qty":59,"price":"16.166"},{"kode":"RST.0239       ","nama_product":"SHAKERATO","qty":58,"price":"9.224"},{"kode":"RST.0221       ","nama_product":"CHICKEN CROQUETTE DEAL","qty":58,"price":"11.772"},{"kode":"RST.0234       ","nama_product":"BEEF BOLOGNESE LASAGNA TAKE AWAY","qty":57,"price":"50.087"},{"kode":"RST.0179       ","nama_product":"CARAMEL LATTE","qty":57,"price":"19.067"},{"kode":"RST.0036       ","nama_product":"FRENCH PIZZA PERS.","qty":56,"price":"19.827"},{"kode":"RST.0133       ","nama_product":"ICE SHAKEN LEMON TEA SMALL","qty":52,"price":"11.122"},{"kode":"RST.0138       ","nama_product":"POCARI","qty":52,"price":"14.022"},{"kode":"RST.0215       ","nama_product":"SOSRO FRUIT TEA GUAVA","qty":48,"price":"6.098"},{"kode":"RST.0237       ","nama_product":"MACCHIATO","qty":45,"price":"9.040"},{"kode":"RST.0128       ","nama_product":"SODA WATER","qty":44,"price":"20.690"},{"kode":"RST.0224       ","nama_product":"ICE CREAM CHOCOLATE","qty":43,"price":"20.761"},{"kode":"RST.0009       ","nama_product":"SHRIMP PERS.","qty":43,"price":"20.657"},{"kode":"RST.0223       ","nama_product":"ICE CREAM PLAN","qty":41,"price":"20.170"},{"kode":"RST.0129       ","nama_product":"PAPAYA JUICE","qty":41,"price":"19.332"},{"kode":"RST.0241       ","nama_product":"CAFE DI PALMA","qty":38,"price":"16.889"},{"kode":"RST.0028       ","nama_product":"CHOCO BANANA REGULAR.","qty":37,"price":"48.120"},{"kode":"RST.0026       ","nama_product":"SHRIMP REGULAR.","qty":37,"price":"51.898"},{"kode":"RST.0256       ","nama_product":"BINTANG RADLER","qty":36,"price":"32.741"},{"kode":"RST.0247       ","nama_product":"MINT","qty":35,"price":"15.981"},{"kode":"RST.0248       ","nama_product":"FANTA GEMBIRA","qty":34,"price":"17.084"},{"kode":"RST.0214       ","nama_product":"SOSRO FRUIT TEA APPLE","qty":32,"price":"11.452"},{"kode":"RST.0226       ","nama_product":"CRISPY PINEAPPLE STICK","qty":32,"price":"16.954"},{"kode":"RST.0245       ","nama_product":"STRAWBERRY GEMBIRA","qty":30,"price":"16.011"},{"kode":"RST.0225       ","nama_product":"ICE CREAM STRAWBERRY","qty":30,"price":"23.385"},{"kode":"RST.0267       ","nama_product":"EXT. MOZZA PIZZA PERS","qty":30,"price":"5.192"},{"kode":"RST.0299       ","nama_product":"REGULAR EXTR. MUSHROOM 50 GR","qty":29,"price":"7.304"},{"kode":"RST.0246       ","nama_product":"MANGGO","qty":28,"price":"15.236"},{"kode":"RST.0216       ","nama_product":"SOSRO FRUIT TEA BLACKURANT","qty":28,"price":"13.500"},{"kode":"RST.0127       ","nama_product":"FANTA STRAWBERRY","qty":26,"price":"13.077"},{"kode":"RST.0279       ","nama_product":"EXT. MOZZA REG","qty":23,"price":"12.435"},{"kode":"RST.0233       ","nama_product":"SOSRO FRUIT TEA STRAWBERRY","qty":23,"price":"10.227"},{"kode":"RST.0235       ","nama_product":"SOSRO LESS SUGAR","qty":20,"price":"11.875"},{"kode":"RST.0249       ","nama_product":"CAFE LATTE","qty":19,"price":"20.118"},{"kode":"RST.0300       ","nama_product":"PEPPERONI PIZZA 15 CM + FRUIT TEA","qty":19,"price":"32.345"},{"kode":"RST.0301       ","nama_product":"BBQ CHICKENT PIZZA15 CM+ FRUIT TEA","qty":19,"price":"42.844"},{"kode":"RST.0302       ","nama_product":"PAKET MARGHERITA PIZZA 25CM+ FRUIT TEA","qty":18,"price":"54.989"},{"kode":"RST.0285       ","nama_product":"EXT. OLIVE REG","qty":18,"price":"3.176"},{"kode":"RST.0263       ","nama_product":"AQUA 330 ML","qty":16,"price":"5.333"},{"kode":"RST.0282       ","nama_product":"EXT. HAM REG","qty":14,"price":"4.000"},{"kode":"RST.0307       ","nama_product":"NESTLE FREE REFILL","qty":13,"price":"12.000"},{"kode":"RST.0303       ","nama_product":"HAWAIIANA PIZZA 25CM+FRUIT TEA","qty":12,"price":"71.060"},{"kode":"RST.0288       ","nama_product":"EXT. SALAMI REG","qty":11,"price":"8.800"},{"kode":"RST.0284       ","nama_product":"EXT. PINEAPPLE REG","qty":11,"price":"4.400"},{"kode":"RST.0251       ","nama_product":"STRONGBOW","qty":11,"price":"35.000"},{"kode":"RST.0062       ","nama_product":"CARAMEL CAFE LATTE","qty":10,"price":"20.300"},{"kode":"RST.0250       ","nama_product":"HEINEKEN","qty":10,"price":"38.889"},{"kode":"RST.0281       ","nama_product":"EXT. ONION REG","qty":9,"price":"3.000"},{"kode":"RST.0271       ","nama_product":"EXT. HAM PERS","qty":9,"price":"2.250"},{"kode":"RST.0273       ","nama_product":"EXT. PINEAPPLE PERS","qty":9,"price":"2.250"},{"kode":"RST.0277       ","nama_product":"EXT. SALAMI PERS","qty":7,"price":"4.000"},{"kode":"RST.0230       ","nama_product":"AMERICANO","qty":6,"price":"11.880"},{"kode":"MSC.0001       ","nama_product":"BAG","qty":6,"price":"13.000"},{"kode":"RST.0274       ","nama_product":"EXT. OLIVE PERS","qty":6,"price":"1.800"},{"kode":"RST.0252       ","nama_product":"STRONGBOW DARK","qty":5,"price":"35.000"},{"kode":"RST.0260       ","nama_product":"FRUIT SALAD","qty":4,"price":"19.800"},{"kode":"RST.0283       ","nama_product":"EXT. BBQ REG","qty":4,"price":"9.000"},{"kode":"RST.0298       ","nama_product":"PERSONAL EXTRA. MUSHROOM 25 GR","qty":4,"price":"4.000"},{"kode":"RST.0272       ","nama_product":"EXT. BBQ PERS","qty":3,"price":"4.500"},{"kode":"RST.0276       ","nama_product":"EXT. SHRIMP PERS","qty":3,"price":"2.500"},{"kode":"RST.0289       ","nama_product":"EXT. F.F. REG","qty":3,"price":"9.000"},{"kode":"RST.0280       ","nama_product":"EXT. ZUCCHINE REG","qty":3,"price":"3.000"},{"kode":"RST.0270       ","nama_product":"EXT. ONION PERS","qty":3,"price":"1.500"},{"kode":"RST.0306       ","nama_product":"PIZZA CAPRICCIOSA REG PROMO GOJEK","qty":2,"price":"0"},{"kode":"RST.0305       ","nama_product":"PIZZA HAM &MUSHROOM REG PROMO GOJEK","qty":2,"price":"0"},{"kode":"MSC.0002       ","nama_product":"COFFEE JAVA BEEN","qty":2,"price":"210.000"},{"kode":"RST.0286       ","nama_product":"EXT, TUNA REG","qty":2,"price":"16.000"},{"kode":"RST.0268       ","nama_product":"EXT. ZUCCHINE PERS","qty":1,"price":"1.500"},{"kode":"RST.0287       ","nama_product":"EXT. SHRIMP REG","qty":1,"price":"5.000"},{"kode":"RST.0269       ","nama_product":"EXT. ONION PERS","qty":1,"price":"1.500"},{"kode":"RST.0253       ","nama_product":"5 BINTANG BUCKET","qty":1,"price":"110.000"},{"kode":"RST.0275       ","nama_product":"EXT. TUNA PERS","qty":1,"price":"8.000"}]

```

---

__report kasir__

- date > tanggal
- seOutlet > nama dept

https://presto-online.barongpos.com/api/reportKasir?date=:date&setOutlet=:setOutlet

_contoh_

https://presto-online.barongpos.com/api/reportKasir?date=2019-11-28&setOutlet=all

```json
[{"label":"Sunday","value":"0.00"},{"label":"Monday","value":"0.00"},{"label":"Tuesday","value":"0.00"},{"label":"Wednesday","value":"0.00"},{"label":"Thursday","value":"0.00"},{"label":"Friday","value":"0.00"},{"label":"Saturday","value":"0.00"}]
```

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

_contoh_

https://presto-online.barongpos.com/api/ajaxBestOutlet?date=2019-11-28&outlet=CRISPY%20PIZZA&tipe=YTD

```json
[{"label":"Jan","value":"111739870.00"},{"label":"Mar","value":"121471262.00"},{"label":"Mar","value":"138569362.00"},{"label":"Apr","value":"135891418.00"},{"label":"May","value":"152101801.00"},{"label":"Jun","value":"155449823.00"},{"label":"Jul","value":"154472455.00"},{"label":"Aug","value":"156406687.00"},{"label":"Sep","value":"137684707.00"},{"label":"Oct","value":"146941835.00"},{"label":"Nov","value":"121124751.00"}]
```

--- 

__ajax sales product__

- date > tanggal
- outlet > kode outlet
- tipe 
  - mtd
  - dtd
- default mtd

https://presto-online.barongpos.com/api/ajaxSellProduct?date=:date&outlet=:outlet&tipe=:tipe

_contoh_

https://presto-online.barongpos.com/api/ajaxSellProduct?date=2019-11-28&outlet=&tipe=YTD



---

__ajax analisis by time__

- date > tanggal
- outlet > kode outlet
- tipe 
  - mtd
  - dtd
- default mtd

https://presto-online.barongpos.com/api/ajaxAnalisisByTime?date=:date&outlet=:outlet&tipe=:tipe

_contoh_

https://presto-online.barongpos.com/api/ajaxAnalisisByTime?date=2019-11-28&outlet=&tipe=MTD

```json
[{"label":"Breakfast","value":"11362457.00"},{"label":"Lunch","value":"31392150.00"},{"label":"Coffee break","value":"0.00"},{"label":"Dinner","value":"95011889.00"}]
```

---

__ajax avarage__

- date > tanggal
- outlet kode outlet
- tipe 
  - ydt
  - dtd
- default ytd

https://presto-online.barongpos.com/api/ajaxAnalisisAverage?date=:date&outlet=:outlet&tipe=:tipe

_contoh_

https://presto-online.barongpos.com/api/ajaxAnalisisAverage?date=2019-11-28&outlet=&tipe=YTD

```json
[{"label":"January","value":42694.974845542805},{"label":"February","value":44564.57161016949},{"label":"March","value":55494.55781683626},{"label":"April","value":52666.547448522826},{"label":"May","value":48680.873614190685},{"label":"June","value":49702.591211226},{"label":"July","value":53498.8972},{"label":"August","value":56292.979218620116},{"label":"September","value":55063.92563510393},{"label":"October","value":56697.91002227172},{"label":"November","value":52667.51104417671}]
```



