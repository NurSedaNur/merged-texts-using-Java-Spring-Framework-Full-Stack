# merged-texts-using-Java-Spring-Framework-Full-Stack
 merged-texts-using-Java-Spring-Framework-Full-Stack
 
 Projeye ait detaylı bilgiye Rapor(1).pdf dosyasından ulaşabilirsiniz.


 • Giriş
Bu projede, kitap, dergi vb. gibi metinlerden elde edilen cümleler/kelimeler arasındaki
benzerlik, frekans gibi özelliklerin bulunması, metinlerin birleştirip birleştirilmeyeceğine
karar verilmesi ve elde edilen verilerden karakter tabanlı cümlelerin/kelimelerin
birleştirilmesi beklenmektedir. Bu işlemlerin yapılması için gerekli algoritma geliştirilmiştir.Amaç: Bu projede iki veya daha fazla metnin uygun bir şekilde birleştirilmesi problemi
için yeni algoritmalar geliştirmek amaçlanmaktadır. Devamında bunları görsel bir
arayüzle sunmanız beklenmektedir. Geliştirdiğiniz algoritmanın performans
özelliklerini ve çalışma sürelerini farklı girdilerde karşılaştırmalısınız.

. İsterler
Geliştirilen web arayüzünde en az iki adet metin gitmeniz gerekmektedir. Bunun için:
● En az iki tane metin giriş butonları bulunmalıdır. (Metin Ekle)
● Girilen metinleri birleştirme butonu bulunmalıdır. (Metinleri Birleştir)
● Girilen metinleri kaydetme (.json formatında) butonu (Birleşik Metni Kaydet)
● Veriden elde edilen en uzun dizi listelerinin tümü bir liste halinde kaydedilmeli
● İki metni birleştirmek işlemi için geçen süre hesaplanmalıdır.

Görsel arayüzde iki adet metin giriş etiketi ve bu etiketlere ait “ekle” , “birleştir” ve “kaydet”
butonları bulunmalıdır. 

2. Başlangıç
Öncelikle https://start.spring.io/ adresinden bir spring projesi temeli oluşturduk. Dili java seçtik ve kullanmak istediğimiz dependencies leri ekledik ( lombok – mongodb – Spring Boot devtools – Spring web – Thymeleaf).
  İndirdiğimiz projeyi eclipse uygulamasında açtık . Algoritma kısmını oluşturmak için model paketinin altında book adlı bir klas oluşturduk ve web arayüzünden alıcak kelimleri ve süreyi tanımladık
![image](https://user-images.githubusercontent.com/115660565/235446126-a6d2abc6-98b5-4509-9a35-b43d1551b2a0.png)
Arayüz kısmı için  templates klasörü altında iki tane html uzantılı dosya oluşturduk. İlk ekranda kullanıcıdan alınacak kelimeler için text boxlar oluşturduk ve birleşme algoritmasına gitmesi için birleştir butonu tanımladık. Arka kısımda ise bir controller classı açıp verileri alıp ikinci ekrana dönmesi için bir method yazdık. İkinci ekranda ise birleştirme kodundan dönen birleşmiş kelime için bir text book ve algoritmanın Süresi için  bir text book oluşturduk. Ayrıca bir kaydet butonu koyduk. Bu buton verileri mongodb ye kaydetmekte.Arka planda ise controoler classında save işlemi için methodunu tanımladık.

Ara yüzde iyileştirme yapmak için ise bootstrap  ve css den yardım aldık.
![image](https://user-images.githubusercontent.com/115660565/235446233-7bf646ef-0f36-4e5b-afc6-f68d9e4a90d1.png)

![image](https://user-images.githubusercontent.com/115660565/235446246-b94569f9-d11a-42fe-9e55-b30568ed14e3.png)

![image](https://user-images.githubusercontent.com/115660565/235446290-d41804e0-2e0c-47e8-ad22-c9856037a15a.png)
