<img width="1280" height="854" alt="لوغو PNG" src="https://github.com/user-attachments/assets/4d686d27-ec18-447a-bbe2-2b2f294a939e" />
<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>معرض الشركة</title>
  <style>
    body {
      font-family: Arial;
      direction: rtl;
      text-align: center;
      background: #f5f5f5;
      margin: 0;
      padding: 20px;
    }

    .header {
      margin-bottom: 20px;
    }

    .company {
      font-size: 28px;
      font-weight: bold;
    }

    .whatsapp {
      margin-top: 10px;
    }

    .whatsapp a {
      background: #25D366;
      color: white;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 8px;
      display: inline-block;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      margin-top: 20px;
    }

    .gallery img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
    }

    input {
      margin: 5px;
      padding: 8px;
      width: 250px;
    }
  </style>
</head>

<body>

  <div class="header">
    <input type="text" id="companyName" placeholder="اسم الشركة">
    <br>
    <input type="text" id="whatsappNumber" placeholder="رقم الواتساب (مثال: 905xxxxxxxxx)">
    <br><br>
    <input type="file" id="images" multiple accept="image/*">
  </div>

  <div class="company" id="title">اسم الشركة</div>

  <div class="whatsapp" id="wa"></div>

  <div class="gallery" id="gallery"></div>

  <script>
    const imagesInput = document.getElementById("images");
    const gallery = document.getElementById("gallery");
    const title = document.getElementById("title");
    const wa = document.getElementById("wa");

    document.getElementById("companyName").addEventListener("input", function() {
      title.innerText = this.value || "اسم الشركة";
    });

    document.getElementById("whatsappNumber").addEventListener("input", function() {
      if (this.value) {
        wa.innerHTML = `<a href="https://wa.me/${this.value}" target="_blank">تواصل واتساب</a>`;
      }
    });

    imagesInput.addEventListener("change", function() {
      gallery.innerHTML = "";
      const files = Array.from(this.files).slice(0, 12);

      files.forEach(file => {
        const reader = new FileReader();
        reader.onload = function(e) {
          const img = document.createElement("img");
          img.src = e.target.result;
          gallery.appendChild(img);
        }
        reader.readAsDataURL(file);
      });
    });
  </script>

</body>
</html>
<img src="logo.png" width="150"> <img width="1280" height="854" alt="لوغو PNG" src="https://github.com/user-attachments/assets/e3f44656-1bc8-4064-9dbb-b701c3e0251c" />
