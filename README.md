# ML_Bootcamp

# Kalp Krizi Tahmini Üzerine Analiz

Bu proje, Birleşik Devletler'deki kalp krizi verilerini kullanarak, StressLevel ve Gender değişkenlerinin kalp krizi (Outcome) üzerindeki etkisini incelemek ve makine öğrenmesi modelleriyle tahmin yapmaktır.

## Giriş

Bu çalışma, sağlık verileri üzerinden stres seviyesi ve cinsiyetin kalp krizi riskini nasıl etkilediğini anlamayı hedeflemektedir. Eldeki veri seti kullanılarak, bu iki değişkenin kalp krizi olasılığı üzerindeki ilişkisi görselleştirilmiş ve Logistic Regression ile Support Vector Machine (SVM) gibi makine öğrenmesi modelleri ile tahminleme yapılmıştır.

## Veri Seti

Bu projede kullanılan veri seti Kaggle'dan indirilmiştir: [ankushpanday2/heart-attack-prediction-in-united-states](https://www.kaggle.com/datasets/ankushpanday2/heart-attack-prediction-in-united-states)
Veri seti, bireylerin stres seviyeleri, cinsiyetleri ve kalp krizi sonuçlarını içermektedir. Çalışmada özellikle 'Outcome', 'Gender' ve 'StressLevel' sütunları kullanılmıştır.


## Analiz ve Görselleştirmeler

Veri setinin genel yapısı incelendikten sonra, StressLevel, Gender ve Outcome arasındaki ilişkileri anlamak için çeşitli görselleştirmeler yapılmıştır.

- **StressLevel Dağılımı:** Genel stres seviyesi dağılımını göstermektedir.
- **Outcome'a Göre StressLevel Dağılımı:** Kalp krizi sonucu ('Outcome') gruplarına göre stres seviyesinin dağılımını karşılaştırmaktadır.
- **Gender'a Göre Outcome Sayımı:** Cinsiyete göre kalp krizi geçiren ve geçirmeyen bireylerin sayısını göstermektedir.
- **StressLevel'a Göre Gender ve Outcome Sayımı:** Stress seviyesine göre cinsiyet ve kalp krizi sonuçlarının kırılımını sunmaktadır.

Bu görselleştirmeler için `matplotlib` ve `seaborn` kütüphaneleri kullanılmıştır.

## Makine Öğrenmesi Modelleri

**Logistic Regression:**
    -   'Outcome' sütunu Label Encoding ile sayısal hale getirilmiştir.
    -   'Gender' sütunu One-Hot Encoding ile işlenmiştir.
    -   StressLevel ve kodlanmış Gender sütunları kullanılarak model eğitilmiştir.
    -   Modelin doğruluk oranı ve sınıflandırma raporu (precision, recall, f1-score) hesaplanmıştır.


Model için `sklearn` kütüphanesi kullanılmıştır. Model performansı, veri setinin %20'lik kısmını oluşturan test seti üzerinde değerlendirilmiştir.

## Sonuçlar ve Değerlendirme

Yapılan analizler ve model uygulamaları sonucunda:

-   Görselleştirmeler, StressLevel ve Gender değişkenlerinin Outcome üzerindeki etkilerine dair ön bilgiler sunmaktadır.
-   Logistic Regression modeli belirli bir doğruluk oranıyla kalp krizi tahmini yapabilmektedir.

Bu çalışma, yalnızca iki değişken üzerinden bir analiz sunmaktadır. Daha kapsamlı bir tahmin modeli için ek değişkenlerin (yaş, tansiyon, kolesterol vb.) ve daha gelişmiş modelleme tekniklerinin kullanılması gerekmektedir.


