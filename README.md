# İntime Project Studio

Beş projeli, gerçek WebGL geometrileriyle çalışan 3D proje vitrini. Three.js 0.180.0 proje içine alınmıştır.

## Dosya yapısı

- `index.html`: sayfa yapısı, menü ve iletişim bağlantısı.
- `css/style.css`: masaüstü ve mobil düzen, sahneler, hareket azaltma desteği.
- `js/app.js`: beş projenin içerikleri, kaydırma zaman çizelgesi, proje detayları ve görsel karşılaştırma.
- `js/world.js`: gerçek 3D banko geometrileri, ayrılıp birleşen parçalar, ışıklar, gölgeler ve fotoğraf düzlemlerine geçişler.
- `js/vendor/`: yerel Three.js modülleri ve MIT lisansı.
- `assets/`: gönderilen görsellerin asılları ve hafif WebP kopyaları.
- `server.cjs`: yalnızca bilgisayarda yerel önizleme sunucusu.

## Açma

Bu sürüm ES modülleri kullanır, dosyayı çift tıklayarak açmak yerine yerel HTTP sunucusuyla açın. Bu klasörde `node server.cjs` çalıştırıp http://127.0.0.1:4173 adresine gidin.

## Düzenleme

Proje isimlerini, açıklamalarını, görsellerini ve renklerini `js/app.js` dosyasının başındaki `projects` listesinden değiştirebilirsiniz. Beş proje başlığı geçici seçimdir. Coffee & More görselleri doğrulanmış tasarım/uygulama bilgisi olmadığı için Görünüm 01 ve Görünüm 02 olarak etiketlendi. İletişim bağlantısı mevcut İntime sitesini açar.

## 3D yolculuk

1. Açılışta bankonun tabanı, cephe çıtaları, taş tezgâhı, cam vitrini, ekipmanı ve lambaları ayrı durur.
2. Kaydırınca parçalar birleşir.
3. Her projede banko farklı bir açıya döner; yan yüzeyler ve raf derinliği gerçek geometrilerle görünür.
4. Proje fotoğrafı 3D bir düzlem olarak kadraja girer ve ekranı kaplar.
5. Fotoğraf uzaklaşarak sonraki banko sahnesine geçer.

Mobilde dikey kaydırma yolculuğu ilerletir, bankonun üstünde yatay parmak hareketi bankoyu döndürür. Görsellerden malzeme dokuları çıkarılmıştır. Bankolar kaynak görselleri referans alan stilize, yeniden oluşturulmuş modellerdir; özgün ölçülü CAD modelleri veya fotogerçekçi birebir dijital kopyalar değildir. Gerçek 3D mekânın içine girilen bir tur kullanılmaz.

Hareket azaltma tercihi açıkken birleşme ve dönüş yerine sabit açılar ve doğrudan geçişler gösterilir. WebGL açılamazsa görselli alternatif ve menüden açılan proje detayları kullanılır. Yazı tipleri internet varsa Google Fonts üzerinden yüklenir; çevrimdışı sistem yazı tipleri kullanılır. Site yayınlanmadı.
