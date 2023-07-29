# Atividade_5
<!DOCTYPE html>
<html>
<head>
  <title>Calculadora de Média Aritmética</title>
</head>
<body>
  <h1>Calculadora de Média Aritmética</h1>
  <label for="valor1">Digite o primeiro valor:</label>
  <input type="number" id="valor1" />
  <br />
  <label for="valor2">Digite o segundo valor:</label>
  <input type="number" id="valor2" />
  <br />
  <label for="valor3">Digite o terceiro valor:</label>
  <input type="number" id="valor3" />
  <br />
  <label for="valor4">Digite o quarto valor:</label>
  <input type="number" id="valor4" />
  <br />
  <button onclick="calcularMedia()">Calcular Média</button>
  <br />
  <p id="resultado"></p>

  <script>
    function calcularMedia() {
      // Obtém os valores digitados pelo usuário
      var valor1 = parseFloat(document.getElementById('valor1').value);
      var valor2 = parseFloat(document.getElementById('valor2').value);
      var valor3 = parseFloat(document.getElementById('valor3').value);
      var valor4 = parseFloat(document.getElementById('valor4').value);

      // Calcula a média aritmética dos quatro valores
      var media = (valor1 + valor2 + valor3 + valor4) / 4;

      // Exibe o resultado da média
      var resultadoElement = document.getElementById('resultado');
      resultadoElement.innerHTML = 'A média aritmética é: ' + media;
    }
  </script>
</body>
</html>
