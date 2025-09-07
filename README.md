# CineRules-MovieLens-20M-Hibrit-Oneri-Sistemi
Bu proje, MovieLens 20M veri seti kullanılarak film tavsiye sistemleri (recommendation systems) üzerine geliştirilmiştir. Öneri sistemleri, kullanıcıların geçmiş tercihlerini ve benzer kullanıcıların davranışlarını analiz ederek kişiselleştirilmiş öneriler sunmayı amaçlar.

Proje iki ana yaklaşımı birleştirmektedir:

Collaborative Filtering (İşbirlikçi Filtreleme):
Kullanıcıların benzerliklerine ve film puanlama kalıplarına dayanarak tahminleme yapar. Matrix Factorization ve kullanıcı-film benzerlik yöntemleri bu kapsamda uygulanmıştır.

Association Rule Mining (Birliktelik Kuralları):
Kullanıcıların yüksek puan verdiği filmleri “alışveriş sepeti” gibi ele alarak, sık birlikte değerlendirilen film gruplarını keşfeder. Böylece “Bu filmi izleyen kullanıcılar, şu filmleri de izledi” mantığıyla öneriler üretir.

Bu hibrit yaklaşım sayesinde:

Sadece popüler filmlere değil, aynı zamanda birlikte sık tercih edilen filmlere dayalı öneriler yapılır.

Kullanıcıya daha çeşitli, anlamlı ve açıklanabilir tavsiyeler sunulur.

🔍 Projede Ele Alınan Başlıca Adımlar

Veri keşfi (EDA) ve ön işleme

Popülerlik tabanlı ve içerik tabanlı (content-based) baseline modeller

Collaborative Filtering (User-User, Item-Item, Matrix Factorization)

Birliktelik kuralları (Apriori / FP-Growth) ile film eşleştirme

Hibrit öneri modeli (CF + Association Rules)

Performans değerlendirmesi (RMSE, Precision@K, Recall@K, NDCG)

🎯 Hedef

Bu proje, öneri sistemleri alanında farklı yaklaşımları birleştirerek hem akademik çalışmalara hem de gerçek dünya uygulamalarına ışık tutmayı hedeflemektedir.
