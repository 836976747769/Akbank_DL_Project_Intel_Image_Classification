# Intel Görüntü Sınıflandırma (EfficientNetB0)

##  Giriş
Bu proje, **Akbank Derin Öğrenme Bootcamp** kapsamında gerçekleştirilmiştir.  
Amaç, Kaggle üzerinde bulunan **Intel Image Classification** veri seti ile farklı sahneleri sınıflandıracak bir derin öğrenme modeli geliştirmektir.  

Projede **EfficientNetB0** tabanlı transfer learning yaklaşımı kullanılmıştır.  
Veri artırma, erken durdurma (EarlyStopping), öğrenme oranı azaltma (ReduceLROnPlateau) ve Grad-CAM gibi yöntemlerle modelin başarımı artırılmış ve sonuçları görselleştirilmiştir.  

---

## Metrikler
Eğitim süreci sonunda elde edilen sonuçlar:  
- **Başlangıç doğruluk:** ~%70  
- **Fine-tuning sonrası doğruluk:** ~%89-90  
- **Kayıp (loss):** ~0.30 seviyelerine kadar düşmüştür.  

 Bu değerler, modelin çok sınıflı görüntü sınıflandırma görevinde yüksek doğrulukla çalışabildiğini göstermektedir.  

---

##  Ekler
- **Grad-CAM görselleştirmeleri:** Modelin karar verirken görüntünün hangi bölgelerine odaklandığını açıklamaktadır.  
- **GPU Kullanımı:** Kaggle T4 GPU üzerinde eğitim yapılmıştır.  
- **Model Kaydı:** En iyi epoch sonrası `best_model.h5` dosyası kaydedilmiştir.  

Ek çalışmalar olarak:  
- Farklı CNN backbone’ları ile (ResNet, VGG16) karşılaştırma yapılabilir.  
- Streamlit veya Gradio ile basit bir kullanıcı arayüzü geliştirilebilir.  

---

##  Sonuç ve Gelecek Çalışmalar
Bu proje ile sahne sınıflandırma problemine başarılı bir çözüm üretilmiştir.  

**Gelecekte yapılabilecekler:**  
- Daha geniş veri setleri ile yeniden eğitim  
- Modelin mobil cihazlar için optimize edilmesi  
- Gerçek zamanlı görüntü sınıflandırma uygulamaları geliştirilmesi  
- Kullanıcıların kendi görsellerini yükleyip sınıflandırabileceği bir web arayüzü hazırlanması  

---

## 🔗 Linkler
-  **Kaggle Notebook:** [Projeyi buradan inceleyebilirsiniz](https://www.kaggle.com/code/selimegndz/akbank)  
-  **Veri Seti:** [Intel Image Classification Dataset](https://www.kaggle.com/puneet6060/intel-image-classification)  
