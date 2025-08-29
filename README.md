[index.html](https://github.com/user-attachments/files/22048942/index.html)
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>⚰️ Тёмный Ритуал Призыва Шаурмы</title>
  <style>
   body {
  background: linear-gradient(180deg, #000000, #1a001a);
  color: #c400ff;
  font-family: 'Courier New', monospace;
  text-align: center;
  padding: 40px;
}

    h1 {
      font-size: 3em;
      text-shadow: 0 0 15px #ff00ff, 0 0 30px #6600ff;
    }
    .pentagram {
      font-size: 4em;
      margin: 20px 0;
      color: #ff1a1a;
      text-shadow: 0 0 20px red, 0 0 40px black;
    }
    button {
      background: #660066;
      color: white;
      border: 2px solid #ff1aef;
      padding: 15px 30px;
      border-radius: 8px;
      font-size: 1.2em;
      cursor: pointer;
      transition: 0.3s;
      margin-top: 20px;
      box-shadow: 0 0 20px #9900ff;
    }
    button:hover {
      background: #990099;
    }
    #ingredients, #fixed {
      margin-top: 30px;
      font-size: 1.3em;
      line-height: 1.8em;
      text-shadow: 0 0 10px #ff33ff;
    }
    .section-title {
      font-size: 2em;
      margin-top: 40px;
      text-shadow: 0 0 10px red;
    }
  </style>
</head>
<body>
  <h1>🥙 Тёмный Ритуал Призыва Шаурмы ⚰️</h1>
  <div class="pentagram">✞ ☽ ✡ ☾ ✞</div>

  <p>Ты осмелился войти в священные тайны. Здесь ты получишь 2 рецепта:</p>
  <ul style="list-style:none; font-size:1.2em;">
    <li>📜 Постоянный рецепт (вечная шаурма)</li>
    <li>🎲 Случайный рецепт (тёмная шаурма, каждый раз разная)</li>
  </ul>

  <div class="section-title">📜 Вечный рецепт</div>
  <div id="fixed">
    - Лаваш, найденный на развалинах древнего базара<br>
    - Курица, исповедавшаяся перед жаркой<br>
    - Огурцы, выросшие под лунным светом<br>
    - Соус чесночный, замешанный на слезах ангела<br>
    - Кроваво-красный кетчуп из преисподней
  </div>

  <div class="section-title">🎲 Случайный рецепт</div>
  <button onclick="summonShawarma()">🔮 Призвать случайную шаурму</button>
  <div id="ingredients"></div>

  <script>
    const pool = [
      "рог единорога, обугленный в пламени ада",
      "волос гнома, выпавший в полнолуние",
      "лунный камень с пятнами крови",
      "капля слёз вампира",
      "пыль с могилы фараона",
      "кусок прокисшего хлеба из параллельного мира",
      "огурец, сорванный в 3 часа ночи",
      "коготь демона",
      "зуб ведьмы",
      "кетчуп из крови дракона",
      "чесночный соус из преисподней",
      "курица обычная (но с душой)"
    ];

    function summonShawarma() {
      let ing = [];
      for (let i = 0; i < 5; i++) {
        let rand = Math.floor(Math.random() * pool.length);
        ing.push(pool[rand]);
      }
      document.getElementById("ingredients").innerHTML =
        "✨ Тёмная шаурма состоит из:<br>" + ing.join("<br>");
    }
  </script>
</body>
</html>
