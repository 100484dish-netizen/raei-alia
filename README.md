# raei-alia<!DOCTYPE html><html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>راعي العليا</title>
  <style>
    body {
      margin: 0;
      font-family: 'Tahoma', sans-serif;
      background: linear-gradient(135deg, #1e1e2f, #2c2c54);
      color: #fff;
    }header {
  background: rgba(0,0,0,0.6);
  padding: 20px;
  text-align: center;
  font-size: 28px;
  font-weight: bold;
  letter-spacing: 2px;
  border-bottom: 2px solid gold;
}

nav {
  display: flex;
  justify-content: center;
  gap: 15px;
  padding: 15px;
}

nav button {
  background: gold;
  border: none;
  padding: 10px 20px;
  border-radius: 25px;
  cursor: pointer;
  font-weight: bold;
  transition: 0.3s;
}

nav button:hover {
  background: orange;
  transform: scale(1.1);
}

.container {
  padding: 20px;
  max-width: 900px;
  margin: auto;
}

.card {
  background: rgba(255,255,255,0.05);
  padding: 20px;
  margin-bottom: 20px;
  border-radius: 15px;
  box-shadow: 0 0 10px rgba(0,0,0,0.5);
}

textarea {
  width: 100%;
  height: 120px;
  border-radius: 10px;
  border: none;
  padding: 10px;
  font-size: 16px;
}

.publish {
  margin-top: 10px;
  background: gold;
  border: none;
  padding: 10px;
  border-radius: 10px;
  cursor: pointer;
  font-weight: bold;
}

footer {
  text-align: center;
  padding: 15px;
  background: rgba(0,0,0,0.5);
  border-top: 1px solid gold;
}

  </style>
</head>
<body><header>راعي العليا</header><nav>
  <button onclick="showSection('home')">الرئيسية</button>
  <button onclick="showSection('write')">اكتب قصتك</button>
  <button onclick="showSection('stories')">القصص</button>
</nav><div class="container">  <div id="home" class="card">
    <h2>مرحبا بك في راعي العليا</h2>
    <p>موقع تاريخي لنشر القصص والروايات بأسلوب عربي فصيح. هنا تكتب، وتشارك، وتبني اسمك.</p>
  </div>  <div id="write" class="card" style="display:none;">
    <h2>اكتب قصتك</h2>
    <textarea id="storyInput" placeholder="اكتب قصتك هنا..."></textarea>
    <button class="publish" onclick="publishStory()">نشر</button>
  </div>  <div id="stories" class="card" style="display:none;">
    <h2>القصص المنشورة</h2>
    <div id="storiesList"></div>
  </div></div><footer>
  جميع الحقوق محفوظة - راعي العليا
</footer><script>
  function showSection(section) {
    document.getElementById('home').style.display = 'none';
    document.getElementById('
