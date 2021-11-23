<div dir='rtl' align="justify">
 
 #  مینی پروژه سوم
 
در این پروژه قرار است عملکرد یک ماشین حساب را شبیه سازی کنیم. عملیات جمع (+)، تفریق (-)، ضرب (*)، تقسیم (/)، توان (^) ، را باید پیاده سازی کنید.
با توجه به اینکه ماشین حساب باید پرانتز گداری عبارات را پشتیبانی کند با کمک ساختمان داده استک،  پرانتز گذاری و اولویت عبارات را محاسبه نمایید. 
دقت داشته باشید که اعداد ورودی میتوانند از نوع اعشاری نیز باشد و برنامه شما باید "." (ممیز) را نیز پشتیبانی کند.
 


## تاریخچه
 ماشین حساب شما باید در هر مرحله از محاسبه وضعیت عبارت را چاپ کند  .

چاپ مراحل محاسبه:
 
 مرحله 1:

4*(2^3)<br>


 مرحله2:
 
 4*8<br>


 مرحله3:
 
 32<br>


 جواب نهایی:<br>
 32<br>
 <br>


## درخت عبارت
 علاوه بر موارد گفته شده شما باید عبارت ریاضی داده شده در ابتدا  را به فرم درخت تبدیل کرده و چاپ کنید.<br>


  مثال :
 ورودی:

```
 (1+3)*(2^3)
```
 
 خروجی درخت:
 
 tree:
 ![tree](https://user-images.githubusercontent.com/70153144/142826292-37bd0066-1964-454f-a66b-fc8a03124bc3.png)

دقت کنید نیازی به نمایش گرافیکی درخت عبارت نیست و تصویر بالا برای درک بهتر درخت نمایش داده شده است.
شما بصورت چاپی از ریشه درخت شروع کرده و به سلیقه خودتان درخت را نمایش دهید. ( اما به عنوان بخش اضافه میتوانید با کتابخانه های گرافیکی آن را نمایش دهید.) 




## مدیریت خطا
 چاپ ارور :اگر عبارت داده شده فرمت صحیح واستانداردی نداشته باشد مثلا پرانتز گذاری اشتباه باشد و یا عملگر ها درست استفاده نشده باشند باید ارور چاپ کرده و سپس آن را مدیریت نمایید.
 .مثال هایی از ورودی های نادرست که باید ارور چاپ کند:<br>
 
 <div dir='ltr' align="justify">
 
 )(1+3)*2<br>
 (((2+5)^2)+4<br>
 3+5^<br>
 +5^<br>
 5/0<br>
 
 <div>


 ### ورودی:
یک عبارت ریاضی شامل اعداد گویا و پرانتز "()" و عملگر های مورد نظر است که  به صورت یک رشته داده می شود . <br>
### خروجی:
یک عدد که حاصل عبارت ریاضی داده شده است ویا پیغام ارور در صورت وجود خطا.
 
  <div dir='ltr' align="justify">


   ورودی1:

 ```
  (1+3) * 2^2
```

 عبارت خروجی 1:

```
  16
```

  ورودی2:

```
  -(-(2^3))/4+1 
```

  عبارت خروجی 2:

```
  3
```

  ورودی3:

``` 
  -(((1+2)*(-3))^(1+1)) 
```

  عبارت خروجی 3:

```
  -81
```

  ورودی4:

```
  )(2+3) 
```

  عبارت خروجی 4:

```
  error
```

  ورودی5:

```
  3+4^
```

  عبارت خروجی 5:

```
  error
```

  ورودی6:

```
  ((1.4+1.6)*10)/100 
``` 
   
  عبارت خروجی 6:

```
  0.3
```
  
  <div>

## بخش امتیازی:
برای پیاده سازی این بخش شما باید  در منوی برنامه خود گزینه ای به نام "add new operator "داشته باشید تا با ستفاده از ان بتوان عمگلر های ئلخواه تعریف کرد و به ماشین حساب اضافه کرد و در محاسبات از انها استفاده کرد.
 نحوه تعریف اپراتور جدید به صورت یز خواهد بود:
 add new operator <br>
a Comp b = 2*a+b<br>
 
 add new operator<br>
a trick b = a^b/b<br>
 
add new operator<br>
a square b = a^2+b^2<br>
 
 همچین گرافیکی کار کردن وافزون ویژگی های دیگر به ماشین حساب که ارزش داشته باشند نمره اضافی خواهد داشت.
 
 <br>
 <hr>

راهنمایی:
میتوانید برای محاسبه عبارت ان را به فرم postfix تبدیل کنید.
 <div>


