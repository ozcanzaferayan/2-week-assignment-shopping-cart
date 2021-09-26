# Shopping Cart 
Alışveriş sitesi uygulaması oluşturmanız gerekiyor. Buradan örnek uygulamanın tasarımına ulaşabilirsiniz.
https://www.figma.com/file/9hO1ApoWscZXLEqrCkFEGI/2-week-assignment
Hazır data için db.json dosyasını kullanabilirsiniz. Bu dosyayı json-server ile ayağa kaldırıp API gibi kullanabilirsiniz.

## Sayfalar
1. Ana sayfa
    * Burada site ile ilgili gelen bir bilgi ve görsel yer alacaktır. Top Navbar dahildir.
2. Shop page
    * Üstteki Shop linkine tıklandığında açılacak sayfadır. Ürünler burada listelenecektir. 
    * soldaki checkbox menüsünden category bazında filtreleme yapılacaktır.
    * Sağdaki sort by dropdown'ında sıralama işlemi gerçekleştirilebilecektir.
        * popülerite (azalan), 
        * fiyat (artan)
        * fiyat (azalan)
3. Product page
    * Ürün detay bilgileri yer alacaktır.
    * Quantity alanı ile birlikte Add to Cart butonundaki değer hesaplanacaktır. Örn 2 item alacaksa fiyat x 2 şeklinde olacaktır.
    * Add to cart butonuna basıldığında eğer kullanıcı login değilse login olma ekranına yönlendirilecektir. 
    * Eğer kullanıcı loginse alışveriş sepetine eklenecektir ve üstteki alışveriş sepeti ikonundaki değer 1 arttırılacaktır.
4. Login page
    * Kullanıcının login işlemi gerçekleştirilecektir. 
    * User listesi için db.json içerisindeki /users endpoint'i kullanılabilir.
    * Eğer username ve password bilgisi uyuşuyorsa client side'da bir token oluşturulup localStorage'a yazılacaktır
    * Login olunduktan sonra, önceki sayfa hangisi ise ona yönlendirilecektir. Örneğin product sayfasından geldi diyelim, aynı ürünün sayfasına redirect edilecektir.
5. Cart page
    * Alışveriş sepei bilgileri yer alacaktır.
    * Alınan tüm ürünlerin fiyatı hesaplanıp görüntülenecektir.
    * Eklenen ürün Remove butonu ile sepetten çıkarılabilecektir.

## Notlar
* Proje içerisinde react-router-dom ve ant design eklenmiştir. Bu kütüphaneleri direkt olarak kullanabilirsiniz.