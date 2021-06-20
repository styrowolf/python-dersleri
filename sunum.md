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

# kısa analiz

```python
print()
``` 

fonksiyonu, argüman olarak verilen değişkeni veya değeri komut satırına yazar.

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

### analizler

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

### analizler