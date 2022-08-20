## Satır Blokları (Row) Kullanımı

Grid sistem, satırlardan(rows) ve sütunlardan(column) oluşur. Bir satır(row) 12 column'dan oluşur. Bu satırları istediğimiz şekilde parçalayabiliriz. Aşağıdaki resimde de görüldüğü gibi istersek bunları 12 eşit parçaya ayırabilir ya da 12'ye tamamlanacak herhangi bir şekilde de bölebiliriz. Örneklerle bunları açıklamaya çalışayım.


![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/Bootstrap-part-2.png)

```html
<div class="row">
  <div class="col">Column</div>
  <div class="col">Column</div>
</div>
```

![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/6of6.PNG)
```html
<div class="row">
  <div class="col">Column</div>
  <div class="col">Column</div>
  <div class="col">Column</div>
</div>
```

![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/3column.PNG)
```html
<div class="row">
  <div class="col">Column</div>
  <div class="col">Column</div>
  <div class="col">Column</div>
  <div class="col">Column</div>
</div>
```

![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/4column.PNG)

Yukarıdaki örneklerde de görüldüğü üzere satırları eşit parçalar halinde column'lara ayırdık. Peki eşit olmayan column'lar yapabilir miyiz? Tabii ki yapabiliriz. Şimdi de örneklerle eşit olmayan column'lar oluşturalım...

- Bu örnekte 2'ye 10'luk bir column oluşturduk.
```html
<div class="row">
  <div class="col-2">2 Column</div>
  <div class="col-10">10 Column</div> 
</div>
```

![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/img-2.PNG)

- Alttaki örnekte ise satırı 8'e 4'lük bir column halinde bölmüş olduk.
```html
<div class="row">
  <div class="col-4">4 Column</div>
  <div class="col-8">8 Column</div> 
</div>
```
![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/8of4.PNG)

- Satırları böldüğümüzde araya ya da herhangi bir kenara boşluk ekleyebiliriz onu da şu şekilde gösterelim;
```html
<div class="row">
  <div class="col-4 mr-auto">4 Column</div> <--mr: margin right (sağından boşluk bırak)-->
  <div class="col-5">5 Column</div> 
</div>

<div class="row">
  <div class="col-4"></div>
  <div class="col-5 ml- auto"></div> <--ml: margin left (solundan boşluk bırak)-->
</div>
```
![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/img-7.PNG)

İki kod bloğunun çıktısı aynı olacak fakat birinci col sağından sola doğru itecek ve boşluk bırakacak diğerinde ise tam tersi ikinci col solundan sağa doğru iterek boşluk bırakacak.

- Bir satırı 4'e 8'lik column'lar halinde böldüğümüzü düşünelim bu satırlar daha sonra kendi içlerinde de tekrar 12'lik column gibi düşünülerek bölünebilir. Bunlara iç içe satırlar diyebiliriz. Aşağıdaki örnekte önce satırı 4'e 8'lik olacak şekilde parçaladık daha sonra 8'lik column'u kendi içinde eşit 2 parçaya böldük.
```html
    <div class="row">
			<div class="col-4 border">4 Column</div>
			<div class="col-8 border">8 Column
				
				<div class="row">
					<div class="col bg-primary">6 Column</div> <!--bg: background, primary:color-->
					<div class="col bg-danger">6 Column</div>  <!--bg: background, primary:color-->
				</div>
			
			
			</div>
		</div>
```

![](https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/bootstrap/bootstrap-satir-bloklari-row-kullanimi/figures/img8.PNG)

