  <h1>Notes ✏</h1>
  <h3> 'package' nedir? </h3>
  
  <p>
    Go dilinde kod organizasyonu paketler ile sağlanır. 
    hem kod içerisinde kullandığımız kütüphaneler hem de ana kodumuz aslında birer pakettir.
  </p>
  
  <h3>Veri tipleri:</h3>
  
  <p>
  ```go 
    var yazi string = "Hello World!"
    var sayi int = 12345
    var ondaliklisayi float32 = 0.5 //float64'de olabilirdi fakat sadece boyut değişmekte.
    var durum bool = false //yada true" bir durum belirtir.
    bilinmeyen := 1 //burda hangi değeri verirseniz verin go tahmin yürütüp otomatik atama yapacaktır. 
  ```
  **Not**: go kullanmadığımız hiç bir yapıyı barındırmaz!<br>
  **string format**: `fmt.printf("veri türü: %T", bilinmeyen) //bize bilinmeyen değişkeninin veri tipini verir "%T"`
  </p>
  
  <h4>Örnek modül yapısı:</h4>
  <p>
    öncelikle bir modül dosyamızı ve klasörümüzü oluşturalım.
    bir tane "testmodules" diye bir klasör oluşturalım ve bunun içerisinede "module1.go" dosyamızı oluşturalım.
    daha sonra ise "module1.go" isimli modülümüzü kullanabilmek için terminale `go mod init examplemodule` yazıp enter tuşuna basıyoruz..
    modülümüz oluşturulduktan sonra "go.mod" adında bir dosya gelecek buranın içerisinde "go"muzun sürümü ve oluşturduğumuz modülümüzün ismi bulunmaktadır.
    ve dosyalarımızı oluşturduk gerekli işlemlerimizi yaptığımıza göre modülü kullanmak için dosya içerisine dahil edelim. bunun için ise "import" anahtar kelimesini         kullanıyoruz örnek: `import "examplemodule/testmodules"` artık "testmodules" klasörümüzün içerisindeki tüm modülleri kullanabiliyoruz.. 
  </p>
