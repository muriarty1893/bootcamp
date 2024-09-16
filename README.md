kullandığım veri seti: https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset

Makine Öğrenmesi Projesi: Finansal Dolandırıcılık Tespiti
Bu proje, makine öğrenmesi algoritmalarını kullanarak finansal işlemler üzerinde dolandırıcılığı tespit etmeyi amaçlamaktadır. Proje kapsamında hem gözetimli hem de gözetimsiz öğrenme yöntemleri kullanılmıştır.

Proje İçeriği
1. Veri Seti
Kullanılan veri seti, Kaggle'da bulunan Online Payments Fraud Detection veri setidir. Veri seti, çeşitli finansal işlemleri ve bu işlemlerle ilgili dolandırıcılık olup olmadığını içermektedir.

Veri Boyutu: 10 MB
Veri Noktası Sayısı: 100 bin+
2. Keşifsel Veri Analizi (EDA)
Keşifsel Veri Analizi kapsamında verideki işlem türleri, dolandırıcılık oranı, işlem miktarları ve bakiyeler analiz edilmiştir. İşlem türlerine göre dolandırıcılık dağılımı görselleştirilmiş, ayrıca eski ve yeni bakiye bilgileri dolandırıcılıkla olan ilişkileri açısından incelenmiştir.

3. Veri Ön İşleme
Veri setinde kategorik veriler (işlem türleri) one-hot encoding yöntemi ile sayısal formata dönüştürülmüştür. Ayrıca veriler eksik değerler açısından temizlenmiş ve eğitim/test kümelerine ayrılmıştır.

4. Kullanılan Modeller
Gözetimli Öğrenme
Logistic Regression: İlk model olarak kullanılan Logistic Regression modeli ile dolandırıcılık tespiti yapılmıştır. Ancak sınıf dengesizliği nedeniyle yüksek oranda yanlış negatifler gözlenmiştir.
Ridge Regression: En iyi performansı sağlayan model olarak seçilmiştir. Ridge regresyonu, overfitting'i engellemek için kullanılan bir regularization (L2) tekniğidir.
Gözetimsiz Öğrenme
Bu kısımda gözetimsiz öğrenme algoritmalarından KMeans ve DBSCAN gibi modeller denendi ancak dolandırıcılık tespitinde daha düşük başarı sağladıkları gözlendi.

5. Model Performansı
Seçilen Ridge Regression modelinin performansı aşağıdaki metriklerle ölçülmüştür:

Ortalama Karesel Hata (MSE): 485.23
Ortalama Mutlak Hata (MAE): 12.89
6. Model Değerlendirmesi
Sonuçlar doğrultusunda, Ridge Regression modelinin dolandırıcılık tespitinde iyi bir performans sergilediği görülmüştür. Logistic Regression modeline kıyasla regularization kullanımıyla daha düşük hata oranları elde edilmiştir.

7. Kaggle Notebook Linki
Projenin tamamlanmış haline Kaggle üzerinden erişebilirsiniz:<a href="https://www.kaggle.com/code/murateker/notebookf25a129d6d"> Kaggle Notebook Linki </a>
