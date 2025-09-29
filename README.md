# Space Flipper

## 🎮 Oyun Açıklaması
Tek dokunuşlu casual mobil oyun. Uzayda yerçekimini değiştirerek engellerden kaçın ve yüksek skor elde edin!

## 🚀 Özellikler
- ✅ Tek dokunuş kontrol
- ✅ Sonsuz gameplay
- ✅ Skor sistemi
- ✅ AdMob reklam entegrasyonu
- ✅ IAP (Reklam kaldırma)
- ✅ Android export hazır

## 💰 Para Kazanma Modeli
1. **Banner Reklamlar**: Sürekli görünen alt banner
2. **Interstitial Reklamlar**: Her 3 oyunda bir tam ekran reklam
3. **IAP**: Reklamları kaldırma seçeneği (€2.99)

## 🔧 Kurulum

### Gereksinimler
- Godot 4.2+
- Android SDK
- AdMob hesabı
- Google Play Console hesabı

### Godot'ta Açma
1. Godot'u açın
2. "Import" butonuna tıklayın
3. `project.godot` dosyasını seçin

### Android Export
1. **AdMob Plugin**: Godot Asset Library'den indirin
2. **Google Play Billing Plugin**: Godot Asset Library'den indirin
3. Project → Export → Android
4. Debug keystore oluşturun
5. APK'yı derleyin

### Gerçek Uygulama İçin Değiştirilmesi Gerekenler

#### AdMob ID'leri (scripts/AdManager.gd)
```gdscript
# Test ID'lerini gerçek ID'lerle değiştirin:
var banner_ad_unit_id = "ca-app-pub-XXXXXXXXXXXXXXXX/XXXXXXXXXX"
var interstitial_ad_unit_id = "ca-app-pub-XXXXXXXXXXXXXXXX/XXXXXXXXXX"
var rewarded_ad_unit_id = "ca-app-pub-XXXXXXXXXXXXXXXX/XXXXXXXXXX"
```

#### Uygulama ID'si (android/AndroidManifest.xml)
```xml
<meta-data
    android:name="com.google.android.gms.ads.APPLICATION_ID"
    android:value="ca-app-pub-GERÇEK_APP_ID~XXXXXXXXXX"/>
```

#### Package Name (project.godot & export_presets.cfg)
```
package/unique_name="com.spaceflipper.game"
```

## 📱 Oyun Mekaniği
- **Dokunun**: Uzayda yerçekimi yönünü değiştir
- **Amaç**: Kırmızı engellerden kaçın
- **Puan**: Yeşil alanlardan geçerek puan kazanın
- **Zorluk**: Zaman geçtikçe engel sıklığı artar

## 🎯 Pazarlama Stratejisi
1. **Play Store ASO**: 
   - "space flipper", "casual game", "one tap" anahtar kelimeleri
   - Çekici ekran görüntüleri
   - Kısa oyun traile

2. **Sosyal Medya**:
   - TikTok/Instagram Reels için oyun videoları
   - "Zor seviye" challenge'ları

3. **Influencer Marketing**:
   - Gaming YouTuber'ları ile işbirliği

## 💡 Geliştirme Önerileri

### Hızlı İyileştirmeler
- [ ] Daha fazla renk teması
- [ ] Power-up'lar (slow-mo, shield)
- [ ] Daily challenges
- [ ] Leaderboard (Google Play Games)

### İleri Özellikler
- [ ] Karakter customization
- [ ] Different game modes
- [ ] Multiplayer races
- [ ] Tournament events

## 📊 Beklenen Gelir
- **1K daily users**: ~$10-30/gün
- **10K daily users**: $100-300/gün
- **100K daily users**: $1000-3000/gün

*Not: Gelir tahminleri ülke, retention ve CTR'ye bağlıdır*

## 🚀 Yayın Süreci
1. **Alpha Test**: Internal testing (1 hafta)
2. **Beta Test**: Closed testing (2 hafta)
3. **Soft Launch**: Seçili ülkeler (1 ay)
4. **Global Launch**: Worldwide

## 📝 Yasal Notlar
- Privacy Policy eklemeyi unutmayın
- GDPR compliance
- COPPA compliance (13 yaş altı)
- Terms of Service

---
Made with ❤️ for quick revenue generation!
