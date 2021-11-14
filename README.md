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
  
   **Not: Her şey bir paket olduğu için aslında import ettiğimiz her şey burada oluşturduğumuz modüller gibidir..**
   
   <h5>Modül yapısı oluşturma algoritma şeklinde anlatım: </h5>
    <ol>
      <li> klasör oluştur. </li>
      <li> klasör içerisine örnek bir dosya oluştur. (örnek: "module1.go) </li>
      <li> terminale `go mod init <modül ismi>` yazıp enter tuşuna basıyoruz. </li>
      <li> main.go içerisine `ìmport <modül ismi>/<modüllerin bulunduğu klasör ismi>` örnek: golesson/testmodules </li>
      <li> ve artık klasör içerisinde bulunan go dosyalarımızı yani kendi yazdığımız modülleri main.go içerisinde kullanabiliyoruz. </li>
    </ol>
