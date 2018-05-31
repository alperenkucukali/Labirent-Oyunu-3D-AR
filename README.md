# Labirent 3D AR Game
## Labirent 3D AR Game Nedir?
*Unity tabanlı , arttırılmış gerçeklik kullanılarak tasarlanmış üç boyutlu bir mobil oyundur. Dumlupınar Üniversitesi Bilgisayar Mühendisliği bölümü sayın Dr. Öğr. Üyesi Muammer AKÇAY 'a Yazılım Mühendisliği dersi projesi olarak sunulmuştur.*
## Labirent 3D AR Game Nasıl Oluşturuldu ?
*Unity , Android Studio , JDK , Visual Studio gibi gerekli program ve uygulamaları bilgisayarımıza kuruyoruz. Arttırılmış gerçeklik kütüphanesi olan Vuforia ‘dan sistemimize uyumlu kütüphaneyi indirip Unity ‘ye import ediyoruz.*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(1).png?raw=true)
</br></br>
*İmport işlemi bittikten sonra Vuforia kütüphanesini kullanabilmek için Lisans Şifresi satın almamız gerekiyor. Vuforia internet sitesinden aldığımız şifreyi Vuforia ‘da gerekli yere yazıyoruz.*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(2).png?raw=true)
</br><br>
*Vuforia Sitesine giderek hedef resmimizi Vuforia veri tabanına Target Manager sekmesinden ekliyoruz. Ardından eklediğimiz veriyi bilgisayara tekrar site üzerinden indiriyoruz. İndirmiş olduğumuz veriyi Unity projemize import ediyoruz.*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(3).png?raw=true)
</br><br>
*Oluşturduğumuz resmin üzerine 3D küpler kullanarak resmimizi 3 boyutlu hale getiriyoruz. Bu küplere Box Collider tanımlıyoruz ve bu sayede labirent içine yerleştireceğimiz topumuz nesnelerin içinden geçemeyecektir.*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(4).png?raw=true)
</br><br>
*Küpler tamamlandıktan sonra labirentimizin ortasına küplerin arasına sığacak boyutta bir Top (Sphere) tanımlıyoruz. Topa da Rigidbody tanımlıyoruz ki küplerin içinden geçemesin. Topun hareket edebilmesi için yerçekimi tanımlıyoruz.*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(5).png?raw=true)
</br><br>
*Topa bir spawnPoint(doğma noktası) tanımlıyoruz ki eğer topumuz labirentimizin dışına çıkarsa veya oyun başlarken nerde duracağını belirlememiz gerekiyor. Eğer topumuz labirentin Y ekseninden 10cm uzaklaşırsa topumuz tekrar doğma noktasına dönecektir.*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(6).png?raw=true)
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(7).png?raw=true)
</br><br>
*Oyunumuzun bilgisayar üzerinde kontrollerini sağladıktan sonra android için uyumla hale getiriyoruz . Unity’e Android Studio (SDK) ve JDK nın dosya yolunu gösteriyoruz. File > Build Settings > Player Settings yaparak android için icon , telefon görünümü , oyunun adı gibi değişiklikleri yapıyoruz ve build ediyoruz.*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/Ekran%20G%C3%B6r%C3%BCnt%C3%BCs%C3%BC%20(8).png?raw=true)
</br><br>
*Oluşan .apk dosyasını android cihazımıza atarak oyunu çalıştırıyor ve eğlenmeye başlıyoruz .*
</br>
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/ss%20(1).png?raw=true)
![](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/ss%20(2).png?raw=true)
</br><br><br>
*Oyunun .apk doysasına* [buradan](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/LabirentAG.apk) *ulaşabilirsiniz.*
<br>
*Oyunu oynayabilmek için kameraya göstermeniz gereken resmi* [buradan](https://github.com/alperenkucukali/Labirent-Oyunu-3D-AR/blob/master/LabirentOyunuProje/Kullan%C4%B1lanResimler/F16WBMDIQ6VC5V2.MEDIUM.jpg) *indirebilirsiniz.*

`Alperen Küçükali`
