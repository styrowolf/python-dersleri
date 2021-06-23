---
marp: true
theme: uncover
# default - gaia - uncover
--- 

# **programlamaya giriş**

## python dili

---

# merhaba dünya!

hadi gelin, ilk kodumuzu yazalım!

```python
print("merhaba dünya")
```

---

# merhaba ____!

adımızla bizi karşılasa bu program çok güzel olur. hemen deneyelim:

```python
ad = input("adınız nedir: ")
print("merhaba", ad)
```

---

### analiz

```python
print()
```

fonksiyonu, argüman olarak verilen değişkeni veya değeri komut satırına yazar.

```python
input()
```

fonksiyonu, argüman olarak verilen yazıyı soru olarak kullanarak komut satırından girdi alır. bu girdi **str** türündedir.

---

# değişkenler

değişkenler, çeşitli değerleri altında sakladığımız adlardır. bu değere erişmek için ve bu değeri değiştirmek için kodumuzda bu adı kullanırız.

---

### örnek:
```python
ad = "mehmet"
soyad = "kurt"
yas = 14
not_ortalamasi = 83.5
programlama_biliyor = False
```

```python
print(ad, soyad)
print("yaş: " + str(yas))
print("not ortalaması: " + str(not_ortalamasi))
```

```
mehmet kurt
yaş: 14
not ortalaması: 83.5
```

---

### analiz

python'da değerlerin farklı türleri vardır.

```python
ad: str = "mehmet" # string (harf dizisi / yazı)
soyad: str = "kurt"
yas: int = 14 # integer (tam sayı)
not_ortalamasi: float = 83.5 # floating-point number (ondalık sayı)
programlama_biliyor: bool = False # boolean (doğru/yanlış)
```

türlere göre değerler farklı fonksiyonlarda kullanabilir, farklı şekilde değiştirilebilir.

---

# matematiksel hesaplar

dört işlem:

```python
7 + 5 # toplama operatörü: +
12 - 9 # çıkarma operatörü: -
3 * 7 # çarpma operatörü: *
8 / 3 # bölme operatörü: /
```

---

### diğer kullanışlı işlemler:

![bg right:40% 100%](fotograflar/bolme.png)
```python
7 // 2 # (tam sayı) bölme operatörü: //
7 % 2 # kalan hesaplama operatörü: %
```

bir de son olarak:

```python
8 ** 3 # kuvvetini alma operatörü: **
```

---

# kısa proje

aşağıda bir öğrencinin aldığı notlar bulunmaktadır. bu öğrencinin ağırlıklı ortalamasını bulan bir program yazın.

dersler | katsayı | alınan not |
:--- | :---: | ---: |
matematik | 7 | 87 |
fen bilimleri | 5 | 92 |
türkçe | 10 | 75 |

**challenge**: alınan notları komut satırından girdi olarak alın.

---

### kısaca ağırlıklı ortalama

## $\frac{k_1 n_1 + k_2 n_2 + ... + k_i n_i}{k_1 + k_2 + ... + k_i}$

burada $k$'ler derslerin katsayısını, $n$'ler de derslerde alınan notları temsil ediyor.

---

# sayıları karşılaştırma

matematiksel ifadeler olarak: 

$10 < 16$
$12 > 8$
$6 \geq 2$
$7 \leq 8$
$8 = \frac{40}{5}$
$16 \ne 18$

---

# sayıları karşılaştırma

sayıları karşılaştırma ifadeleri sonuç olarak *boolean* türünü verir.

```python
7 < 5 # 7 küçüktür 5 -> False (yanlış)
12 > 8 # 12 büyüktür 8 -> True (doğru)
6 >= 2 # 6 büyüktür veya eşittir 2 -> True (doğru)
7 <= 8 # 7 küçüktür veya eşittir 8 -> True (doğru)
8 == 40/5 # 8 eşittir 40/5 -> True (doğru)
16 != 18 # 16 eşit değildir 18 -> True (doğru)
```

---

# kontrol akışı

##### **if (eğer) - elif (değilse eğer) - else (değilse)**

kimi zaman programımızda çeşitli şartları kontrol etmek ve ona göre farklı kodlar çalıştırmak isteyebiliriz. 
kontrol akışı yapıları bize bunu sağlar.

---

# if - elif - else

if - elif - else yapısı biraz önce gösterdiğimiz *boolean* türünü veren bir ifadeyi ve değişkeni alarak çalıştıracağımız kodu kontrol etmemizi sağlar.

```python
sart: bool = 6 <= 4 

if sart: # şart yerine direkt 
# yukarıdaki ifadeyi de yazabilirsiniz
    print("verdiğin ifade doğru!")
else:
    print("verdiğin ifade yanlış!")
```

---

# if - elif - else

örnek: 

```python
hava_durumu = input("güneşli -> 1, yağmurlu -> 2, bulutlu -> 3: ")

if int(hava_durumu) == 1:
    print("şemsiye almana gerek yok")
elif int(hava_durumu) == 2:
    print("şemsiye kesinlikle almalısın")
elif int(hava_durumu) == 3:
    print("bilemedim şemsiye alsam mı almasam mı")
else:
    print("hangi hava durumu bu ya, anlayamadım")
```

---