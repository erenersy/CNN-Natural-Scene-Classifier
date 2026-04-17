# Intel Natural Scene Classification with CNN 

Bu proje, Intel'in doğal manzara veri setini kullanarak görüntü sınıflandırma yapabilen bir Derin Öğrenme (Deep Learning) modelidir. Proje kapsamında farklı CNN mimarileri denenmiş ve model performansı detaylı hata analizleri ile raporlanmıştır.

## Proje Özeti
* **Hedef:** 6 farklı sınıfı (Binalar, Orman, Buzul, Dağ, Deniz, Sokak) en yüksek doğrulukla ayırt etmek.
* **Başarı Oranı (Validation Accuracy):** ~%85
* **Ekip:** Eren Ersoy, Emre Küçükgöçer, Sude Acıköse, İrem Bilim.

## Teknik Detaylar
* **Kütüphaneler:** TensorFlow, Keras, OpenCV, NumPy, Matplotlib, Seaborn.
* **Mimari:** 3 adet Evrişimli (Convolutional) blok, Max Pooling ve overfitting engellemek için %50 Dropout içeren optimize edilmiş yapı.
* **Veri Ön İşleme:** Görüntü boyutlandırma (150x150), normalizasyon ve veri artırma (Data Augmentation) teknikleri uygulanmıştır.

## Öne Çıkan Analizler
Proje sadece eğitimle sınırlı kalmayıp şu analizleri içermektedir:
- **Varyasyon Deneyleri:** "Küçük Model" ve "Dropoutsuz Model" ile performans karşılaştırmaları.
- **Confusion Matrix:** Sınıf bazlı Precision ve Recall değerlerinin incelenmesi.
- **Hata Analizi:** Modelin özellikle Dağ (Mountain) ve Buzul (Glacier) sınıflarını karıştırma nedenlerinin görsel olarak saptanması.
- **Tahmin Görselleştirme:** Modelin kararlı olduğu ve yanıldığı örneklerin olasılık skorlarıyla raporlanması.

## Nasıl Çalıştırılır?
1. Bu repoyu bilgisayarınıza indirin veya Google Colab'de açın.
2. [Kaggle](https://www.kaggle.com/) üzerinden kendi API key'inizi alın.
3. Kod içerisindeki Aşama 2 bölümüne kullanıcı adı ve anahtarınızı ekleyerek veri setini otomatik indirin.
4. Tüm hücreleri sırayla çalıştırarak eğitimi ve analizi başlatın.

---
*Bu çalışma, Sivas Cumhuriyet Üniversitesi Bilgisayar Mühendisliği Bölümü bünyesinde hazırlanmıştır.*
