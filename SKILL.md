---
name: turkce-humanizer
description: Yapay zekâyla yazılmış Türkçe metindeki "bunu yapay zekâ yazmış" dedirten izleri temizler ve metni doğal, insan yazmış gibi yeniden yazar. Kullanıcı "insan gibi yaz", "yapay zekâ kokmasın", "doğallaştır", "humanize", "robot gibi durmasın" dediğinde ya da Türkçe bir metni düzeltmeni istediğinde kullan.
---

# Türkçe Humanizer

Görevin: verilen Türkçe metnin **anlamını ve bilgilerini koruyarak** yapay zekâ izlerini temizlemek. Yeni bilgi ekleme, iddia uydurma, kaynak uydurma. Metnin tonunu koru: resmi metin resmi, samimi metin samimi kalsın.

## 1. Bu izleri bul

| # | İz | Örnek (önce) | Nasıl düzelt |
|---|---|---|---|
| 1 | Klişe açılış | "Günümüzde teknolojinin hızla geliştiği bu dönemde..." | Doğrudan konuya gir. |
| 2 | Klişe kapanış | "Sonuç olarak...", "Özetle...", "Unutmayın ki..." | Son cümleyi asıl fikirle bitir ya da sil. |
| 3 | Şişirilmiş önem | "kritik bir öneme sahiptir", "hayati bir rol oynamaktadır", "devrim niteliğinde" | Somut söyle: neyi, ne kadar değiştiriyor? |
| 4 | "Sadece... değil, aynı zamanda..." | "Sadece hızlı değil, aynı zamanda güvenli." | "Hızlı ve güvenli." ya da iki ayrı cümle. |
| 5 | Üçleme takıntısı | "hızlı, güvenilir ve etkili", her listede tam 3 madde | Gerçekte kaç tane varsa o kadar yaz. |
| 6 | -mektedir / edilgen yığını | "gerçekleştirilmektedir", "sağlanmaktadır", "kullanılmaktadır" | Etken ve kısa: "yapıyor", "sağlıyor", "kullanıyoruz". |
| 7 | Bağlaç merdiveni | Her paragraf "Ayrıca", "Bunun yanı sıra", "Öte yandan", "Dolayısıyla" ile başlıyor | Çoğunu sil; cümleler kendi bağlansın. |
| 8 | Dolgu kalıpları | "Bu bağlamda", "bu doğrultuda", "söz konusu", "belirtmek gerekir ki", "önemli bir nokta" | Sil. |
| 9 | Kaynaksız otorite | "Uzmanlara göre", "Araştırmalar gösteriyor ki" (kaynak yok) | Kaynak varsa adını yaz, yoksa iddiayı yumuşat ya da sil. |
| 10 | Kaçamak dil | "genel olarak", "bir nevi", "belki de", "bir ölçüde" üst üste | En fazla bir tane bırak. |
| 11 | Asistan sesi | "Harika soru!", "Umarım yardımcı olur", "İşte size ...:" | Sil. |
| 12 | Uzun tire ve dramatik iki nokta | "Sonuç belli — başarı." | Virgül, nokta ya da düz cümle. |
| 13 | Biçim süsü | Her şey madde işaretli, her yerde **kalın**, emoji madde başları, "Başlık Gibi Büyük Harf" | Düz paragraf; kalın en fazla bir yerde. |
| 14 | Tekdüze ritim | Bütün cümleler aynı uzunlukta | Kısa ve uzun cümleleri karıştır. Ara sıra çok kısa bir cümle. |
| 15 | Ahlak dersi kapanışı | "...ancak her teknolojide olduğu gibi bilinçli kullanmak gerekir." | Metin istemiyorsa sil. |
| 16 | Soyut kelime kalabalığı | "süreç", "yapı", "dinamik", "potansiyel", "boyut" | Somut özne ve eylem: kim, ne yaptı? |

## 2. Yeniden yaz
1. Önce metnin ne söylediğini tek cümleyle kendine özetle. Bu anlam değişmeyecek.
2. Yukarıdaki izleri tek tek temizle.
3. Etken çatı, somut kelimeler, gerçek örnekler kullan (metinde varsa).
4. Cümle uzunluklarını karıştır. Gereksiz her kelimeyi at.
5. Kullanıcının metni samimiyse konuşma diline yakın kal; resmiyse resmi ama sade kal.
6. Sayıları, adları, tarihleri, alıntıları **aynen** koru.

## 3. Son kontrol
- Anlam ve bilgiler aynı mı? Yeni iddia eklemedin mi?
- Tablodaki izlerden kaldı mı? (Özellikle 1, 2, 4, 6, 7, 8)
- Sesli okununca bir insan böyle konuşur mu?

## Çıktı
Sadece düzeltilmiş metni ver. Kullanıcı isterse altına kısa bir "neleri değiştirdim" listesi ekle.

> Not: Bu bir düzenleme aracıdır. Kopya, intihal ya da kural ihlali için değil, metnin robot gibi durmaması için kullan.

Uyarlama: [blader/humanizer](https://github.com/blader/humanizer) (Siqi Chen, MIT) ve Wikipedia "Signs of AI writing" rehberi fikrinden Türkçe için yeniden yazılmıştır.
