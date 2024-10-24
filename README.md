# classification_fish
Fish Classification with ANN
Akbank Derin Öğrenme Bootcamp Projesi: Balık Türü Sınıflandırma
Bu proje, Akbank tarafından düzenlenen Derin Öğrenme Bootcamp'ı kapsamında gerçekleştirilmiştir. Projenin amacı, Kaggle üzerinde sağlanan büyük ölçekli balık veri seti kullanılarak bir derin öğrenme modelinin geliştirilmesi ve balık türlerinin doğru şekilde sınıflandırılmasıdır.

# Proje Konusu
Projenin ana amacı, sağlanan balık veri seti üzerinde bir yapay sinir ağı (ANN) mimarisi kullanarak sınıflandırma modeli geliştirmektir. Veri seti, çeşitli balık türlerini içeren resimlerden oluşmaktadır ve modelin bu resimlerden yola çıkarak hangi türe ait olduğunu belirlemesi beklenmektedir.

Veri Seti: A Large Scale Fish Dataset

Projede Kullanılan Teknolojiler
Python
TensorFlow ve Keras
Pandas ve NumPy
Matplotlib ve Seaborn (Veri görselleştirme)
Scikit-learn (Veri işleme ve değerlendirme)
Adımlar
# 1. Veri Önişleme
Veri seti, .png formatında resimlerden oluştuğu için, geleneksel veri yükleme yöntemleri yerine resimler işlenerek bir Pandas DataFrame oluşturulmuştur. Aşağıdaki adımlar bu sürecin temelini oluşturmaktadır:

Resimlerin uygun formatta yüklenmesi ve etiketlenmesi.
Eğitim ve test veri seti olarak ayrılması.
Görselleştirme ile veri setinin analizi.
# 2. Modelin Oluşturulması
Yapay Sinir Ağı (ANN) modeli kullanılmıştır. Model, aşağıdaki yapılandırma ile geliştirilmiştir:

Katmanlar: 5 gizli katman ve 1 çıkış katmanı.
Aktivasyon Fonksiyonları: ReLU ve Softmax.
Düzenleyiciler: Dropout katmanları ve L2 regularization aşırı öğrenmeyi (overfitting) önlemek için kullanılmıştır.
AdamW optimizörü ile model optimize edilmiştir.
# 3. Modelin Eğitilmesi
Model, eğitim verileri kullanılarak eğitilmiştir. Eğitim sırasında dropout, batch normalization ve hiperparametre ayarlamaları ile modelin performansı optimize edilmiştir.

# 4. Modelin Değerlendirilmesi
Model başarı ile eğitildikten sonra performansı çeşitli metriklerle ölçülmüştür:

Accuracy: Modelin doğruluk oranı.
Loss Fonksiyonu: Eğitim sırasında kayıp fonksiyonunun grafiği çıkarılmıştır.
Confusion Matrix: Hangi türlerin doğru ve yanlış sınıflandırıldığını görselleştirmek için kullanılmıştır.
# 5. Hiperparametre Optimizasyonu
Katman sayısı, düğüm sayısı, dropout oranı ve optimizasyon parametreleri ile oynanarak model performansı iyileştirilmiştir.
Sonuçlar
Model, balık türlerini başarılı bir şekilde sınıflandırmakta ve değerlendirme adımlarında iyi sonuçlar elde etmiştir. Hiperparametre optimizasyonu sonucunda modelin doğruluğu artırılmış ve aşırı öğrenme önlenmiştir.

# Kaggle Notebook Linki
Projenin Kaggle üzerindeki notebook'una buradan ulaşabilirsiniz: [Kaggle Notebook](https://www.kaggle.com/code/mustafayapar/ann-fishdataset)
