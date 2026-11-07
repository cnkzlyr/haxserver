# 🥩 Köfteci Yusuf Futsal Pro (%100 Dana Eti Garantili)

**Köfteci Yusuf Futsal Pro**, modern HaxBall sunucuları için geliştirilmiş; dinamik harita ölçekleme (1v1 - 5v5), şov ve gol kutlama animasyonları, gerçek zamanlı şut hız radarı (km/h), direk titremesi, altın gol (uzatma), MVP ödülleri, "Kazanan Sahada Kalır" rotasyonu, AFK koruması ve **en ağır halısaha sövmeleri & racon sistemine** sahip profesyonel bir HaxBall Headless sunucu botudur.

---

## 🌟 Öne Çıkan Özellikler

- 🥩 **%100 Dana Eti & Köfteci Yusuf Teması**: Köfteci Yusuf ızgara unvanları (`🌱 Çırak`, `🍖 Izgaracı`, `🥩 Kasap`, `🔥 Usta Köfteci`, `👑 Köfte Kralı`, `🐐 Yusuf Reis`).
- 🤬 **Ağır Halısaha Küfürleri & Racon**: Kaleciyi, defansı, direği ve kendi kalesine gol atanı yerin dibine sokan en ağır sokak ve halısaha replikleri!
- 🏟️ **Dinamik 1v1 - 5v5 Harita Motoru**: Oyuncu sayısına göre orijinal UZY Futsal haritalarını otomatik seçer ve takımları dengeler (1v1'den 5v5'e pürüzsüz geçiş).
- 👑 **Kral Kutlama Animasyonu**: Gol atan oyuncuya altın disk boyutu, disko aurası ve dönen kutlama emojileri (`👑` Kral Tacı -> `🔥` Alev -> `⚡` Şimşek -> `🐐` GOAT).
- 🎯 **Asist Yıldızı**: Asist yapan oyuncuya özel yeşil ışık (`🎯` -> `👟` -> `✨`).
- 💀 **Rakip Yıkılış Animasyonu**: Gol yiyen takım oyuncularına anlık demoralize ifadeleri (`💀`, `🗿`, `🤦‍♂️`, `📉`, `🤡`) ve küçülme efekti.
- 🤦‍♂️ **Kendi Kalesine Utanç Modu**: Kendi kalesine atan oyuncuya sekmeli utanç ifadeleri (`💩` -> `🤡` -> `🙈`).
- 🚀 **Füze Şut Radarı (km/h)**: Atılan golün ağlara giriş hızını hesaplayarak 70+ km/h şutlarda özel füze duyurusu geçer.
- 💥 **Direk Titremesi ve Ses Efektleri**: Top direğe çarptığında top anlık kor kırmızısına döner, çarpma sesi çalar ve ağır direk sövmesi yapılır.
- ⏳ **Altın Gol & Uzatmalar**: Normal süre berabere bittiğinde maç durmaz; anında "Altın Gol" moduna geçerek ilk golü atanın kazandığı heyecanlı uzatma başlar.
- 🌟 **Maçın Yıldızı (MVP) & Hat-Trick**: Maç boyunca gol ve asistleri puanlayarak maç sonunda resmi MVP'yi taçlandırır; 3 golde Hat-Trick, 4 golde Poker patlatır.
- 🏆 **Kazanan Sahada Kalır (Winner-Stays)**: Kazanan takım serisini korumak için sahada kalır, yenilen takım izleyiciye geçer ve sıradaki izleyiciler oyuna dahil olur (`!streak` serisi tutulur).
- 💤 **Saha İçi AFK Koruması**: Sahada 18 saniye boyunca hareketsiz kalan oyuncu uyarılır, 24 saniyede otomatik izleyiciye çekilerek yerine sıradaki oyuncu alınır.

---

## 🚀 Termux & Linux Başlatma

### 1. Yöntem: Python ile Başlatma (Termux Destekli)

```bash
cd ~/haxserver
python3 start_server.py
```
*(Token istediğinde telefonunuzun tarayıcısından [https://www.haxball.com/headlesstoken](https://www.haxball.com/headlesstoken) linkine girip tokeni kopyalayın ve terminale yapıştırın).*

Veya tokeninizi doğrudan argüman olarak verebilirsiniz:
```bash
python3 start_server.py <BURAYA_TOKENINIZI_YAPISTIRIN>
```

---

### 2. Yöntem: Manuel Tarayıcı Konsolu (Standalone)
1. Tarayıcınızda [Haxball Headless](https://www.haxball.com/headless) sayfasını açın.
2. [Haxball Token Al](https://www.haxball.com/headlesstoken) sayfasından tokeninizi alın.
3. [bot_script.js](file:///data/data/com.termux/files/home/haxserver/bot_script.js) dosyasındaki `BURAYA_ALDIĞINIZ_TOKENI_YAPIŞTIRIN` yerine tokeninizi yapıştırın.
4. Headless sekmesinde `F12` tuşuna basıp (veya İncele -> Konsol) tüm kodu yapıştırıp `Enter`'a basın.

---

## 🎮 Komutlar

### 👥 Müşteri (Oyuncu) Komutları:
| Komut | Açıklama |
|---|---|
| `!yardim` / `!help` | Komut menüsünü gösterir |
| `!stats` | Kişisel istatistiklerinizi ve kasap/köfte unvanınızı gösterir |
| `!stats <isim>` | Başka bir oyuncunun istatistiklerini görüntüler |
| `!top` / `!siralama` | En çok gol atan ve kazanan ilk 3 köfteciyi listeler |
| `!streak` | Sahadaki takımın güncel galibiyet serisini gösterir |
| `!afk` | AFK moduna geçer / sıradan çıkar |
| `!bb` / `!bye` | Sunucudan güvenli ayrılma mesajı |
| `!admin <şifre>` | Yönetici yetkisi alır (Varsayılan şifre: `kofteciyusuf123`) |

### 🛡️ Yönetici (Admin) Komutları:
| Komut | Açıklama |
|---|---|
| `!harita <1-5>` | Haritayı manuel olarak 1v1 - 5v5 tierine ayarlar |
| `!swap` | Kırmızı ve Mavi takımların yerini değiştirir |
| `!lock` / `!unlock` | Takım girişlerini kilitler / açar |
| `!reset` | Maçı anında yeniden başlatır |
| `!kick <id> [sebep]` | Belirtilen oyuncuyu sunucudan atar |
| `!ban <id> [sebep]` | Belirtilen oyuncuyu kalıcı olarak banlar |
| `!karaekle <auth/isim>` | Oyuncuyu kara listeye ekler |
| `!karasil <auth/isim>` | Oyuncuyu kara listeden siler |
| `!mute <id>` / `!unmute <id>` | Oyuncuyu susturur / susturmayı kaldırır |
| `!duyuru <mesaj>` | Tüm odaya renkli ve sesli Köfteci Yusuf duyurusu geçer |

---

## 📄 Lisans
MIT License. %100 Hakiki Dana Eti Garantili.
