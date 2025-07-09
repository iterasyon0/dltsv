## dltsv (Double Less-Than Seperated Values)
---
dltsv; csv, tsv gibi veri saklama dosya formatlarının küçük bir sorununu çözer. csv'de verileri , ler ile birbirlerinden ayırırsınız. dltsvde iki adet << ile bu yapılır.

dltsv bash betiği çalıştırıldığı zaman; 
1. öncelikle vim, bulunamazsa nano çalıştırılır.
2. önümüze gelen editöre verilerimizi gireriz.

örnek girdi:
```
id<<isim<<yaş
1<<aleyna<<12
2<<mahmut<<35
```
3. kaydedip çıkıldığı vakit program column ve markdown olmak üzere iki adet çıktı üretir.

örnek çıktı:
```

=== Column Table ===

id  isim    yaş
1   aleyna  12
2   mahmut  35




=== Markdown Table ===

|id|isim|yaş|
| --- | --- | --- |
|1|aleyna|12|
|2|mahmut|35|
```

örnekteki markdown tablosunu olduğu gibi aşağıya yapıştırıyorum:
|id|isim|yaş|
| --- | --- | --- |
|1|aleyna|12|
|2|mahmut|35|

---

* vim veya nano paketlerinden birisinin sisteminizde kurulu olması lazım. başka bir terminal editörü kullanıyorsanız betikteki ilgili yerleri düzenleyin.
