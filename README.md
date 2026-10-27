# Türkçe Humanizer 🇹🇷

Yapay zekâya yazdırdığın Türkçe metindeki "bunu yapay zekâ yazmış" dedirten izleri temizleyen agent skill. Claude, ChatGPT, Codex, Cursor ve talimat dosyası kabul eden her araçta çalışır.

**Neden?** Orijinal [Humanizer](https://github.com/blader/humanizer) İngilizce kalıplar için yazıldı. Türkçe metinlerin kendi izleri var: "Günümüzde..." diye açılış, "Sonuç olarak..." diye kapanış, "-mektedir" yığınları, "sadece... değil, aynı zamanda..." kalıbı, her paragrafa "Ayrıca / Bunun yanı sıra". Bu skill 16 Türkçe izi tanır ve metni anlamını bozmadan doğallaştırır.

## Önce / sonra
**Önce:** Günümüzde yapay zekâ, iş süreçlerinde kritik bir öneme sahip olup sadece verimliliği artırmakla kalmamakta, aynı zamanda maliyetleri de düşürmektedir. Sonuç olarak, şirketlerin bu teknolojiye uyum sağlaması büyük önem taşımaktadır.

**Sonra:** Yapay zekâ şirketlerde hem işi hızlandırıyor hem masrafı düşürüyor. Uyum sağlamayan geride kalacak.

## Kurulum
**Claude Code:**
```bash
git clone https://github.com/ibrahimdiken/turkce-humanizer ~/.claude/skills/turkce-humanizer
```
Sonra Claude'a "bu metni insan gibi yaz" demen yeterli.

**Claude (web/masaüstü):** Ayarlar → Yetenekler → Skills → bu klasörü zip yapıp yükle.

**ChatGPT / Gemini / diğerleri:** `SKILL.md` dosyasının içeriğini kopyala, Proje talimatına (ya da Özel GPT / Gem talimatına) yapıştır.

## Uyarı
Bu bir düzenleme aracı. Kopya, intihal ya da kural ihlali için değil, metnin robot gibi durmaması için kullan.

## Teşekkür
- [blader/humanizer](https://github.com/blader/humanizer), Siqi Chen (MIT). Fikir ve yapı buradan; Türkçe kalıplar ve metin yeniden yazıldı.
- Wikipedia'nın "Signs of AI writing" rehberi (WikiProject AI Cleanup gönüllüleri).

Hazırlayan: [İbrahim Diken](https://github.com/ibrahimdiken) · YouTube & Instagram: @devibrahimdiken
