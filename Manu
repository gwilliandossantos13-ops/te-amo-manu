<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Te Amo Manu ❤️</title>

  <style>
    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: black;
      font-family: Arial, Helvetica, sans-serif;
      transition: background 0.6s ease;
    }

    /* FUNDO COM FOTO (só ativa aos 100%) */
    body.fundo-ativo {
      background:
        linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
        url("https://drive.google.com/uc?export=view&id=1qEKIHGDlW9xRCAVwwSQ_tp3rZJH6U6m6")
        no-repeat center center fixed;
      background-size: cover;
    }

    .card {
      background: white;
      padding: 30px;
      border-radius: 18px;
      text-align: center;
      box-shadow: 0 10px 25px rgba(0,0,0,0.4);
      max-width: 330px;
      width: 90%;
    }

    h1 {
      margin-bottom: 10px;
      color: #ff4d6d;
    }

    .counter {
      font-size: 32px;
      font-weight: bold;
      margin: 20px 0;
      color: #333;
    }

    .bar {
      width: 100%;
      height: 16px;
      background: #eee;
      border-radius: 10px;
      overflow: hidden;
      margin-bottom: 20px;
    }

    .bar-fill {
      height: 100%;
      width: 0%;
      background: linear-gradient(90deg, #ff4d6d, #ff8fa3);
      transition: width 0.3s ease;
    }

    button {
      background: #ff4d6d;
      color: white;
      border: none;
      padding: 12px 20px;
      font-size: 18px;
      border-radius: 12px;
      cursor: pointer;
    }

    button:disabled {
      background: #aaa;
      cursor: not-allowed;
    }

    .message {
      margin-top: 15px;
      color: #555;
      font-size: 16px;
    }

    #finalText {
      display: none;
      margin-top: 20px;
      color: #333;
      font-size: 15px;
      line-height: 1.5;
    }
  </style>
</head>

<body>
  <div class="card">
    <h1>💖 Para Você 💖</h1>
    <p>Cada clique aumenta meu amor por vc</p>

    <div class="counter" id="counter">0%</div>

    <div class="bar">
      <div class="bar-fill" id="barFill"></div>
    </div>

    <button id="loveButton">Te amo ❤️</button>

    <div class="message" id="message"></div>

    <div id="finalText">
      <p><strong>Manu</strong>, vc é o meu anjo. Eu não consigo viver sem vc.</p>
      <p>Eu queria ter te conhecido antes; não sei nem como eu conseguia viver sem vc.</p>
      <p>Vc é uma perfeição de mulher. Eu te acho incrível, linda, perfeita e o amor da minha vida.</p>
      <p>E eu quero te pedir um favor: por favor, sempre que eu fizer algo que vc não goste, me fala. Eu quero ser perfeito pra vc também.</p>
      <p style="font-weight:bold; color:#ff4d6d;">TE AMO, MANU ❤️</p>
    </div>
  </div>

  <script>
    let contador = 0;

    const counterEl = document.getElementById('counter');
    const barFill = document.getElementById('barFill');
    const button = document.getElementById('loveButton');
    const message = document.getElementById('message');

    button.addEventListener('click', () => {
      if (contador < 100) {
        contador += 10;
        if (contador > 100) contador = 100;

        counterEl.textContent = contador + '%';
        barFill.style.width = contador + '%';
      }

      if (contador === 100) {
        button.disabled = true;
        message.textContent = 'Chegamos a 100%! 💕';
        document.getElementById('finalText').style.display = 'block';
        document.body.classList.add('fundo-ativo');
      }
    });
  </script>
</body>
</html>
