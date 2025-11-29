# 💊 İlaç ve Yan Etki Analizi: Veri Madenciliği Projesi

Bu proje, **Veri Madenciliğinde İleri Konular** dersi (Yüksek Lisans - 2025-2026 Güz) ara sınavı kapsamında hazırlanmıştır. Proje, çeşitli ilaçların yan etki profillerini, tedavi sürelerini ve hasta demografisini **Veri Madenciliği** ve **İstatistiksel Analiz** yöntemleriyle incelemektedir.

## 📊 Proje Özeti

Bu çalışmada, 1.000 hasta kaydı içeren veri seti üzerinde kapsamlı bir **Keşifsel Veri Analizi (EDA)** ve **Denetimsiz Öğrenme (Hiyerarşik Kümeleme)** uygulanmıştır.

* **Amaç:** İlaçlar ve yan etkiler arasındaki gizli ilişkileri (pattern) ortaya çıkarmak ve klinik çıkarımlarda bulunmak.
* **Kapsam:** Veri setindeki **15 farklı ilaç** ve **30 farklı yan etki** için tam popülasyon analizi yapılmıştır.

## 🔑 Öne Çıkan Bulgular

Analiz sonucunda elde edilen kritik "Veri Madenciliği" ve "Klinik" bulgular şunlardır:

1.  **Tramadol ve Mide Bulantısı:** Veri setindeki en güçlü birliktelik kuralı (association), **Tramadol** kullanımı ile **Mide Bulantısı (Nausea)** arasında tespit edilmiştir (Global Maksimum Frekans).
2.  **Aykırı Gözlem (Outlier) - İnsülin:** Hiyerarşik kümeleme analizi, **Insulin Glargine** ilacını diğer tüm ilaçlardan ayırmıştır. Bunun nedeni, sadece bu ilaca özgü olan "Enjeksiyon yeri ağrısı" ve "Kilo alımı" yan etkileridir.
3.  **Veri Kalitesi Tespiti:** Analiz sırasında **"Low sugar"** ve **"Low blood sugar"** değişkenlerinin veri setinde ayrı ayrı etiketlendiği, ancak semantik olarak aynı olduğu tespit edilmiştir. Bu bulgu, veri temizliği (data cleaning) ihtiyacını ortaya koymuştur.
4.  **Yaş ve İyileşme İlişkisi:** Yaş ile İyileşme Skoru arasında yapılan korelasyon analizinde $r \approx 0.01$ bulunmuştur. Bu, tedavi başarısının hastanın yaşından bağımsız olduğunu kanıtlamaktadır.

## 🛠 Kullanılan Teknolojiler ve Kütüphaneler

Proje **Python** dili kullanılarak **Jupyter Notebook** ortamında geliştirilmiştir.

* **Pandas:** Veri manipülasyonu ve çapraz tablolar (Crosstab).
* **Seaborn & Matplotlib:** Veri görselleştirme (Heatmap, Boxplot, Pie Chart).
* **Scipy:** Hiyerarşik kümeleme (Hierarchical Clustering) algoritmaları.
* **Numpy:** Sayısal hesaplamalar.

## 📂 Dosya Yapısı

* `254329023_onder_sevki_sut.ipynb`: Projenin kaynak kodlarını, analizleri ve yorumları içeren ana Jupyter Notebook dosyası.
* `254329023_onder_sevki_sut.html`: Notebook dosyasının rapor formatındaki HTML çıktısı.
* `real_drug_dataset.csv`: Analizde kullanılan ham veri seti.

## 🚀 Kurulum ve Çalıştırma

Projeyi kendi bilgisayarınızda çalıştırmak için:

1.  Repoyu klonlayın:
    ```bash
    git clone [https://github.com/ondersevkisut-uskudar/VeriMadenciligi_Proje.git](https://github.com/ondersevkisut-uskudar/VeriMadenciligi_Proje.git)
    ```
2.  Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install pandas numpy matplotlib seaborn scipy
    ```
3.  Jupyter Notebook'u başlatın ve `.ipynb` dosyasını çalıştırın.

## 📝 Yazar

**Önder Şevki Süt**
* **Öğrenci No:** 254329023
* **Ders:** Veri Madenciliğinde İleri Konular

---
*Bu proje akademik amaçla hazırlanmıştır.*
