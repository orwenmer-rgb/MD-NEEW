![Uploading Create_a_premium_A4_portrait_202606141213.jpeg…]()
<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>معرض الشركة</title>

  <style>
    body {
      font-family: Arial;
      direction: rtl;
      margin: 0;
      background: #f4f4f4;
      text-align: center;
    }

    header {
      background: #111;
      color: white;
      padding: 20px;
    }

    header img {
      width: 120px;
      border-radius: 10px;
      margin-bottom: 10px;
    }

    h1 {
      margin: 10px 0 0;
      font-size: 28px;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      padding: 20px;
    }

    .gallery img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
    }

    /* زر واتساب ثابت */
    .whatsapp {
      position: fixed;
      bottom: 20px;
      left: 20px;
      background: #25D366;
      color: white;
      padding: 15px 20px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    }

    .whatsapp:hover {
      background: #1ebe5d;
    }
  </style>
</head>

<body>

  <!-- الهيدر -->
  <header>
    <!-- شعار الشركة -->
    <img src="logo.png" alt="Logo">

    <!-- اسم الشركة -->
    <h1>اسم الشركة</h1>
  </header>

  <!-- معرض الصور -->
  <div class="gallery">

    <img src="img1.jpg">
    <img src="img2.jpg">
    <img src="img3.jpg">
    <img src="img4.jpg">
    <img src="img5.jpg">
    <img src="img6.jpg">
    <img src="img7.jpg">
    <img src="img8.jpg">
    <img src="img9.jpg">
    <img src="img10.jpg">
    <img src="img11.jpg">
    <img src="img12.jpg">

  </div>

  <!-- زر واتساب -->
  <a class="whatsapp" href="https://wa.me/905xxxxxxxxx" target="_blank">
    واتساب
  </a>

</body>
</html>
