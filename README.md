
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Testes para Processo Seletivo</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      line-height: 1.5;
    }
    h2 {
      color: #1a237e;
    }
    textarea, input[type="text"] {
      width: 100%;
      padding: 8px;
      margin: 5px 0 15px 0;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    button {
      background: #25d366;
      color: #fff;
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }
    button:hover {
      background: #1ebe5b;
    }
  </style>
</head>
<body>
  <h1>Testes para Processo Seletivo</h1>

  <h2>1. Teste de Interpretação</h2>
  <p><b>Texto:</b><br>
  “O consórcio é uma forma de compra planejada, sem juros, em que um grupo de
  pessoas contribui mensalmente para a aquisição de bens ou serviços. Cada mês ocorre
  uma assembleia para contemplação, onde alguns participantes são sorteados ou ofertam
  lances para receber o crédito antecipado.”</p>

  <label>1. O que é o consórcio?</label>
  <textarea id="q1"></textarea>

  <label>2. O consórcio tem juros?</label>
  <textarea id="q2"></textarea>

  <label>3. Como são escolhidos os contemplados?</label>
  <textarea id="q3"></textarea>

  <label>4. O que é possível adquirir pelo consórcio?</label>
  <textarea id="q4"></textarea>

  <label>5. Qual a vantagem do consórcio em relação ao financiamento?</label>
  <textarea id="q5"></textarea>

  <h2>2. Teste de Raciocínio Lógico</h2>
  <label>1. Complete a sequência: 3, 6, 9, 12, ______?</label>
  <input type="text" id="q6">

  <label>2. Próximo número na sequência: 2, 4, 8, 16, ______?</label>
  <input type="text" id="q7">

  <label>3. Se hoje é terça-feira, que dia será daqui a 10 dias?</label>
  <input type="text" id="q8">

  <label>4. João tem 3 maçãs e dá 2 para Maria. Quantas maçãs João tem agora?</label>
  <input type="text" id="q9">

  <label>5. Se todos os carros são veículos e todos os veículos têm rodas, os carros têm rodas? (Sim/Não)</label>
  <input type="text" id="q10">

  <h2>3. Teste de Cálculo</h2>
  <label>1. Calcule 0,3% de R$ 183.452,67</label>
  <input type="text" id="q11">

  <label>2. Uma parcela mensal é R$ 780, paga em 72 meses. Qual o valor total pago?</label>
  <input type="text" id="q12">

  <label>3. Se o valor do consórcio é R$ 150.000 e a taxa administrativa é 15%, qual o valor total a ser pago?</label>
  <input type="text" id="q13">

  <label>4. Qual é 10% de R$ 200.000?</label>
  <input type="text" id="q14">

  <label>5. Se um cliente paga R$ 1.900 por mês durante 72 meses, qual o valor total pago?</label>
  <input type="text" id="q15">

  <button onclick="enviar()">Enviar Respostas</button>

  <script>
    function enviar() {
      let respostas = "";
      for (let i = 1; i <= 15; i++) {
        respostas += "Q" + i + ": " + document.getElementById("q" + i).value + "%0A";
      }

      // Seu número de WhatsApp (coloque com DDI 55 e DDD da sua região)
      let telefone = "5598985315556"; 

      let url = "https://wa.me/" + telefone + "?text=Respostas do Candidato:%0A%0A" + respostas;

      window.open(url, "_blank");
    }
  </script>
</body>
</html>
