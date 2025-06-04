<!DOCTYPE html>
<html lang="my">
<head>
  <meta charset="UTF-8">
  <title>MMSub Movies</title>
  <style>
    body {
      background-color: #000;
      color: #fff;
      font-family: Arial, sans-serif;
      padding: 20px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
    }
    .post {
      background-color: #1a1a1a;
      border-radius: 10px;
      overflow: hidden;
      text-align: center;
    }
    .post img {
      width: 100%;
      height: auto;
    }
    .post h2 {
      margin: 10px 0;
    }
    .post a {
      color: #ff4081;
      text-decoration: none;
    }
  </style>
</head>
<body>

  <h1>MMSub Movies</h1>
  <div class="grid">
    <div class="post">
      <a href="post1.html">
        <img src="IMG_20250603_000208_434.jpg" alt="Movie 1">
        <h2>go go မြန်မာ</h2>
      </a>
    </div>
    <div class="post">
      <a href="post2.html">
        <img src="IMG_20250603_000159_189.jpg" alt="Movie 2">
        <h2>myanmar မြန်မာ</h2>
      </a>
    </div>
    <!-- ထပ်မံသော post များကို ဒီနေရာတွင် ထည့်ပါ -->
  </div>

</body>
</html>
