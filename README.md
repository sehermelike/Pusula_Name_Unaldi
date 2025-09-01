# Pusula Intern Data Science Case

*Ad Soyad:Seher Melike Ünaldı* 
*Email: sehermelikeunaldi@gmail.com* 

---

## 📌 Proje Hakkında
Bu proje, *Pusula Intern Data Science Case* kapsamında verilen fizik tedavi ve rehabilitasyon veri seti üzerinde yapılmıştır.  
Amaç, hedef değişken olan *TedaviSuresi* etrafında veri setini keşfetmek (EDA) ve *modellemeye hazır hale getirmektir*.  

---

## 🔎 Adımlar
### 1. Exploratory Data Analysis (EDA)
- Veri tipleri ve özet istatistikler incelendi.  
- Eksik değerler analiz edildi.  
- Görselleştirmeler yapıldı:
  - Histogram (sayısal değişkenler)  
  - Barplot (kategorik değişkenler)  
  - Korelasyon matrisi (sayısal değişkenler arası)  
  - Hedef değişken (TedaviSuresi) dağılımı  

### 2. Data Pre-processing
- Eksik değerler SimpleImputer ile dolduruldu.  
- *KronikHastalik* ve *Alerji* sütunları virgülle ayrılmış değerler olarak geldi → özel fonksiyon ile *multi-label one-hot encoding* uygulandı.  
- Kardinalite kontrolü yapıldı:  
  - Düşük kardinaliteli sütunlar → *OneHotEncoder*  
  - Yüksek kardinaliteli sütunlar → *frequency encoding*  
- Sayısal değişkenler StandardScaler ile normalize edildi.  
- Sonuç: *modelleme için temiz ve tutarlı bir veri seti*.  

---

## ⚙️ Kullanım
1. Dosyaları Colab veya lokal ortamınıza alın.  
2. Talent_Academy_Case_DT_2025.xlsx dosyasını proje klasörüne koyun.  
3. Notebook’u çalıştırın:  
   ```bash
   python main.py
