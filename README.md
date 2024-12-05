# quizzest
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zest</title>
    <link rel="stylesheet" href="./style/style.css">
    <link rel="shortcut icon" href="img/logoicon3.ico" type="image/x-icon">
    <style>
        head {
  box-sizing: border-box;
  display: none;
}

body {
  display: block;
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  margin: auto;
  height: 100%;
  width: 100%;
  background: #c7d9f1;
  background-image: url(../img/background.png);
  background-size: cover;
  background-repeat: repeat;
  background-position: center;
}
.content {
  width: 100%;
  margin: 50px auto 0 auto;
  max-width: 550px;
}
header {
  text-align: center;
  color: #55605b;
  background-attachment: fixed;
}
h1 {
  font-size: 40px;
  font-family: impact, serif;
}
p {
  color: #55605b;
  margin: 2px;
  font-size: 20px;
}
rooter {
  font-style: italic;
}
.span {
  font-size: 15px;
  color: #6e7c76be;
}
form {
  background-color: beige;
  border-radius: 10px;
  padding: 20px;
  box-shadow: 5px 5px 5px 5px #6e7c76be;
  margin-top: auto;
}
.form-grupo {
  margin: auto;
  padding: 3px;
}
.form-control {
  width: 100%;
  display: block;
  height: 30px;
  padding: 5px;
  color: #55605b;
  background-color: #fff;
  border-radius: 5px;
  border-color: #626d7ab2;
}
label {
  display: flex;
  align-items: center;
  margin: 10px;
  color: #55605b;
}
*,
*::after,
*::before {
  box-sizing: border-box;
}
select {
  margin: 5px;
}
.input-checkbox {
  margin-right: 10px;
}
.input-textarea {
  padding: 10px;
  min-height: 120px;
  width: 100%;
  resize: vertical;
}

.submit-button {
  width: 100%;
  background-color: #e5d404;
  padding: 10px;
  cursor: pointer;
  border-radius: 10px;
  border: none;
  color: #55605b;
  font-family: Impact, Haettenschweiler, "Arial Narrow Bold", sans-serif;
  font-size: larger;
}

    </style>
</head>
<body>
    <div class="content">
    <header>
    <h1 id="title" class="center-text">Quiz de Satisfação Zest</h1>
    <p id="description" class="center-text">Conte-nos o quão saboroso estava seu pedido. Obrigado por tirar um tempinho para nossa melhora.</p>
    <rooter>Zest Confeitaria agradece</rooter></header>
    <form id="survey-form">
        <div class="form-grupo">
            <label id="name-label" for="Nome">Nome</label>
            <input type="text" name="Nome" id="name" placeholder="ZÉst da Silva" required class="form-control">
        </div>
        <div class="form-grupo">
            <label id="email-label" for="email">Email: </label>
            <input type=email name="email" placeholder="amoZEST@gmail.com" id="email" required class="form-control">
        </div>
        <div class="form-grupo">
            <label id="number-label" for="Idade">Quantos anos você tem?</label>
                <input type="number" id="Idade" min="1" max="99" placeholder="Idade" class="form-control">
        </div>
        <div class="form-grupo">
            <label id="insta-label" for="instagram">Mande seu Instagram!</label>
             <span class="span">(opicional)</span><input type="text" name="Instagram" id="instagram" class="form-control" placeholder="@ZestConfeitaria">
        </div>
        <div class="form-grupo">
            <label id="niver-label" for="niver">Seu Aniversário! </label>
             <input type="date" name="Aniversário" id="niver" class="form-control">
        </div>

        <div class="form-grupo">
            <p>Quanto você amou a Zest?</p>
            <label ><input name="satisfaçao" type="radio" value="Muito">Muito! Quero Zest todo evento.</label>
            <label ><input name="satisfaçao" type="radio" value="Gostei">Gostei! Quero Zest de vez em quando.</label>
            <label ><input name="satisfaçao" type="radio" value="Mais ou menos">Mais ou menos! Quero Zest por enquanto não.</label>
        </div>
        <div class="form-grupo">
            <p>Qual sua experiência favortia da Zest até agora?</p>
            <label for="favorito"></label>
            <select name="favorito" id="dropdown" class="form-control" required>
                <option disabled selected value="Selecione uma opção."></option>
                <option value="Bolo">Bolo Gostosão.</option>
                <option value="Doces">Doces Deliciosos.</option>
                <option value="Atendimento">Bom atendimento.</option>
                <option value="0">Confeiteiro Lindoo.</option>
                <option value="Todos">Todas as opções, menos a de cima.</option>
            </select>
        </div>
        <div class="form-grupo">
           <p> Que sabor de fatia gostaria que vendesse na Sexta da Fatia?
            <span class="span">(Sexta da Fatia é uma promoção semanal das fatias de bolo dos sabores mais votados.)</span>
           </p>
            <label ><input name="prefer" class="input-checkbox" type="checkbox" value="chocolate" id="sabor">Chocolate e Laranja</label>
            <label ><input name="prefer" class="input-checkbox" type="checkbox" value="limao" id="sabor">Limão e Mirtilo</label>
            <label ><input name="prefer" class="input-checkbox" type="checkbox" value="coco" id="sabor">Amêndoas e Coco</label>
            <label ><input name="prefer" class="input-checkbox" type="checkbox" value="abacaxi" id="sabor">Ninho e Abacaxi</label>
            
        </div>
        <div class="form-grupo">
            <p>Algum comentário ou sugestão?</p> 
            <textarea name="comentarios" id="comentarios" class="input-textarea" placeholder="Escreva aqui com toda a doçura de nossos doces ou até o azedinho do limão tão amado na Zest."></textarea>
        </div>
        <div class="form-grupo">
            <button type="submit" id="submit" class="submit-button">Enviar</button>
        </div>
    </div>
</body>
</html>
