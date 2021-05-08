Daha fazla bilgi için --> [Proje Raporu](https://github.com/mustafayigit34/flutter-mobilSorgular-YazLab/files/6412286/Rapor.pdf)

# Mobil Sorgular
Öncelikle ```pubspec.yaml``` dosyasında
<br> ```flutter pub get``` <br>
komutunu çalıştırmanız gerekmektedir. Aksi taktirde çalışmayacaktır.
Daha sonra ```"lib\main.dart"``` yolunu izleyerek <br> ```flutter emulators --launch "Your Emulator Name"``` <br> ile sanal cihazını çalıştırıp ardından <br> ```flutter run``` <br> komutuyla uygulamayı çalıştırabilirsiniz.
## Giriş
Bu projede Firebase Firestore üzerinden 
çeşitli sorgular yapılarak filtrelenmiş veriler alınmış, ardından bu veriler ile proje isterleri üç aşama halinde gerçeklenmiştir.
İlk aşamada veritabanı üzerinde bulunan 
verilerden istere uygun olan veriler getirilmiştir. İkinci aşamada ise kullanıcı uygulamaya daha çok dahil edilmiş ve kullanıcı 
tarafından seçilen başlangıç-bitiş tarihine, 
bölge adına göre istere cevap niteliğinde 
olan veriler ekranda saydırılarak sıralanmıştır. Üçüncü ve son aşamada ise projeye 
Google Maps ürünleri dahil olmuş ve kullanıcıdan alınan sınırlamalara göre üretilen 
sonuç harita üzerinde çizdirilerek kullanıcıya görsel bir sonuç sunulmuştur. Kullanıcıların tüm bu işlemleri yapabilmesi için 
bir mobil uygulama tasarlanmıştır.
