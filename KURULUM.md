# Slider Dialer: telefondan APK alma rehberi

Bilgisayar gerekmez. GitHub'ın ücretsiz bulut derlemesi APK'yı sizin için üretir.

## 1. GitHub hesabı
github.com adresinden ücretsiz hesap açın (zaten varsa giriş yapın).

## 2. Depo (repository) oluşturun
- Sağ üstteki + işareti, ardından New repository
- Repository name: SliderDialer
- Public seçili olsun
- Create repository

## 3. Dosyaları ekleyin
Depo sayfasında "creating a new file" bağlantısına dokunun. Üstteki dosya adı kutusuna aşağıdaki yolu aynen yazın (/ işareti klasör açar), içeriği alttaki büyük kutuya yapıştırın ve Commit changes, sonra yine Commit changes diyerek kaydedin.

Eklenecek 10 dosya (adlar tam böyle olmalı):

1. settings.gradle.kts
2. build.gradle.kts
3. gradle.properties
4. app/build.gradle.kts
5. app/src/main/AndroidManifest.xml
6. app/src/main/kotlin/com/example/sliderdialer/MainActivity.kt
7. app/src/main/kotlin/com/example/sliderdialer/CallManager.kt
8. app/src/main/kotlin/com/example/sliderdialer/CallService.kt
9. app/src/main/kotlin/com/example/sliderdialer/CallActivity.kt
10. .github/workflows/build.yml  (başında nokta var, nokta unutulmasın)

Her dosyanın içeriği size ayrı dosya olarak gönderildi. Dosyayı açıp tüm metni kopyalayın.

Daha önce ilk 7 dosyayı eklediyseniz: AndroidManifest.xml ve MainActivity.kt dosyalarının içeriğini yenisiyle değiştirin (dosyayı açın, kalem simgesine dokunun, tüm metni silip yenisini yapıştırın), CallManager.kt, CallService.kt ve CallActivity.kt dosyalarını yeni dosya olarak ekleyin.

## 4. APK'nın derlenmesini bekleyin
- Depoda Actions sekmesine girin
- "Build APK" çalışıyor olmalı, 3-5 dakika sürer
- Yeşil tik çıkınca o çalışmaya dokunun
- En altta Artifacts bölümünde SliderDialer-apk dosyasını indirin

Kırmızı çarpı çıkarsa o çalışmaya dokunup hata metnini bana gönderin.

## 5. Kurulum
- İnen dosya zip'tir, dosya yöneticisinden açıp app-debug.apk'ya dokunun
- Telefon "bilinmeyen kaynaklardan yükleme" izni isterse Ayarlar'dan bu tarayıcı veya dosya yöneticisi için izin verin
- Kurulduktan sonra uygulama "Slider Dialer" adıyla görünür

## Arama ekranını etkinleştirme
Arama ekranı (gelen ve giden aramada cevapla, reddet, bitir, sessiz, hoparlör) yalnızca uygulama telefonun varsayılan arama uygulaması olursa çalışır.

1. Uygulamayı açın, "Varsayılan arama uygulaması yap" düğmesine dokunun
2. Çıkan pencerede Slider Dialer'ı seçip onaylayın
3. Bildirim ve arama izinlerini verin

Varsayılan yaptıktan sonra yaptığınız ve aldığınız aramalar bu uygulamanın ekranıyla yönetilir.

Geri dönmek için: Ayarlar, Uygulamalar, Varsayılan uygulamalar, Telefon uygulaması (telefon markasına göre adı biraz değişir) yolundan eski arama uygulamanızı seçin.

Önemli: Acil aramalar (112) dahil tüm aramalar bu ekrandan geçer. Uygulama ilk kez denendiği için, güvenli tarafta kalmak adına denemeyi ikinci bir telefon varken yapın ve çalıştığından emin olmadan günlük kullanım telefonunuzda varsayılan yapmayın.

## Kullanım
- Tuş takımı veya Slider ile numara modu arasında üstteki düğmeyle geçin
- Alttaki çubuğu sağa kaydırınca arama başlar. Varsayılan arama uygulamasıysa kendi arama ekranı açılır, değilse telefonun arama ekranı numarayla açılır
- Sola kaydırınca mesaj uygulaması açılır
