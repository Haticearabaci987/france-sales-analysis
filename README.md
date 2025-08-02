# france-sales-analysis
Filtered France from a multi-country retail dataset and performed a detailed Excel-based sales analysis.
Online Retail - Fransa Satışları Analizi
Bu çalışma, Online Retail veri setinden Fransa ülkesine ait satışları filtreleyip, çeşitli Excel fonksiyonları ile satış performansını ve istatistiklerini analiz etmektedir. Kullanılan temel fonksiyonlar: COUNT, COUNTA, COUNTIFS, TRIM, CONCATENATE, LEFT, RIGHT, WEEKDAY, EXACT, SUMIF, SUMIFS ve RANK'tir.

1. Veri Hazırlığı ve Filtreleme
Fransa Satışları Filtreleme:

Ülke sütunundan France olan kayıtlar filtrelenmiştir.

Invoice Listesi:

Filtrelenen Fransa satışlarındaki benzersiz Invoice numaraları listeye alınmıştır.

2. Temel İstatistikler
a) Toplam Satış (Ciro)
SUMIF fonksiyonu kullanılarak Fransa’ya ait satışların toplam geliri (Ciro) hesaplanmıştır.

b) Fransa’dan Kaç Farklı Müşteri Alışveriş Yaptı?
COUNTA ve UNIQUE fonksiyonları veya COUNTIFS ile benzersiz müşteri sayısı bulunmuştur.

c) Bir Kişi Ortalama Ne Kadar Alışveriş Yaptı?
Ciro Bazında Ortalama: Toplam ciro, müşteri sayısına bölünmüştür.

Adet Bazında Ortalama: Toplam ürün adedi, müşteri sayısına bölünmüştür.

d) Bir Kişi Ortalama Kaç Günde Bir Alışveriş Yapıyor?
Müşterilerin ilk ve son alışveriş tarihleri arasındaki gün farkı hesaplanmış, toplam alışveriş sayısına bölünerek ortalama alışveriş sıklığı bulunmuştur.

Tarihlerde WEEKDAY ve DATEDIF fonksiyonları kullanılmıştır.

e) Bir Seferde En Yüksek Siparişli Ürün (Ciro Bazında)
Her invoice için ürünlerin toplam ciroyu gösteren sütun hesaplandıktan sonra, en yüksek tutar belirlenmiştir.

3. Günlük En Yüksek Ciro Getiren Kayıtlar (Rank Fonksiyonu)
Her gün için RANK fonksiyonu kullanılarak ciro değerleri sıralanmıştır.

Gün bazında en yüksek ciroya sahip kayıtlar seçilmiştir.

4. Fiyat, Gelir ve Adet Verilerinin Değişim Katsayıları (Coefficient of Variation - CV)
CV = (Standart Sapma / Ortalama) formülü ile Fiyat, Gelir ve Adet sütunlarının değişim katsayıları hesaplanmıştır.

Bu değerler, verinin ne kadar değişken olduğunu gösterir.

5. Dışa Düşen (Aykırı) Değerlerin İncelenmesi
Fiyat, Gelir ve Adet verilerinde çok yüksek veya çok düşük değerler (aykırı değerler) gözlemlenmiştir.

Örneğin:

Çok yüksek adetli siparişler ya da çok düşük fiyatlı ürünler olabilir.

Bu değerler analiz sonuçlarını etkileyebilir ve dikkatle incelenmelidir.

Bu dışa düşen değerlerin varlığı satış hacmindeki çeşitlilik ve kayıt hatalarından kaynaklanabilir.

Kullanılan Excel Fonksiyonlarına Örnekler
Fonksiyon	Kullanım Amacı
COUNT	Sayısal verilerin sayılması
COUNTA	Boş olmayan hücrelerin sayılması
COUNTIFS	Çoklu koşullara göre sayım
TRIM	Hücredeki gereksiz boşlukların temizlenmesi
CONCATENATE	Hücrelerin birleştirilmesi
LEFT / RIGHT	Metnin sol veya sağından karakter alma
WEEKDAY	Tarihin haftanın hangi günü olduğunu bulma
EXACT	Metinlerin birebir eşitliğini kontrol etme
SUMIF / SUMIFS	Koşullu toplam hesaplama
RANK	Değerlerin sıralanması

Sonuç
Fransa satışlarından elde edilen temel istatistikler, müşteri davranışları ve satış performansı hakkında detaylı bilgi sağlamaktadır.

RANK fonksiyonu ile günlük en yüksek ciro getiren işlemler belirlenmiştir.

Fiyat, gelir ve adet verilerindeki yüksek değişim katsayıları ve dışa düşen değerler, veri kalitesi ve satış trendlerinin çeşitliliği hakkında uyarıcıdır.

Bu analiz, daha iyi pazarlama stratejileri geliştirmek ve stok yönetimini optimize etmek için kullanılabilir.

