# Weather_prediction_ltsm_model

Harika bir fikir! Bir README.md dosyası, projenizi hem sizin hem de başkaları için anlaşılır ve erişilebilir kılar.

İşte projeniz için hazır, kapsamlı bir README.md dosyası. Bu metni doğrudan kopyalayıp GitHub deponuza yapıştırabilirsiniz.

Markdown

# ☀️ İspanya Şehirleri İçin LSTM Tabanlı Hava Durumu Tahmini

Bu proje, İspanya'daki beş büyük şehir (Valencia, Madrid, Bilbao, Barcelona, Seville) için sıcaklık tahmini yapmak amacıyla **LSTM (Uzun-Kısa Süreli Hafıza)** sinir ağlarını kullanmaktadır. Model, geçmiş 24 saatlik veriyi analiz ederek bir sonraki saatteki sıcaklık tahminini yapacak şekilde eğitilmiştir.

## Projenin Amacı ve Özellikleri

* **Zaman Serisi Analizi:** Geçmişe ait hava durumu verilerini kullanarak gelecekteki sıcaklıkları tahmin etme.
* **Derin Öğrenme Modeli:** Her bir şehir için ayrı bir LSTM modeli eğitme ve bu modellerin performansını değerlendirme.
* **Çoklu Önemli Özellikler:** Tahmin modelinde sıcaklık dışında basınç, nem, rüzgar hızı ve bulutluluk gibi diğer özellikleri de kullanma.
* **Model Performans Değerlendirmesi:** Modellerin doğruluğunu, **RMSE (Ortalama Karesel Hatanın Karekökü)** metriği ile ölçme.

## Model Performansı

Eğitilen modeller, test verileri üzerinde gösterdikleri düşük RMSE değerleri ile yüksek başarıya ulaştılar. Bu değerler, tahminlerin gerçek sıcaklıktan ortalama sapmasını gösterir.

| Şehir | Test RMSE (°C) |
| :--- | :--- |
| **Bilbao** | **0.88** |
| Madrid | 0.95 |
| Valencia | 0.98 |
| Barcelona | 0.99 |
| Seville | 1.07 |

En iyi performansı gösteren Bilbao modeli, ortalama sadece **0.88 °C**'lik bir hata payıyla tahmin yaptı.

## Kullanılan Teknolojiler

* **Python:** Projenin temel programlama dili.
* **Pandas:** Veri işleme ve analizi için kullanıldı.
* **NumPy:** Sayısal işlemler ve dizi manipülasyonları için kullanıldı.
* **TensorFlow / Keras:** Derin öğrenme modellerini oluşturmak ve eğitmek için kullanıldı.
* **Scikit-learn:** Veri normalleştirme (MinMaxScaler) için kullanıldı.

## Dosya Yapısı

Projenin temel dosya yapısı aşağıdaki gibidir:

/
├── weather_features.csv            # Orijinal veri seti
├── hava_durumu_tahmin_projesi.ipynb # Kaggle not defteri (ana kod)
├── trained_models/                # Eğitilen modellerin kaydedildiği klasör
│   ├── lstm_model_valencia.h5
│   └── ... (diğer şehirlerin modelleri)
├── README.md                      # Bu dosya


## Projeyi Çalıştırma

1.  Bu depoyu yerel makinenize klonlayın: `git clone <depo_adresiniz>`
2.  Gerekli kütüphaneleri yükleyin: `pip install pandas numpy tensorflow scikit-learn`
3.  `hava_durumu_tahmin_projesi.ipynb` dosyasını Jupyter veya benzeri bir ortamda açarak adımları sırasıyla çalıştırın.

---
