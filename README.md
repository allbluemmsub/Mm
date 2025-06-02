<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AllBlue MMSub</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      margin: 0;
      padding: 20px;
    }

    h1 {
      text-align: center;
    }

    .search-bar, .category-bar {
      text-align: center;
      margin: 10px 0;
    }

    .search-bar input {
      padding: 8px;
      width: 80%;
      max-width: 400px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .card {
      background: #fff;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    .card img {
      width: 100%;
      border-radius: 10px;
    }

    .card h2 {
      font-size: 18px;
      margin: 10px 0 5px;
    }

    .card p {
      font-size: 14px;
      color: #555;
    }

    .card a {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 15px;
      background: #007bff;
      color: #fff;
      border-radius: 5px;
      text-decoration: none;
    }

    .card a:hover {
      background: #0056b3;
    }

    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <h1>

  <div class="search-bar">
    <input type="text" id="searchInput" placeholder=" ကားနာမည်ရှာရန်..." onkeyup="filterMovies()" />
  </div>

  <div class="grid" id="movieGrid">

    <!-- POST 1 -->
    <div class="card" data-title="IPX-310" data-category="school">
      <img src="IMG_20250603_000159_189.jpg" alt="IPX-310" />
      <h2>အရမ်းကြည့်ကောင်းတယ်ကျောင်းသားကားလေးပါ</h2>
      <a href="https://megaup.net/xxxxxx" target="_blank">Download</a>
    </div>

    <!-- POST 2 -->
    <div class="card" data-title="IPX-222" data-category="nurse">
      <img src="IMG_20250603_000208_434.jpg" alt="IPX-222" />
      <h2>သူနာပြုလေးအရမ်းမိုက်</h2>
      <a href="https://megaup.net/yyyyyy" target="_blank">Download</a>
    </div>

    <!-- POST 3 -->
    <div class="card" data-title="IPX-999" data-category="teacher">
      <img src="IMG_20250603_000212_622.jpg" alt="IPX-999" />
      <h2>ဆရာမကားကောင်းလေး</h2>
      <a href="https://megaup.net/zzzzzz" target="_blank">Download</a>
    </div>

    <!-- POST 4 -->
    <div class="card" data-title="IPX-999" data-category="teacher">
      <img src="IMG_20250603_000159_189.jpg" alt="IPX-999" />
      <h2>စာရင်းကိုင်မလေး</h2>
      <a href="https://megaup.net/zzzzzz" target="_blank">Download</a>
      </div>

  <script>
    function filterMovies() {
      const input = document.getElementById("searchInput").value.toLowerCase();
      const selectedCategory = document.getElementById("categorySelect").value;
      const cards = document.querySelectorAll(".card");

      cards.forEach(card => {
        const title = card.dataset.title.toLowerCase();
        const category = card.dataset.category;

        const matchesSearch = title.includes(input);
        const matchesCategory = (selectedCategory === "all" || selectedCategory === category);

        if (matchesSearch && matchesCategory) {
          card.classList.remove("hidden");
        } else {
          card.classList.add("hidden");
        }
      });
    }
  </script>
