# Hayvan Görselleri Sınıflandırma Projesi

Bu proje, **PyTorch** kullanılarak oluşturulmuş bir **Convolutional Neural Network (CNN)** modelini hayvan görsellerini sınıflandırmak için eğitmekte ve test etmektedir. Çeşitli veri artırma (augmentation) teknikleri ve renk sabitliği yöntemleri uygulanarak model performansı ölçülmüştür.

## Özellikler

- **Veri Seçimi ve Hazırlığı:**
  - 10 farklı hayvan sınıfından görseller seçilerek bir çalışma dizini oluşturulmuştur.
  - Görseller 64x64 çözünürlüğe yeniden boyutlandırılmıştır.
- **Veri Artırma (Augmentation):**
  - Görsellere rastgele yatay çevirme, döndürme, bulanıklaştırma ve parlaklık ayarları uygulanmıştır.
- **CNN Modeli:**
  - 3 konvolüsyon katmanı (Conv2D) ve 2 tam bağlantılı (fully connected) katman içerir.
  - Dropout tekniği ile aşırı öğrenme (overfitting) önlenmiştir.
- **Performans Ölçümleri:**
  - Modelin doğruluğu, manipüle edilmiş görüntüler ve renk sabitliği uygulanmış görüntüler üzerinde test edilmiştir.

## Kullanılan Teknolojiler

- **Python**
- **PyTorch**
- **OpenCV**
- **Matplotlib**
- **Scikit-learn**

## Veri Kümesi

Proje, [Animals with Attributes 2 (AWA2)](https://cvml.ist.ac.at/AwA2/) veri kümesini kullanmaktadır. Aşağıdaki hayvan sınıfları çalışmada kullanılmıştır:

- **Collie**
- **Dolphin**
- **Elephant**
- **Fox**
- **Moose**
- **Rabbit**
- **Sheep**
- **Squirrel**
- **Giant Panda**
- **Polar Bear**

Her sınıftan 650 görsel seçilmiş ve eğitim/test veri setleri oluşturulmuştur.

## Sonuçlar

1. **Model Doğruluğu:**
   - CNN modeli: **%72.38** doğruluk.
2. **Manipüle Görseller:**
   - Manipüle edilmiş veri doğruluğu: **%25.00**.
3. **Renk Sabitliği:**
   - Renk sabitliği uygulanmış veri doğruluğu: **%34.85**.

## Görseller

Model performansı aşağıdaki grafikte gösterilmektedir:

![Model Karşılaştırması](./Tablo.png)

## Lisans

Bu proje MIT Lisansı ile lisanslanmıştır. Daha fazla bilgi için [LICENSE](./LICENSE) dosyasına göz atabilirsiniz.
