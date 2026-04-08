# mathgot-home
موقع مطعم مذغوط منزلنا
<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>مذغوط منزلنا</title>

<style>
body {
  font-family: Arial;
  direction: rtl;
  text-align: center;
  background: #fdf6f0;
}

.header {
  background: #8e3b1f;
  color: white;
  padding: 20px;
  border-radius: 0 0 20px 20px;
}

.container {
  background: white;
  padding: 20px;
  margin: 20px;
  border-radius: 15px;
  box-shadow: 0 0 10px #ddd;
}

button {
  padding: 12px 25px;
  background: #d35400;
  color: white;
  border: none;
  border-radius: 8px;
  font-size: 16px;
}

input, textarea {
  width: 80%;
  padding: 10px;
  margin: 5px;
  border-radius: 8px;
  border: 1px solid #ccc;
}
</style>

</head>

<body>

<div class="header">
<h1>🍽️ مذغوط منزلنا</h1>
<p>الطعم البيتي الأصيل ❤️ اطلب قبل توصل</p>
</div>

<div class="container">
<h2>📋 المنيو</h2>
<p>🍗 مذغوط دجاج - 25 ريال</p>
<p>🥩 مذغوط لحم - 35 ريال</p>
<p>🍚 رز إضافي - 5 ريال</p>
</div>

<div class="container">
<h2>📦 اطلب الآن</h2>

<input id="name" placeholder="اسمك"><br>
<input id="phone" placeholder="رقم الجوال"><br>
<textarea id="order" placeholder="اكتب طلبك"></textarea><br>

<button onclick="sendOrder()">إرسال الطلب عبر واتساب</button>
</div>

<script>
function sendOrder() {
  var name = document.getElementById("name").value;
  var phone = document.getElementById("phone").value;
  var order = document.getElementById("order").value;

  var message = "طلب جديد من مذغوط منزلنا:%0A"
              + "الاسم: " + name + "%0A"
              + "الجوال: " + phone + "%0A"
              + "الطلب: " + order;

  window.open("https://wa.me/966XXXXXXXXX?text=" + message);
}
</script>

</body>
</html>
