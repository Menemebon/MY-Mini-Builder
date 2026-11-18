<h1 align="center">📱 MY BUILDER</h1>
<h3 align="center">Telefonda kodla • Telefonda APK yap • Telefonda imzala</h3>

<p align="center"><b>PC'si olmayanlar için Android uygulama yapım atölyesi.</b></p>

---

## ✨ Ne yapar?

- 🌐 **WEB / SİTE** projelerini **telefonda** imzalı **APK**'ya çevirir (PC yok)
- 🔑 **Keystore** üretir, içe/dışa aktarır, yedekler (.p12)
- 🎮 **Hazır mini oyunlar**: Yılan, Hafıza, Balon Patlat, Zıpla, XOX — oyna ya da projeye ekleyip kendi APK'n yap
- ⚙️ İkon, izinler, tema rengi, tam ekran, JS köprüsü (`Android.toast / share / vibrate / copy / openUrl`)
- 📦 Java / Kotlin projeleri için Android Studio **ZIP** çıktısı

## 🚀 Kurulum (bir kez, PC'de)

1. Android Studio'yu aç → **File > Open** → bu klasörü seç
2. Gradle Sync bitsin ("Use JVM 21" çıkarsa kabul et)
3. **Build > Build APK(s)** → `app/build/outputs/apk/debug/app-debug.apk`
4. APK'yı telefona kur. Bundan sonrası tamamen telefonda.

## 📲 Telefonda kullanım

1. **Yeni Proje** → WEB veya SİTE seç (ya da **Hazır Oyunlar → Projeye ekle**)
2. Kodunu yaz / URL gir → **Test Et**
3. **APK Oluştur** → **Kur** veya **Kaydet / Paylaş**
4. Güncelleme için aynı anahtar şart → **Anahtarlar → Yedekle**

## ⚠️ Sınırlar

- Java/Kotlin projeleri telefonda derlenmez (ZIP → Android Studio)
- Üretilen APK minSdk 24+
- Keystore'unu kaybedersen uygulamayı güncelleyemezsin, yedekle

## 📁 Yapı

```
app/src/main/java/com/mybuilder/app/   → uygulama kodu (Java)
app/src/main/assets/games/             → hazır oyunlar (HTML)
app/src/main/assets/template/          → ZIP çıktısı şablonu
```

---
<p align="center">Made with ❤️ — <b>My Builder</b></p>
