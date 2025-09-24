# Intel Görüntü Sınıflandırma (EfficientNetB0)

## Proje Amacı
- Projenin amacı, Akbank Derin Öğrenme Bootcamp'i kapsamında **görüntü sınıflandırma modeli geliştirmek ve modelin performansını değerlendirmektir.**

## Veri Seti Hakkında
- **Adı:** Intel Image Classification
- **Sınıflar:** Buildings, Forest, Glacier, Mountain, Sea, Street
- **Boyut:** ~25.000 eğitim, 14.000 test görüntüsü

## Kullanılan Yöntemler
- **Model:** Transfer öğrenme ile önceden eğitilmiş **EfficientNetB0** modeli kullanılmıştır.
- **Veri Ön İşleme:** Görüntülerin boyutu 224x224 piksele yeniden boyutlandırıldı.
- **Veri Artırımı (Data Augmentation):** Modelin genelleme yeteneğini artırmak için yatay çevirme, döndürme ve yakınlaştırma gibi teknikler uygulandı.

## Elde Edilen Sonuçlar
- **Doğruluk ve Kayıp Grafikleri:**
  * Aşağıdaki grafikler, modelin eğitim ve doğrulama setlerinde başarılı bir şekilde öğrendiğini, **doğruluk (accuracy)** değerinin yükseldiğini ve **kayıp (loss)** değerinin düştüğünü göstermektedir. Overfitting gözlemlenmemiştir.
  * (Grafiklerin ekran görüntüsünü buraya ekleyebilirsiniz.)

- **Test Seti Sonuçları:**
  * **Test Doğruluğu (Test Accuracy):** [Kaggle Notebook'unuzdaki **Hücre 11**'in çıktısından bu değeri kopyalayın ve buraya yapıştırın.]
  * **Sınıflandırma Raporu:**
    ```
    [Kaggle Notebook'unuzdaki **Hücre 11**'in çıktısından sınıflandırma raporunu kopyalayın ve buraya yapıştırın.]
    ```

- **Grad-CAM Görselleştirmesi:**
  * Modelin hangi bölgelere odaklandığını gösteren **Grad-CAM** görselleri, modelin başarılı bir şekilde [örnek bir sınıf adı yazın, örn: "Buildings" veya "Forest"] gibi sınıfları ayırt ederken doğru nesnelere odaklandığını göstermektedir.
  * (Grad-CAM görselinin ekran görüntüsünü buraya ekleyebilirsiniz.)

---

**Kaggle Notebook Linki:** [Kaggle projenizin linkini buraya yapıştırın.]
