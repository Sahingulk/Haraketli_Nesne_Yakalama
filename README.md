<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
  
</head>
<body>

<h1>Hareket Algılama (Python & OpenCV)</h1>

<p>Bu Python kodu, bir kameradan canlı görüntü alır ve hareket algılamak için OpenCV kütüphanesini kullanır.</p>

<h2>Nasıl Çalışır?</h2>
<ol>
  <li><strong>Kamera Bağlantısı:</strong> Kod, varsayılan kamera cihazını kullanarak (<code>cv2.VideoCapture(0)</code>) kameraya bağlanır.</li>
  <li><strong>Hareket Algılama İşlemi:</strong>
    <ul>
      <li>Önceki ve mevcut kareler arasındaki farkı hesaplar.</li>
      <li>Fark karesi, bir eşik değeri üzerinde piksel farkları içeren bir ikili görüntüye dönüştürülür.</li>
      <li>Eşik değerini aşan pikseller, kontur bulma işlemi için kullanılır.</li>
      <li>Konturlar, belirli bir alan eşiğinden büyük olan hareketli nesneleri belirlemek için kullanılır.</li>
    </ul>
  </li>
  <li><strong>Hareket Tespiti ve Görselleştirme:</strong>
    <ul>
      <li>Hareket algılandığında, karenin üzerine sınırlayıcı kutular çizilir ve "Hareket var" mesajı konsola yazılır.</li>
      <li>Hareket algılanmazsa, "Durgun" mesajı konsola yazılır.</li>
    </ul>
  </li>
  <li><strong>Pencere Gösterimi:</strong> Kod, her kareyi işledikten sonra bir pencerede işlenmiş kareleri gösterir.</li>
  <li><strong>Çıkış:</strong> Kullanıcı "q" tuşuna basarak programı sonlandırabilir.</li>
</ol>

<h2>Gereksinimler:</h2>
<ul>
  <li>Python 3.x</li>
  <li>OpenCV kütüphanesi</li>
  <li>imutils kütüphanesi</li>
</ul>

<h2>Kullanım:</h2>
<ol>
  <li>Kodu çalıştırmak için Python ortamına sahip bir bilgisayarda çalıştırın.</li>
  <li>Bir kamera cihazını (varsayılan kamera genellikle "0" olarak belirtilir) bilgisayarınıza bağlayın.</li>
  <li>Kodu çalıştırın ve kameradan alınan canlı görüntüyü izleyin.</li>
</ol>

</body>
</html>
