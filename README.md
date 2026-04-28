# GreenwashingNLP: Türkçe Metin Analiz Modeli 🌿

Bu proje, kurumsal sürdürülebilirlik iddialarını analiz ederek **"Greenwashing"** (Yanıltıcı Çevreci İddialar) içeren ifadeleri tespit etmek amacıyla geliştirilmiş bir Doğal Dil İşleme (NLP) prototipidir.

---

## 🚀 Proje Hakkında
Sistem, **BERTurk** mimarisi üzerine inşa edilmiş olup, Türkçe doğal dil işleme yetenekleri ile metin tabanlı verileri gelişmiş derin öğrenme yöntemleriyle sınıflandırır. 

* **Hız:** Cümle başına ~100-200ms çıkarım (inference) süresi ile real-time kullanıma uygundur.
* **Standartlar:** Analiz kriterleri belirlenirken **EU Green Claims Directive** ve **FTC Green Guides** referans alınmıştır.
* **Model:** `dbmdz/bert-base-turkish-cased` tabanlı, özel veri seti ile optimize edilmiş fine-tuned model.

### 📊 Model Performans Grafikleri
Eğitim süreci boyunca modelin hata (loss), doğruluk (accuracy) ve F1-Score değerlerinin takibi yapılmıştır. Grafikler, modelin istikrarlı bir şekilde öğrendiğini ve test verisi üzerindeki başarısını göstermektedir:

<img width="1472" height="399" alt="image" src="https://github.com/user-attachments/assets/8b426d35-1c18-4d9d-939d-cd082899c41c" />
<img width="1473" height="950" alt="image" src="https://github.com/user-attachments/assets/1caf25fe-d4b7-46c7-9ff8-5c6596f9f229" />


---

## 🛠️ Kurulum ve Kullanım
Bu depo, sistemin **mimari iskeletini ve çıkarım (inference) mantığını** sergilemek amacıyla oluşturulmuştur. 

> **Not:** Modelin ağırlık dosyaları (`.safetensors`) ticari gizlilik nedeniyle bu repoya dahil edilmemiştir. Bu nedenle `predict.py` dosyası yerelinizde doğrudan çalışmayacaktır. Kod yapısını inceleyerek sistemin nasıl bir boru hattı (pipeline) üzerinde çalıştığını görebilirsiniz.
> 
## 📂 Dosya Yapısı

 **src/predict.py: ** Modelin metinleri analiz ettiği canlı tahmin modülü.

 **models/: **  Modelin mimari kimliğini belirleyen konfigürasyon ve tokenizer dosyaları.

 **requirements.txt: ** Projenin çalışması için gerekli kütüphane bağımlılıkları.

## [!IMPORTANT]

Ticari Gizlilik Notu: Eğitim veri setleri, veri dengeleme algoritmaları ve tam model ağırlıkları (.safetensors), fikri mülkiyetin korunması ve ticari gizlilik nedeniyle bu kamuya açık (public) depoda paylaşılmamıştır. 

##  📧 İletişim
Elif Nur Ayhan - eifnurayhan671@gmail.com
