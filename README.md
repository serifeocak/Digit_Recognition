# YÜKSEK DÜZEY PROGRAMLAMA PROJE ÖDEVİ
Şerife Sümeyye OCAK - 202013171046

Rapor Linki:https://github.com/serifeocak/digit_recognizer/blob/main/rapor.pdf

Kod Linki:https://github.com/serifeocak/Digit_Recognition/blob/main/digit_recognizer/digit-recognition-with-simple-cnn.ipynb

Kullanılan Araçlar ve Teknolojiler
- **Python**: Veri analizi ve model geliştirme.  
- **Pandas & NumPy**: Veri manipülasyonu ve hesaplama.  
- **Matplotlib & Seaborn**: Veri görselleştirme.  
- **Keras**: Derin öğrenme modeli oluşturma.  
- **TensorFlow**: Model eğitimi ve optimizasyon.  
- **Jupyter Notebook**: Kodlama ve analiz ortamı.  


Bu çalışmada, el yazısı ile yazılmış rakamları otomatik olarak tanımlayabilen bir görüntü sınıflandırma modeli tasarlanmıştır. Model, görsel verilerden özellik çıkarmada başarılı olan bir derin öğrenme yöntemi olan Convolutional Neural Network (CNN) mimarisi üzerine inşa edilmiştir.

Modelin geliştirilmesi için 28x28 piksellik gri tonlamalı rakam görüntülerinden oluşan bir veri seti kullanılmıştır. Veri seti, piksellerin ölçeklendirilmesi ve uygun boyutlandırma işlemleriyle model eğitimi için optimize edilmiştir. Eğitim sürecinde, Adam optimizasyon algoritması ve Sparse Categorical Crossentropy kayıp fonksiyonu kullanılarak modelin performansı artırılmıştır. Eğitim ve test veri setlerinde elde edilen sonuçlar, modelin yüksek doğruluk oranına sahip olduğunu göstermiştir.

### **Giriş**
Bu proje kapsamında, el yazısı ile yazılmış rakamların doğru bir şekilde sınıflandırılmasını hedefleyen bir CNN modeli geliştirilmiştir. CNN mimarisi, görsellerdeki piksellerin ilişkilerini öğrenerek, etkili bir sınıflandırma gerçekleştirme yeteneğine sahiptir.

### **Materyal ve Metot**
#### **Veri Seti**
Çalışmada, Kaggle platformundan temin edilen *Digit Recognizer* veri seti kullanılmıştır. Veri seti şu bileşenlerden oluşmaktadır:
- **train.csv**: Etiketlenmiş 42.000 el yazısı rakam görüntüsü (0-9).
- **test.csv**: Etiketsiz 28.000 rakam görüntüsü. Modelin performansını değerlendirmek için kullanılmıştır.

Veri setindeki her görüntü 28x28 piksel boyutunda gri tonlamalıdır. Eğitim sürecinde tüm *train.csv* verisi kullanılmış, veri bölümlemesi yapılmamıştır.

#### **Model Eğitimi**
Bu çalışmada CNN tabanlı bir model eğitilmiştir. Eğitim sürecinde:
- **Adam** optimizasyon algoritması kullanılarak modelin parametre güncellemeleri hızlandırılmıştır.
- **Sparse Categorical Crossentropy** kayıp fonksiyonu ile model performansı değerlendirilmiştir.
- 50 Epoch boyunca eğitim yapılmış ve modelin doğruluk oranı her aşamada artmıştır.


#### **Sonuçlar ve Çıktılar**
Modelin eğitilmesi tamamlandıktan sonra, aşağıdaki çıktılar elde edilmiştir:

#### **1.Eğitim doğruluğu (Accuracy):** Model, eğitim verileri üzerinde yaklaşık %99 doğruluk sağlamıştır.

#### **2.Test doğruluğu (Accuracy):** Test verileri üzerinde model, %98 doğruluk oranı ile başarılı olmuştur.

#### **3.Confusion Matrix:** Test sonuçlarını detaylandırarak, hangi rakamların doğru veya yanlış sınıflandırıldığını görmek için kullanılmıştır.  

Sonuç olarak, bu yöntemlerle geliştirilmiş model hem eğitim hem de test veri setlerinde başarılı bir performans göstermiştir.



![image](https://github.com/user-attachments/assets/b1b72b12-a720-4f77-a951-ca72041ab571)


![image](https://github.com/user-attachments/assets/4aef6766-1f31-47b0-898c-7af993e951eb)

