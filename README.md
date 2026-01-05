<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>متجر الأحذية</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <!-- ربط ملف CSS -->
  <link rel="stylesheet" href="style/style.css">
</head>
<body>
  <!-- رأس الصفحة -->/* إعدادات عامة */

body {
    font-family: "Segoe UI", Tahoma, sans-serif;
    margin: 0;
    background-color: #f5f5f5;
    direction: rtl;
}


/* رأس الصفحة */

header {
    background-color: #232f3e;
    color: white;
    padding: 15px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.5em;
    font-weight: bold;
}

.navbar ul {
    list-style: none;
    display: flex;
    gap: 20px;
    margin: 0;
    padding: 0;
}

.navbar ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

.navbar ul li a:hover {
    color: #ff9900;
}

.search-box {
    display: flex;
    gap: 5px;
}

.search-box input {
    padding: 8px;
    border-radius: 5px;
    border: none;
}

.search-box button {
    background-color: #ff9900;
    border: none;
    padding: 8px 12px;
    border-radius: 5px;
    cursor: pointer;
}

.search-box button:hover {
    background-color: #e68a00;
}


/* المنتجات */

.products {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    margin: 20px;
}

.product {
    background: white;
    padding: 15px;
    border-radius: 8px;
    text-align: center;
    width: 220px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s;
}

.product:hover {
    transform: translateY(-5px);
}

.product img {
    width: 100%;
    height: auto;
    border-radius: 5px;
}

.price {
    font-size: 1.2em;
    color: #232f3e;
    font-weight: bold;
}

.add-to-cart {
    background-color: #ff9900;
    border: none;
    padding: 10px;
    margin-top: 10px;
    cursor: pointer;
    border-radius: 5px;
    width: 100%;
}

.add-to-cart:hover {
    background-color: #e68a00;
}


/* الفوتر */

footer {
    background-color: #232f3e;
    color: white;
    text-align: center;
    padding: 10px;
}


/* Responsive Design */

@media (max-width: 768px) {
    header {
        flex-direction: column;
        align-items: flex-start;
    }
    .navbar ul {
        flex-direction: column;
        gap: 10px;
    }
    .products {
        flex-direction: column;
        align-items: center;
    }
}
  <header>
    <div class="logo">🥿 متجر الأحذية</div>
    <nav class="navbar">
      <ul>
        <li><a href="#">الرئيسية</a></li>
        <li><a href="#">العروض</a></li>
        <li><a href="#">السلة 🛒 <span id="cart-count">0</span></a></li>
        <li><a href="#">حسابي</a></li>
      </ul>
    </nav>
    <div class="search-box">
      <input type="text" placeholder="ابحث عن حذاء...">
      <button>بحث</button>
    </div>
  </header>

  <!-- المنتجات -->
  <main class="products">
    <div class="product">
      <img src="images/shoe1.jpg" alt="حذاء رياضي">
      <h2>حذاء رياضي</h2>
      <p class="price">500 جنيه</p>
      <button class="add-to-cart">أضف للسلة</button>
    </div>

    <div class="product">
      <img src="images/shoe2.jpg" alt="حذاء كلاسيك">
      <h2>حذاء كلاسيك</h2>
      <p class="price">700 جنيه</p>
      <button class="add-to-cart">أضف للسلة</button>
    </div>
  </main>

  <!-- الفوتر -->
  <footer>
    <p>© 2026 متجر الأحذية - جميع الحقوق محفوظة</p>
  </footer>

  <!-- ربط ملف JS -->
  <script src="js/script.js"></script>
</body>
</html>
