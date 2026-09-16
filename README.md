# Mobil UDF Editör ve PDF Dönüştürücü (Android APK Projesi)

Bu proje; UYAP Doküman Editörü (.udf) dosyalarını Android cihazlarda yerel olarak açıp düzenlemeye, biçimlendirmeye, tekrar .udf olarak kaydetmeye ve doğrudan A4 formatında .pdf üretmeye yarayan bağımsız bir Android uygulamasıdır.

## Yöntem 1: GitHub ile Sıfır Kurulumla Doğrudan APK Çıkarma (Önerilen - 3 Dakika)

Bilgisayarınıza Android Studio veya Java kurmadan, doğrudan GitHub'ın ücretsiz sunucularını kullanarak APK üretmek için:

1. [GitHub](https://github.com)'da ücretsiz bir hesap açın ve yeni bir boş depo (repository) oluşturun.
2. Bu ZIP paketinin içindeki tüm dosyaları deponuza yükleyin (Upload files / Commit).
3. GitHub, içindeki `.github/workflows/build_apk.yml` dosyasını otomatik olarak algılar ve **Actions** sekmesinde APK derleme işlemini başlatır.
4. Yaklaşık 2-3 dakika sonra işlem bittiğinde, **Actions** > son çalışma > **Artifacts** kısmından `app-debug.apk` dosyasını doğrudan telefonunuza indirip kurabilirsiniz!

## Yöntem 2: Kendi Bilgisayarınızda (Lokal) Derleme

Eğer bilgisayarınızda Node.js yüklüyse terminalden şu 3 komutu çalıştırarak Android Studio projesini açabilirsiniz:

```bash
npm install
npx cap add android
npx cap open android
```
Android Studio açıldığında **Build > Build Bundle(s) / APK(s) > Build APK(s)** demeniz yeterlidir.
