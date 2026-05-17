# ChordFinder 🎸

> Şarkılarından gitar akorlarını otomatik olarak tespit eden, açık kaynaklı web uygulaması.

![ChordFinder](https://img.shields.io/badge/ChordFinder-v1.0.0-7C73FF?style=for-the-badge&logo=guitar&logoColor=white)
![License](https://img.shields.io/badge/Lisans-MIT-34d399?style=for-the-badge)
![No Server](https://img.shields.io/badge/Sunucu-Gerekmez-ff6b9d?style=for-the-badge)
![Vanilla JS](https://img.shields.io/badge/Vanilla-JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## ✨ Özellikler

- 🎵 **Otomatik Akor Tespiti** — MP3, MP4, WAV veya OGG dosyandan gitar akorlarını bulur
- 🔑 **Ton Seçimi** — İstersen orijinal tonu kullan, istersen başka bir tona transpoz et
- 📊 **Zaman Damgaları** — Her akorun şarkıda nerede geçtiğini gösterir
- 🎸 **Gitar Diyagramları** — SVG tabanlı parmak pozisyonu diyagramları
- 🌙 **Dark / Light Mod** — Tercih tarayıcıya kaydedilir
- 📋 **Panoya Kopyala** — Akor ilerlemesini tek tıkla kopyala
- ⬇️ **TXT İndir** — Tüm sonuçları metin dosyası olarak indir
- 🔒 **%100 Gizlilik** — Hiçbir dosya sunucuya gönderilmez, her şey tarayıcıda çalışır

---

## 🚀 Nasıl Kullanılır

### 1. Dosya Yükle
MP3, MP4, WAV veya OGG formatında bir müzik dosyası sürükle-bırak yap ya da dosya seçici ile seç.

### 2. Ton Seç
- **Orijinal tonu kullan** *(varsayılan)* — Şarkının kendi tonunda analiz yapar
- **Ton seç** — 12 ton arasından istediğini seç ve Majör/Minör modunu belirt

### 3. Analiz Et
"Analiz Et" butonuna bas. Web Audio API ile sesini işler, kromatik özellikler çıkarır ve akorları tespit eder.

### 4. Sonuçları İncele
- Tespit edilen akor ilerlemesini gör
- Her akorun zaman damgasını ve gitar diyagramını incele
- Sonuçları panoya kopyala veya TXT olarak indir

---

## 🛠 Teknolojiler

| Katman | Teknoloji |
|--------|-----------|
| Arayüz | HTML5 + CSS3 + Vanilla JavaScript |
| Ses İşleme | Web Audio API (Native Browser API) |
| Pitch Analizi | FFT (Fast Fourier Transform) — Özel implementasyon |
| Ton Tespiti | Krumhansl-Schmuckler Anahtar Tanıma Algoritması |
| Akor Eşleştirme | Kromatik özellik + şablon korelasyon |
| Fontlar | Syne + DM Mono + DM Sans (Google Fonts CDN) |
| Diyagramlar | SVG (sunucusuz, inline) |

---

## 📦 Kurulum

**Sunucu gerekmez.** Tek bir HTML dosyasından oluşur.

```bash
# 1. Repoyu klonla
git clone https://github.com/efearslanbass/chordfinder.git

# 2. Klasöre gir
cd chordfinder

# 3. index.html dosyasını tarayıcında aç
# (Çift tıkla veya aşağıdaki komutla)
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

Ya da doğrudan indirip çift tıklayabilirsin. Hepsi bu!

> **Not:** İnternet bağlantısı yalnızca Google Fonts CDN için gereklidir. Ses analizi tamamen çevrimdışı çalışır.

---

## 🔒 Gizlilik

ChordFinder'da yüklediğin dosyalar **hiçbir sunucuya gönderilmez**.

- Tüm ses işleme tarayıcının **Web Audio API**'si ile yapılır
- Hiçbir veri depolanmaz veya iletilmez
- Kullanıcı tercihleri (dark/light mod) yalnızca kendi tarayıcına (localStorage) kaydedilir

---

## 🎸 Desteklenen Akorlar

Uygulama aşağıdaki akor türlerini tanıyabilir:

`C` `Cm` `D` `Dm` `E` `Em` `F` `Fm` `G` `Gm` `A` `Am` `B` `Bm`
`C#` `C#m` `D#` `D#m` `F#` `F#m` `G#` `G#m` `A#` `A#m`

Her akor için SVG tabanlı gitar parmak diyagramı gösterilir.

---

## 🤝 Katkıda Bulunma

Pull request'ler ve issue'lar memnuniyetle karşılanır!

```bash
# Fork'la → Clone et → Branch oluştur → Değişiklik yap → PR aç
git checkout -b feature/yeni-ozellik
git commit -m "feat: yeni özellik eklendi"
git push origin feature/yeni-ozellik
```

### Katkı Fikirleri
- [ ] Daha fazla akor şekli eklemek
- [ ] BPM (tempo) tespiti
- [ ] MIDI export özelliği
- [ ] Çoklu dil desteği
- [ ] Mobil PWA desteği
- [ ] Gerçek zamanlı mikrofon analizi

---

## 📄 Lisans

Bu proje **MIT Lisansı** altında dağıtılmaktadır. Detaylar için [LICENSE](./LICENSE) dosyasına bakın.

---

<div align="center">

Müzisyenler için, müzisyenler tarafından yapıldı 🎵

**[⭐ Star ver](https://github.com/efearslanbass/chordfinder)** • **[🐛 Bug bildir](https://github.com/efearslanbass/chordfinder/issues)** • **[💡 Öneri sun](https://github.com/efearslanbass/chordfinder/issues)**

</div>
