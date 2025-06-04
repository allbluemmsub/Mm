<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My JAV Sub Website</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      background: #f5f5f5;
    }
    h1 {
      text-align: block;
    }
    #searchBar {
      margin: 5px;
      display: right;
      padding: 10px;
      width: 40%;
      font-size: 16px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(50px, 2fr));
      gap: 20px;
      padding: 20px;
    }
    .card {
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      overflow: hidden;
      text-align: center;
      transition: 0.3s;
    }
    .card:hover {
      transform: scale(1.02);
    }
    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .card h3 {
      margin: 10px 0;
    }
    .card a {
      display: block;
      background: #007bff;
      color: white;
      text-decoration: none;
      padding: 10px;
      border-bottom-left-radius: 10px;
      border-bottom-right-radius: 10px;
    }
  </style>
</head>
<body>
  <img src="ads02.gif">
  <input type="text" id="searchBar" onkeyup="searchPosts()" placeholder="Search by title...">  <div class="grid" id="postGrid">
    <!-- Example Post -->
    <div class="card">
      <img src="IMG_20250603_000159_189.jpg">
      <h3>IPX-310
      <a href="post1.html">View Post</a>
      
    <div class="card">
      <img src="IMG_20250603_000159_189.jpg" alt="ABP-123">
      <h3>ABP-123
      <a href="post2.html">View Post</a>
      
  </div>  <script>
    function searchPosts() {
      const input = document.getElementById('searchBar').value.toLowerCase();
      const cards = document.querySelectorAll('.card');
      cards.forEach(card => {
        const title = card.querySelector('h3').textContent.toLowerCase();
        card.style.display = title.includes(input) ? 'block' : 'none';
      });
    }
  </script></body>
</html>
