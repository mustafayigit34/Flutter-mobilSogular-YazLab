Daha fazla bilgi için --> [Proje Raporu](https://github.com/mustafayigit34/flutter-mobilSorgular-YazLab/files/6412286/Rapor.pdf)

# Mobil Sorgular
## Kurulum
Öncelikle ```pubspec.yaml``` dosyasında ```flutter pub get``` komutunu çalıştırmanız gerekmektedir. Aksi taktirde çalışmayacaktır.
Daha sonra ```"lib\main.dart"``` yolunu izleyerek ```flutter emulators --launch "Your Emulator Name"``` ile sanal cihazını çalıştırıp ardından ```flutter run``` komutuyla uygulamayı çalıştırabilirsiniz.
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

## Yöntem
Bu projede izlenilen yol aşağıda anlatılmıştır: <br>
Proje isterlerine geçmeden önce projede 
kullanılacak verilerin sayısının azaltılması 
ve bulut ortamına yüklenmesi işlemleri 
Python dili kullanılarak yapılmıştır. Daha 
sonra ise proje isterlerine geçilmiştir. Proje 
üç tip sorgu için üç aşama şeklinde 
tasarlanmıştır. <br>
Veriler https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page sitesinden alınıp birkaç düzenleme ile Firebase Firestore'a aktarılmıştır.
Dosya isimleri: <br>
```yellow tripdata 2020-12.csv``` <br>
``` taxi+ zone lookup.csv``` <br>
olup indirildikten sonraki düzenlemeler ile Firestore'da şu şekilde görülmektedir: <br>
![trips](https://user-images.githubusercontent.com/65903573/117537692-57da8680-b00b-11eb-9005-bd2d86916325.png)
![zones](https://user-images.githubusercontent.com/65903573/117537654-1944cc00-b00b-11eb-8704-9213d2e70b1c.png) <br>
                      trips                                          zones
Belge (collection9 isimleri sırasıyla "trips" ve "zones" olmalıdır.
