# Metin2-Balik-Botu
Metin2 ve Özel Sunucu için basit bir Javascript Balik Botu, Pixel aramayla çalışır. Bu botu kullanabilmek için bilgisayarınızda NodeJs'nin yüklü olması gerekiyor. Eğer yüklü değil ise buradan indirebilirsiniz: [NodeJS](https://nodejs.org/en/download)

CMD'yi yani Konsol Uygulamasını çalıştırın ve ardından aşağıdaki yönergeleri takip edin.

Bağımlılıkları yüklemek için:

```markdown
npm install
```

# Kullanım
1. Metin'i pencere modunda kurun.
2. Çözünürlüğü 1920x1080 olarak ayarlayın.
3. Pencereyi ekranın sol üst köşesine yerleştirin.
4. Oltayı donatın
5. Yemleri düğmelere yerleştirin: 1, 2, 3 eşit bölünmüş örneğin: 200, 200, 200
6. Komut dosyasını çalıştırın.

# Bilgi
Bu komut dosyası belirli konumlardaki pikselleri kontrol ederek çalışır. ZorinOS with Wine'da çalışacak şekilde yapılandırılmıştır; bu, ayarların Windows'ta farklı olabileceği anlamına gelir. Aşağıdaki değişkenleri özelleştirmeniz gerekebilir:

FishingBox: Olta kutusunun konumu. Balık tutma kutusunun 1 piksellik siyah (#000000) bir sınırı vardır ve bu, kullanıcının o anda balık tutmakta olup olmadığını belirlemek için gereklidir.

FishingArea: Balık tutma alanını tanımlar (fishingArea + boxSize). Kare kullanıyoruz çünkü balık ancak dairenin içindeyken vurulabilir hale geliyor ve kenarı "kırmızıya" dönüşüyor.

CirclePos: Balık içerideyken renk değiştiren dairedir. KIRMIZI renge döndüğünde bot balığı yakalamaya çalışacaktır; aksi takdirde bekleyecektir.

# Komut Dosyasını Çalıştırma
```markdown
node index.js
```
