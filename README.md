# Erkenaz
Қазақ әдеби мұрасын цифрландыру
<!DOCTYPE html><html lang="kk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Қазақ әдеби мұрасын цифрландыру</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f5f5f5;
    }
    header {
      background: #2c3e50;
      color: white;
      padding: 15px;
      text-align: center;
    }
    nav {
      background: #34495e;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
      font-weight: bold;
    }
    .container {
      padding: 20px;
    }
    .card {
      background: white;
      padding: 15px;
      margin-bottom: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    footer {
      background: #2c3e50;
      color: white;
      text-align: center;
      padding: 10px;
    }
    input {
      padding: 10px;
      width: 100%;
      margin-bottom: 15px;
    }
  </style>
</head>
<body><header>
  <h1>Қазақ әдеби мұрасын цифрландыру</h1>
  <p>Ұлттық әдебиетті сақтау және дамыту</p>
</header><nav>
  <a href="#">Басты бет</a>
  <a href="#">Шығармалар</a>
  <a href="#">Авторлар</a>
  <a href="#">Байланыс</a>
</nav><div class="container">
  <input type="text" id="search" placeholder="Шығарманы іздеу..." onkeyup="searchFunction()">  <div class="card">
    <h2>Абай Құнанбайұлы</h2>
    <p>Қара сөздер жинағы</p>
  </div>  <div class="card">
    <h2>Мұхтар Әуезов</h2>
    <p>Абай жолы романы</p>
  </div>  <div class="card">
    <h2>Ілияс Жансүгіров</h2>
    <p>Құлагер поэмасы</p>
  </div>
</div><footer>
  <p>© 2026 Қазақ әдеби мұрасы</p>
</footer><script>
function searchFunction() {
  let input = document.getElementById('search');
  let filter = input.value.toLowerCase();
  let cards = document.getElementsByClassName('card');

  for (let i = 0; i < cards.length; i++) {
    let text = cards[i].innerText.toLowerCase();
    if (text.includes(filter)) {
      cards[i].style.display = "block";
    } else {
      cards[i].style.display = "none";
    }
  }
}
</script></body>
</html>
