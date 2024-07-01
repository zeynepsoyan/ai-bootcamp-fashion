# Fashion MNIST Classification Project

Check out the full explanation of the project in English in (this Medium article)[https://medium.com/@zeynepsoyan/ml-classification-with-fashion-mnist-a-comparison-of-algorithms-58008e1b29a5]

## Veri Seti Hakkında
Bu proje, Keras kütüphanesinde sağlanan Fashion MNIST veri seti üzerine kurulmuştur. Fashion MNIST, kıyafet görüntülerinden oluşan bir veri setidir ve 10 farklı sınıfa sahiptir:

- T-shirt/top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle boot

Veri seti, her biri 28x28 piksel boyutunda olan 60,000 eğitim görüntüsü ve 10,000 test görüntüsünden oluşur. Her piksel değeri 0 ile 255 arasında değişir ve gri tonlamalıdır.

## Projenin Amacı
Bu projenin amacı, Fashion MNIST veri seti üzerinde çeşitli makine öğrenmesi ve derin öğrenme algoritmalarını kullanarak sınıflandırma yapmaktır. Farklı algoritmaların performanslarını karşılaştırarak, hangi algoritmanın bu veri seti üzerinde en iyi sonucu verdiğini belirlemektir.

## Algoritmalar ve Deneyler
### Makine Öğrenmesi Algoritmaları
- **K-Nearest Neighbors (KNN)**
- **Random Forest**
- **Decision Tree**
- **Support Vector Classifier (SVC)**

Yapılan deneylerde, SVC algoritması diğer makine öğrenmesi algoritmalarına kıyasla en iyi performansı göstermiştir.

### Yapay Sinir Ağı (ANN) Deneyleri
1. **Deney**: 
   - 2 katman, sırasıyla 4 ve 8 nöron, dropout yok, epoch sayısı 10
   - Temel performans, ancak sınırlı başarı

2. **Deney**: 
   - 2 katman, sırasıyla 64 ve 32 nöron, dropout yok, epoch sayısı 20
   - Daha iyi sonuç, ancak overfitting problemi

3. **Deney**: 
   - 2 katman, sırasıyla 64 ve 32 nöron, %30 dropout, epoch sayısı 20
   - Overfitting problemi azaldı

4. **Deney**: 
   - 3 katman, sırasıyla 128, 64 ve 32 nöron, %30 dropout, epoch sayısı 30
   - En iyi sonuç elde edildi

### Genel Bulgular
- **SVC Algoritması**: Makine öğrenmesi algoritmaları arasında en iyi performansı gösterdi.
- **ANN Modelleri**: Doğru hiperparametre ayarları ve dropout kullanımı ile güçlü sonuçlar elde edildi.
- **Overfitting**: Daha karmaşık modellerde ortaya çıktı, ancak dropout tekniği ile kontrol altına alındı.

![image](https://github.com/zeynepsoyan/ai-bootcamp-fashion/assets/54821016/cb7119a8-6c8e-4da7-971d-aa516428fd7b)
