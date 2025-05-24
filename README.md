<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Oferta Especial</title>
  <style>
    body {
      font-family: sans-serif;
      background: #f9fafb;
      color: #111827;
      text-align: center;
      padding: 40px;
    }
    .container {
      background: #ffffff;
      padding: 30px;
      border-radius: 12px;
      max-width: 500px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.05);
    }
    h1 {
      color: #1d4ed8;
    }
    p {
      font-size: 1.1em;
      margin-bottom: 20px;
    }
    input[type="text"], input[type="email"] {
      padding: 12px;
      margin: 10px 0;
      width: 100%;
      border: 1px solid #d1d5db;
      border-radius: 6px;
    }
    button {
      background: #16a34a;
      color: white;
      padding: 14px 28px;
      border: none;
      border-radius: 8px;
      font-size: 1em;
      cursor: pointer;
      margin-top: 10px;
    }
    button:hover {
      background: #15803d;
    }
    .messenger {
      display: inline-block;
      margin-top: 20px;
      background: #1877f2;
      color: white;
      padding: 12px 24px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
    }
    .note {
      font-size: 0.9em;
      color: #6b7280;
      margin-top: 30px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>🎁 Oferta Exclusiva!</h1>
    <p>Deposite R$20 e receba um bônus de R$10<br><strong>Válido para os 100 primeiros!</strong></p>

    <!-- FORM -->
    <form onsubmit="showMessage(event)">
      <input type="text" name="nome" placeholder="Seu nome" required />
      <input type="email" name="email" placeholder="Seu email" required />
      <button type="submit">Cadastrar & Receber Oferta</button>
    </form>

    <!-- Messenger Button -->
    <a class="messenger" href="https://m.me/61576668571142" target="_blank">
      Fale com a gente no Messenger
    </a>

    <div class="note">
      Promoção válida por tempo limitado. Consulte os termos via Messenger.
    </div>
  </div>

  <script>
    function showMessage(e) {
      e.preventDefault();
      alert("Cadastro enviado! Clique no botão Messenger para falar com kami.");
    }
  </script>
</body>
</html>
