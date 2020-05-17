# عبارت شرطی یک خطی (oneline `if` statement)

<div style="direction:rtl!important">

* فرض کنید مقدار `result` باید بر اساس زوج یا فرد بودن `num` ورودی، یکی از مقادیر `"odd"` یا `"even"` ست شود 

</div>

```python
num = int(input("num = "))
if num % 2 == 0:
    result = "even"
else:
    result = "odd"    
```

<div style="direction:rtl!important">

* این عبارت را می‌تونیم این شکلی هم بنویسیمش که خلاصه‌تر بشه.

</div>

```python
num = int(input("num = "))
result = "even" if num % 2 == 0 else "odd"
```

<div style="direction:rtl!important">

* اگه تعداد حالت‌ها بیشتر بود چی؟ مثلا اگه می‌خواستیم باقیمانده تقسیم `num` بر عدد `3` را به صورت یک رشته در متغیر `result` ذخیره کنیم چه کار کنیم؟ 

* اول همون حالت عادی شرطی تو در تو را بنویسیم

</div>

```python
num = int(input("num = "))
if num % 3 == 0:
    result = "sefr"
else:
    if num % 3 == 1:
        result = "yek"
    else:
        result = "do" 
```

<div style="direction:rtl!important">

* خب اون بخش داخلی `else` را می‌تونیم مثل حالت قبلی به یه `if` یک خطی تبدیلش کنیم و نتیجه‌اش هر چی که شد را توی متغیر `ye_chizi` نگه می‌داریم.

* اگه ما توی مسیر کدمون برسیم به اون بلاک `else` پس مقدار `result` مورد نظرمون همون چیزیه که توی متغیر `ye_chizi` ذخیره شده.

</div>


```python
num = int(input("num = "))
if num % 3 == 0:
    result = "sefr"
else:
    ye_chizi = "yek" if num % 3 == 1 else "do"
    result = ye_chizi
```

<div style="direction:rtl!important">

* حالا بیاین یه بار دیگه ساختار شرطی یک خطی را مرور کنیم

</div>



```python
variable = <یک عبارت پایتونی> if <یک شرط پایتونی> else <یک عبارت پایتونی دیگر>
```

<div style="direction:rtl!important">

* خب؟ شما به جای `<یک عبارت پایتونی دیگر > ` می‌تونین هر عبارت پایتونی‌ای قرار بدین حتی اگه خود اون عبارت، یک شرط یک خطی باشه. پس این شکلی می‌تونم شرط‌های تو در تو را هم یک خطی بنویسم. 

</div>


```python
num = int(input("num = "))
ye_chizi = "yek" if num % 3 == 1 else "do"
result = "sefr" if num % 3 == 0 else ye_chizi
```

<div style="direction:rtl!important">

* مرحله آخرش این‌جوری می‌شه. ولی می‌بینید که خوانایی کد پایین‌تر میاد. پس بهتره خیلی زیاد ازش استفاده نکنیم.

</div>


```python
num = int(input("num = "))

result = "sefr" if num % 3 == 0 else "yek" if num % 3 == 1 else "do"
```

