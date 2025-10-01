<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A História do Punk Rock</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            font-size: 16px;
            background-color: #ffffff;
            color: #000000;
            transition: background-color 0.3s, color 0.3s;
            padding: 20px;
            line-height: 1.6;
        }

        header {
            margin-bottom: 20px;
        }

        button {
            padding: 8px 12px;
            font-size: 14px;
            cursor: pointer;
            margin-right: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #f0f0f0;
        }

        .alto-contraste {
            background-color: #000000;
            color: #ffff00;
        }
        
        .alto-contraste button {
            background-color: #ffff00;
            color: #000000;
            border-color: #fff;
        }
    </style>
</head>
<body>

    <header>
        <button id="btn-aumentar">A+</button>
        <button id="btn-diminuir">A-</button>
        <button id="btn-contraste">Contraste</button>
    </header>
    
    <h1>Bem-vindo à Página da História do Punk Rock!</h1>
    
    <p>
        Prepare-se para uma viagem no tempo e descubra como um gênero musical
        revolucionou a música e a cultura.
    </p>

    <h2>O Que Foi o Punk Rock?</h2>
    
    <p>
        O **Punk Rock** surgiu em meados dos anos 70 como uma resposta
        ao que era visto como a "complacência" do rock progressivo e do rock
        de arena da época. Caracterizado por músicas curtas e rápidas, com
        instrumentação crua e letras que abordavam temas como rebeldia,
        anarquia e crítica social, o punk foi mais que um estilo musical;
        foi um movimento cultural. Bandas como os Ramones, Sex Pistols e
        The Clash se tornaram ícones dessa era, influenciando não apenas
        a música, mas também a moda e o comportamento. A sua filosofia
        "faça você mesmo" (DIY - Do It Yourself) inspirou gerações a
        criar arte de forma independente e autêntica.
    </p>

    <script>
        const btnAumentar = document.getElementById('btn-aumentar');
        const btnDiminuir = document.getElementById('btn-diminuir');
        const btnContraste = document.getElementById('btn-contraste');
        const corpoPagina = document.body;

        let tamanhoFonteAtual = 16;
        
        btnAumentar.addEventListener('click', () => {
            tamanhoFonteAtual += 2;
            corpoPagina.style.fontSize = `${tamanhoFonteAtual}px`;
        });

        btnDiminuir.addEventListener('click', () => {
            if (tamanhoFonteAtual > 10) { 
                tamanhoFonteAtual -= 2;
                corpoPagina.style.fontSize = `${tamanhoFonteAtual}px`;
            }
        });
        
        btnContraste.addEventListener('click', () => {
            corpoPagina.classList.toggle('alto-contraste');
        });
    </script>

</body>
</html>

