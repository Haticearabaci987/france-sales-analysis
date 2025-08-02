France Sales Analysis
Bu proje, Online Retail veri setinden Fransa satışlarını filtreleyip, Excel fonksiyonları kullanarak detaylı satış analizi yapmaktadır. Kullanılan başlıca fonksiyonlar:

COUNT, COUNTA, COUNTIFS, TRIM, CONCATENATE, LEFT, RIGHT, WEEKDAY, EXACT, SUMIF, SUMIFS, RANK.

1. Veri Hazırlığı ve Filtreleme
Ülke sütunundan France kayıtları filtrelendi.

Fransa satışlarına ait benzersiz Invoice numaraları listelendi.

2. Temel İstatistikler
Toplam Satış (Ciro): SUMIF ile Fransa satışlarının toplam geliri hesaplandı.

Farklı Müşteri Sayısı: COUNTA ve UNIQUE ile benzersiz müşteri sayısı bulundu.

Müşteri Başına Ortalama Alışveriş:

Ciro bazında toplam ciro / müşteri sayısı

Adet bazında toplam ürün adedi / müşteri sayısı

Ortalama Alışveriş Sıklığı:
Müşterilerin ilk ve son alışveriş tarihleri arasındaki gün farkı, toplam alışveriş sayısına bölünerek hesaplandı (WEEKDAY, DATEDIF kullanıldı).

En Yüksek Ciro Getiren Tek Sipariş: Her invoice için toplam ciro hesaplandı ve en yüksek sipariş belirlendi.

3. Günlük En Yüksek Ciro Getiren Kayıtlar
RANK fonksiyonu kullanılarak her günün en yüksek ciro getiren satışları tespit edildi.

4. Fiyat, Gelir ve Adet Verilerinin Değişim Katsayıları (CV)
CV = Standart Sapma / Ortalama formülü ile Fiyat, Gelir ve Adet sütunlarının değişkenlik katsayıları hesaplandı.

Yüksek CV, verideki dalgalanmanın büyüklüğünü gösterir.

5. Aykırı (Dışa Düşen) Değerlerin İncelenmesi
Fiyat, Gelir ve Adet sütunlarında aşırı yüksek veya düşük (aykırı) değerler gözlemlendi.

Bu değerler analiz sonuçlarını etkileyebilir ve veri kalitesi ile satış trendlerinde çeşitlilik olduğunu gösterir.

Dikkatle incelenmesi önerilir.

Kullanılan Excel Fonksiyonları
Fonksiyon	Kullanım Amacı
COUNT	Sayısal verilerin sayılması
COUNTA	Boş olmayan hücrelerin sayılması
COUNTIFS	Çoklu koşullara göre sayım
TRIM	Gereksiz boşlukların temizlenmesi
CONCATENATE	Hücre içeriklerinin birleştirilmesi
LEFT / RIGHT	Metinden karakter alma (sol/sağ)
WEEKDAY	Tarihin haftanın hangi günü olduğunu bulma
EXACT	Metinlerin birebir eşitliğini kontrol etme
SUMIF / SUMIFS	Koşullu toplam hesaplama
RANK	Değerlerin sıralanması

Sonuç
Bu analiz ile Fransa satışlarının genel performansı, müşteri davranışları ve satış trendleri hakkında kapsamlı bilgi elde edilmiştir. Elde edilen bulgular, pazarlama stratejileri ve stok yönetimi kararlarının iyileştirilmesi için temel oluşturur.



