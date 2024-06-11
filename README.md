<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>feliz dia dos namorados</title>

    <style>
        body {
            background-color: red;

        }


        .painel {
            margin: auto;
            background-color: white;
            width: 500px;
            height: 500px;
            border-radius: 20px;
            text-align: center;
            padding-top: 50px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }

        #sim {
            height: 40px;
            width: 60px;
            background-color: red;
            border: 2px solid white;
            border-radius: 10px;
            color: white;
            margin-left: -60px;

        }

        #nao {
            position: absolute;
            height: 40px;
            width: 60px;
            background-color: red;
            border: 2px solid white;
            border-radius: 10px;
            color: white;
            margin-left: 10px;

        }
    </style>

</head>

<body>


    <div class="painel">
        <h1> feliz dia dos namorados</h1>

        <img src="https://gifman.net/wp-content/uploads/2019/06/ursinho-fofo-apaixonado.gif" alt="">

        <h2>aceita namorar comigo?</h2>

        <button id="sim" onclick="parabens()"> sim! </button>
        <button onmouseover="fuja()" id="nao"> nao! </button>

    </div>

    <script>
        function fuja() {
            var botaoNao = document.getElementById("nao")

            var largurajanela = window.innerWidth;
            var alturajanela = window.innerHeight;

            var maxX = largurajanela - botaoNao.offsetWidth;
            var maxY = alturajanela - botaoNao.offsetHeight;

            var aleatorioX = Math.floor(Math.random() * maxX);
            var aleatorioY = Math.floor(Math.random() * maxY);

            botaoNao.style.left = aleatorioX + "px";
            botaoNao.style.top = aleatorioY + "px";
        }

        function parabens() {
            alert("parabens, voce fez a escolha certa:) ")
        }
    </script>

    </div>

</body>

</html>
