# Antrenmanım – Android fitness uygulaması

## APK'yı bilgisayar kurmadan alma (GitHub ile, yaklaşık 5 dakika)
1. github.com'da ücretsiz hesap aç, sağ üstten **+ → New repository** ile boş bir depo oluştur.
2. Depo sayfasında **"uploading an existing file"** bağlantısına tıkla ve bu klasörün **içindeki her şeyi** sürükle-bırak (`.github` klasörü dahil), sonra **Commit changes**'e bas.
   - `.github` klasörü gizli göründüğü için yüklenmezse: **Add file → Create new file**'a bas, dosya adına `.github/workflows/build-apk.yml` yaz ve bu dosyanın içeriğini yapıştır.
3. **Actions** sekmesine geç; "APK oluştur" işi 3-5 dakikada yeşil olur.
4. İşe tıkla, en alttaki **Artifacts** bölümünden `Antrenmanim-apk` dosyasını indir, zip'i aç, içindeki `.apk`'yı telefonuna at ve kur
   (telefon "bilinmeyen kaynaklar" izni isterse bu dosya için izin ver).

## Android Studio ile
Klasörü **File → Open** ile aç, senkronizasyon bitince **Build → Build App Bundle(s) / APK(s) → Build APK(s)**.

## Arayüzü değiştirmek
Tüm ekranlar `app/src/main/assets/index.html` dosyasında.

## Hazır program
İlk açılışta 3 günlük program (Pazartesi, Çarşamba, Cuma) GIF'leriyle birlikte yüklenir; tüm hareketler 3 set × 8 tekrar × 60 kg olarak gelir, **✏️ Düzenle** ile değiştirebilirsin.
GIF'ler `app/src/main/assets/gifs/` klasöründe, program ise `index.html` içindeki `DEFAULT_PROGRAM` bölümünde.
