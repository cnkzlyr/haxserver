# ⚡ Galaxy Futsal Pro - Advanced HaxBall Headless Host

**Galaxy Futsal Pro**, modern HaxBall sunucuları için geliştirilmiş; dinamik harita ölçekleme (1v1 - 5v5), şov ve gol kutlama animasyonları, gerçek zamanlı şut hız radarı (km/h), direk çarpma efektleri, altın gol (uzatma), MVP ödülleri, "Kazanan Sahada Kalır" rotasyonu, AFK koruması ve gerçekçi sokak/halısaha racon sistemine sahip profesyonel bir HaxBall Headless botudur.

---

## 🌟 Öne Çıkan Özellikler

- 🏟️ **Dinamik 1v1 - 5v5 Harita Motoru**: Odadaki oyuncu sayısına göre orijinal UZY Futsal haritalarını otomatik olarak seçer ve takımları dengeler (1v1'den 5v5'e kesintisiz geçiş).
- 👑 **Gol & Şov Kutlama Animasyonları**: Gol atan oyuncuya parlayan altın disk, kral tacı (`👑`), alev (`🔥`), şimşek (`⚡`) ve keçi (`🐐`) animasyonu. Asist yapan maestrolara özel yeşil parıltı (`🎯`, `👟`, `✨`).
- 💀 **Rakip Yıkılış Efekti**: Gol yiyen takım oyuncularına anlık demoralize ifadeleri (`💀`, `🗿`, `🤦‍♂️`, `📉`, `🤡`) ve küçülme efekti.
- 🚀 **Füze Şut Radarı (km/h)**: Atılan golün ağlara giriş hızını hesaplayarak 70+ km/h şutlarda özel füze duyurusu geçer.
- 💥 **Direk Titremesi ve Ses Efektleri**: Top direğe çarptığında top anlık kor kırmızısına döner, çarpma sesi çalar ve gerçekçi direk sövmesi yapılır.
- ⏳ **Altın Gol & Uzatmalar**: Normal süre berabere bittiğinde maç durmaz; anında "Altın Gol" moduna geçerek ilk golü atanın kazandığı heyecanlı uzatma başlar.
- 🌟 **Maçın Yıldızı (MVP) & Hat-Trick / Poker**: Maç boyunca gol, asist ve kendi kalesine atılan golleri puanlayarak maç sonunda resmi MVP'yi ve hat-trick yapanları taçlandırır.
- 🏆 **Kazanan Sahada Kalır (Winner-Stays)**: Kazanan takım serisini korumak için sahada kalır, yenilen takım izleyiciye geçer ve sıradaki izleyiciler oyuna dahil olur. Seri galibiyet sayacı aktiftir.
- 💤 **Saha İçi AFK Koruması**: Sahada 18 saniye boyunca hareketsiz kalan oyuncu uyarılır, 24 saniyede otomatik izleyiciye çekilerek yerine sıradaki oyuncu alınır.
- 📊 **Gelişmiş İstatistik & Rütbe Sistemi**: Gol, asist, kendi kalesine, galibiyet oranı, seri ve MVP sayısına göre unvanlar (`🌱 Çaylak`, `⚽ Amatör`, `🔥 Futsalcı`, `⚡ Pro`, `👑 Usta`, `🐐 Efsane`).
- 🗣️ **Gerçekçi Halısaha & Haxball Raconu**: Cinsel içerikten arındırılmış, halısahanın ve rekabetçi Haxball kültürünün saf hırsını ve heyecanını yansıtan gerçekçi tepkiler.

---

## 🚀 Başlatma Yöntemleri

### 1. Yöntem: Tam Otomatik Python Host (Önerilen)
Chrome arka planda çalışarak [Haxball Headless Token](https://www.haxball.com/headlesstoken) sayfasından tokeni otomatik çözer ve sunucuyu başlatır:

```bash
python3 start_server.py
```
> Terminalde çıkan `Oda Linki: https://www.haxball.com/play?c=...` bağlantısını kopyalayıp oyuncularla paylaşabilirsiniz.

---

### 2. Yöntem: Manuel Tarayıcı Konsolu (Standalone)
1. Tarayıcınızda [Haxball Headless](https://www.haxball.com/headless) sayfasına gidin.
2. [Haxball Token Al](https://www.haxball.com/headlesstoken) sayfasından tokeninizi alın.
3. [bot_script.js](file:///data/data/com.termux/files/home/haxserver/bot_script.js) dosyasındaki `BURAYA_ALDIĞINIZ_TOKENI_YAPIŞTIRIN` kısmına tokeninizi yapıştırın.
4. Headless sekmesinde `F12` tuşuna basıp **Console (Konsol)** sekmesine tüm kodu yapıştırıp `Enter`'a basın.

---

## 🎮 Komutlar

### 👥 Oyuncu Komutları:
| Komut | Açıklama |
|---|---|
| `!yardim` / `!help` | Komut listesini gösterir |
| `!stats` | Kişisel istatistiklerinizi ve rütbenizi görüntüler |
| `!stats <isim>` | Belirtilen oyuncunun istatistiklerini görüntüler |
| `!top` / `!siralama` | Sunucunun en çok gol atan ve kazanan ilk 3 oyuncusu |
| `!streak` | Sahadaki takımın güncel galibiyet serisini gösterir |
| `!afk` | AFK moduna geçip sıradan çıkar / geri döner |
| `!bb` / `!bye` | Sunucudan ayrılma mesajı |
| `!admin <şifre>` | Yönetici yetkisi alır (Varsayılan: `galaxyadmin2026`) |

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
| `!duyuru <mesaj>` | Tüm odaya renkli ve sesli duyuru geçer |

---

## ⚙️ Yapılandırma

Ayarları değiştirmek için [bot_script.js](file:///data/data/com.termux/files/home/haxserver/bot_script.js) veya [start_server.py](file:///data/data/com.termux/files/home/haxserver/start_server.py) dosyalarındaki değişkenleri güncelleyebilirsiniz:
- `ADMIN_PASSWORD`: Yönetici şifresi (varsayılan: `galaxyadmin2026`)
- `roomName`: Oda başlığı
- `scoreLimit`: Varsayılan skor limiti (varsayılan: 5)
- `timeLimit`: Varsayılan süre limiti (varsayılan: 3 dk)

---

## 📄 Lisans
MIT License. Özgürce geliştirebilir, kullanabilir ve dağıtabilirsiniz.
