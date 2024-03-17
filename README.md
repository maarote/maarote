<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>bobao</title>
    <style>
        body {
            background-image: url('https://img.freepik.com/vetores-gratis/fundo-de-aquarela-rosa-pintado-a-mao-detalhado_1048-17039.jpg');
        }
    </style>
</head>
<body>
    <h1>O Glauco é um bobão</h1>
    <b>Mas eu amo muitão</b>
    <p>
        <img src="https://static.tumblr.com/cadb630fdbe6065b4fcba6c4104099c7/heyalgh/0r2ndy6o2/tumblr_static_2xch03aecjcwko44ccwoc40cc_2048_v2.jpg" alt="Glauco">
    </p>
    <p>Responda o quanto me ama:</p>
    <form id="formResposta">
        Muito: <input type="radio" name="resposta" value="muito" required> <br>
        Pouco: <input type="radio" name="resposta" value="pouco"> <br>
        <input type="submit" value="Enviar">
    </form>

    <script>
        document.getElementById("formResposta").addEventListener("submit", function(event) {
            event.preventDefault(); // Impede o envio padrão do formulário

            var resposta = document.querySelector('input[name="resposta"]:checked').value;

            if (resposta === "muito") {
                alert("Resposta certa! Você me ama muitão. ❤️");
            } else {
                alert("Resposta errada! Você deveria me amar muitão! 😢");
            }
        });
    </script>
</body>
</html>
