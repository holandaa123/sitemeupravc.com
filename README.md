<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Pedido de Namoro</title>
  <style>
    body {
      font-family: Arial, sans-serif;
    }

    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    h1 {
      text-align: center;
    }

    .buttons {
      display: flex;
      justify-content: center;
      margin-top: 20px;
    }

    .button {
      margin: 0 10px;
      padding: 10px 20px;
      font-size: 18px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .button-yes {
      background-color: #4CAF50;
      color: white;
    }

    .button-no {
      background-color: #f44336;
      color: white;
      transition: transform 0.3s;
    }

    .button-no:hover {
      transform: translateX(calc(100vw - 100%));
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Pedido de Namoro</h1>
    <div class="buttons">
      <button class="button button-yes">Sim</button>
      <button class="button button-no">Não</button>
    </div>
  </div>

  <script>
    const buttonNo = document.querySelector('.button-no');

    buttonNo.addEventListener('mouseover', () => {
      buttonNo.style.transform = `translateX(${Math.random() * (window.innerWidth - buttonNo.offsetWidth)}px)`;
    });

    buttonNo.addEventListener('mouseout', () => {
      buttonNo.style.transform = 'translateX(0)';
    });
  </script>
</body>
</html>
