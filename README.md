<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Te Amo 10.000 Veces Sofía</title>
  <style>
    body {
      background-color: #ffe4f1;
      font-family: 'Segoe UI', sans-serif;
      text-align: center;
      padding: 30px;
    }

    h1 {
      color: #d63384;
    }

    input {
      padding: 10px;
      font-size: 16px;
      border-radius: 8px;
      border: 1px solid #ccc;
      width: 200px;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 8px;
      border: none;
      background-color: #d63384;
      color: white;
      cursor: pointer;
      margin-left: 10px;
    }

    button:hover {
      background-color: #c2185b;
    }

    #output {
      margin-top: 30px;
      white-space: pre-wrap;
      color: #e91e63;
      font-weight: bold;
      max-height: 400px;
      overflow-y: auto;
      border: 2px solid #f8bbd0;
      padding: 20px;
      background: #fff;
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <h1>TE AMA MUCHO SEBASTIAN💖</h1>
  <input type="text" id="entrada" placeholder="Escribe aquí">
  <button onclick="verificarPalabra()">Enviar</button>

  <div id="output"></div>

  <script>
    function verificarPalabra() {
      const entrada = document.getElementById("entrada").value.trim().toLowerCase();
      const salida = document.getElementById("output");

      if (entrada === "te amo") {
        let resultado = "";
        const mensaje = "💖 Te amo Sofia 💖\n";
        for (let i = 0; i < 10000; i++) {
          resultado += mensaje;
        }
        salida.textContent = resultado;
      } else {
        salida.textContent = "Escribí exactamente: te amo";
      }
    }
  </script>

</body>
</html>
