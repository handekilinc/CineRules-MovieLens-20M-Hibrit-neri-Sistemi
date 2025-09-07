<h1 align="center">🎬 Hybrid Movie Recommendation System</h1>  

---

## 📂 Dataset Information  

Bu proje, **MovieLens (20M Dataset)** verisi kullanılarak gerçekleştirilmiştir.  

**Veri seti şunları içermektedir:**  
- 🎞️ `rating.csv` → Kullanıcıların filmlere verdiği puanlar  
- 🎬 `movie.csv` → Filmlere ait başlık ve tür bilgileri  
- 🏷️ `tag.csv` → Kullanıcıların filmlere uyguladığı etiketler  
- 🔗 `link.csv` → IMDb ve TMDb kimlikleri  
- 📊 `genome_scores.csv` → Film–etiket alaka düzeyi  
- 📝 `genome_tags.csv` → Etiket açıklamaları  

**Veri Özeti:**  
- 🎥 27.278 film  
- 👥 138.493 kullanıcı  
- ⭐ 20.000.263 rating  
- 🏷️ 465.564 tag  

---

## 🎯 Project Objectives  

- 👤 Kullanıcıların geçmiş film izleme ve puanlama davranışlarını analiz ederek kişiselleştirilmiş film önerileri sunmak  
- 🔗 Birliktelik Kuralı (Association Rule Mining) ve **Collaborative Filtering (CF)** yöntemlerini birleştirerek hibrit öneri sistemi tasarlamak  
- ⚡ Daha ölçeklenebilir ve optimize edilmiş öneri sistemi geliştirmek  

---

## 📝 Project Overview  

Öneri sistemleri, kullanıcıya ilgisini çekebilecek içerikleri tahmin etmeyi amaçlar.  

📌 Bu projede:  
- 📚 **Birliktelik Kuralı (Apriori)** → Filmler arasındaki birlikte izlenme ilişkileri bulundu.  
- 👥 **Collaborative Filtering (CF)** → Kullanıcıların tercihleri üzerinden öneriler üretildi.  
- 🔀 **Hibrit Model** → Apriori + CF birleşimi ile daha güvenilir ve çeşitli öneriler sağlandı.  

---

## 🔑 What is Association Rule Mining?  

Birliktelik kuralı, kullanıcıların geçmiş davranışlarından:  
**“X izlendiyse, Y de izlenir”** şeklinde ilişki kuralları çıkarmayı sağlar.  

Örneğin:  
👉 Eğer bir kullanıcı **The Matrix** izlediyse, yüksek olasılıkla **Inception** da izlemiştir.  

Bu projede **Apriori algoritması** ile kurallar çıkarıldı ve öneri sistemine entegre edildi.  

---

## 🛠️ Libraries Used  

Projede aşağıdaki Python kütüphaneleri kullanılmıştır:  
- 🐼 **pandas** → Veri işleme  
- 🔢 **numpy** → Sayısal hesaplamalar  
- 📐 **mlxtend** → Apriori & Association Rules  
- 📊 **matplotlib** → Veri görselleştirme  
- 🌐 **networkx** (opsiyonel) → Kuralların grafiksel gösterimi  

---

## 📌 Project Steps  

1. **Veri Hazırlama**  
   - Eksik verilerin kontrolü  
   - Kullanıcı × Film pivot matrisi oluşturma  
   - One-Hot Encoding  
   - Rating ≥ 4 olan filmleri **beğenilen (liked)** olarak işaretleme  

2. **Birliktelik Kuralları (Apriori)**  
   - En sık birlikte izlenen film kümelerini bulma  
   - Confidence & Lift metrikleri ile filtreleme  

3. **Collaborative Filtering (CF)**  
   - Kullanıcıların izlediği filmler üzerinden benzer kullanıcı davranışlarını analiz etme  

4. **Hybrid Model**  
   - Apriori + CF birleşimi ile öneriler üretme  

5. **Visualization**  
   - 📊 İlk 10 kullanıcı için öneri sonuçlarını grafikle gösterme  

---

## 🔮 Future Work  

- 🤖 **Deep Learning** tabanlı modeller (Autoencoders, Neural Collaborative Filtering) ile daha güçlü öneriler geliştirmek  
- ⏳ Zaman serisi analizi yaparak film tercihlerindeki dönemsel değişimleri incelemek  
- 📝 Content-based filtering ile film açıklamalarını ve tür bilgilerini kullanmak  
- 🌍 Gerçek zamanlı öneri sistemi (ör. bir web app) geliştirmek  

---

## ✅ Conclusion  

Bu proje, **birliktelik kuralları** ve **işbirlikçi filtreleme** yöntemlerini birleştirerek **hibrit bir öneri sistemi** ortaya koymuştur.  

- 📌 Apriori algoritması ile güçlü film ilişkileri keşfedildi.  
- 👤 Collaborative Filtering ile kullanıcıya özel öneriler üretildi.  
- 🔀 Hibrit model, yalnızca tek bir yönteme dayalı sistemlere kıyasla daha **zengin, çeşitli ve güvenilir** öneriler sağladı.  

🎯 **Sonuç olarak**, bu çalışma gelecekte daha gelişmiş makine öğrenimi ve derin öğrenme tabanlı öneri sistemleri için sağlam bir temel sunmaktadır.  

---

## 📌 Reference  

F. Maxwell Harper and Joseph A. Konstan. 2015. *The MovieLens Datasets: History and Context.*  
ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4, Article 19.  
DOI: [10.1145/2827872](http://dx.doi.org/10.1145/2827872)  
