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

  <!-- Facebook Pixel Base Code -->
  <script>
    !function(f,b,e,v,n,t,s){
      if(f.fbq)return;n=f.fbq=function(){
        n.callMethod ? n.callMethod.apply(n,arguments) : n.queue.push(arguments)
      };
      if(!f._fbq)f._fbq=n;
      n.push=n;
      n.loaded=!0;
      n.version='2.0';
      n.queue=[];
      t=b.createElement(e);t.async=!0;
      t.src=v;
      s=b.getElementsByTagName(e)[0];
      s.parentNode.insertBefore(t,s)
    }(window, document,'script',
      'https://connect.facebook.net/en_US/fbevents.js');
    fbq('init', '693015023514001');
    fbq('track', 'PageView');
  </script>
</head>
<body>
  <div class="container">
    <h1>🎁 Oferta Exclusiva!</h1>
    <p>Deposite R$20 e receba um bônus de R$10<br><strong>Válido para os 100 primeiros!</strong></p>

    <!-- FORM -->
    <form onsubmit="handleForm(event)">
      <input type="text" name="nome" placeholder="Seu nome" required />
      <input type="email" name="email" placeholder="Seu email" required />
      <button type="submit">Cadastrar & Receber Oferta</button>
    </form>

    <!-- Messenger Button -->
    <a class="messenger" href="https://m.me/61576668571142" 
       onclick="fbq('trackCustom', 'MessengerClick', {eventID: 'msg123'});" target="_blank">
      Fale com a gente no Messenger
    </a>

    <div class="note">
      Promoção válida por tempo limitado. Consulte os termos via Messenger.
    </div>
  </div>

  <!-- Script to simulate form event tracking -->
  <script>
    function handleForm(event) {
      event.preventDefault();
      fbq('track', 'Lead', {
        content_name: 'LandingForm',
        eventID: 'lead123'
      });

      alert("Cadastro enviado com sucesso! Entraremos em contato.");
      event.target.reset();
    }
  </script>

  <!-- Optional: noscript fallback -->
  <noscript>
    <img height="1" width="1" style="display:none"
         src="https://www.facebook.com/tr?id=693015023514001&ev=PageView&noscript=1" />
  </noscript>
</body>
</html>
