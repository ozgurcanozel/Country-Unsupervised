Bu proje, ülkelerin çeşitli verilerini analiz ederek hangi ülkelerin finansal desteğe/bütçeye ihtiyacı olduğunu (Budget Needed, In Between, No Budget Needed) belirlemeyi amaçlayan bir makine öğrenmesi ve veri analitiği çalışmasıdır

### Proje Adımları

1. **Veri Yükleme ve İnceleme:** `29-country_data.csv` içeri aktarıldı. Veri setinin genel yapısı, istatistiksel özellikleri ve eksik değerleri incelendi
2. **Veri Ön İşleme ve Keşifsel Veri Analizi (EDA):** Veriler arasındaki ilişkiler `seaborn` ve `matplotlib` kullanılarak görselleştirildi ve modele hazır hale getirildi
3. **Temel Bileşenler Analizi (PCA):** Çok boyutlu veri setinin varyansını büyük ölçüde koruyarak boyut sayısını düşürmek ve model performansını artırmak için PCA uygulandı
4. **Modelleme ve Sınıflandırma:** Ülkeler bütçe ihtiyaçlarına göre 3 farklı kategoriye ayrıldı:
   - 🔴 **Budget Needed** (Bütçe İhtiyacı Olanlar)
   - 🟡 **In Between** (Arada Kalanlar)
   - 🟢 **No Budget Needed** (Bütçe İhtiyacı Olmayanlar)
5. **Görselleştirme:** Model çıktıları, `plotly.express` kütüphanesi ile bir dünya haritası üzerinde görselleştirildi.

### Model Performansı

- **[Silhouette Score]:** `[0.4386320345236684]`

### Harita Görselleştirmesi

### Ülkelere Göre Bütçe İhtiyacı (Needed Budget By Country)
PCA ve sınıflandırma adımları sonucunda elde edilen verilerin coğrafi dağılımı aşağıdadır.

![Dünya Haritası Çıktısı](https://github.com/user-attachments/assets/765da092-772b-4414-8a13-19928534edef)
### Korelasyon ve Dağılım Grafikleri
Değişkenler arası ilişkileri gösteren diğer analiz çıktıları:

<img src="https://github.com/user-attachments/assets/c7a5e9aa-bf6e-43e8-9700-169ccd2ab5e9" alt="Korelasyon Tablosu" width="50%" height="auto">

### Kurulum ve Çalıştırma

Projeyi kendi bilgisayarınızda çalıştırmak için:

1. Repoyu klonlayın:
   ```bash
   git clone [https://github.com/ozgurcanozel/](https://github.com/ozgurcanozel/)[REPO_ADINI_BURAYA_YAZ].git
2. Gerekli kutuphaneleri kopyalayin
   ```bash
   pip install numpy pandas seaborn matplotlib plotly scikit-learn
3. Jupyter Notebook'u başlatın ve CountryDataSet.ipynb dosyasını çalıştırın.
