<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flashcards com Imagens</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Fredoka One', cursive;
      background: linear-gradient(to right, #fceabb, #f8b500);
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 30px;
    }

    .flashcard {
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      width: 240px;
      height: 200px;
      margin: 15px;
      border-radius: 15px;
      perspective: 1000px;
      cursor: pointer;
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
      transition: transform 0.2s;
    }

    .flashcard:hover {
      transform: scale(1.05);
    }

    .inner-card {
      position: relative;
      width: 100%;
      height: 100%;
      transition: transform 0.8s;
      transform-style: preserve-3d;
    }

    .flashcard.flipped .inner-card {
      transform: rotateY(180deg);
    }

    .front, .back {
      position: absolute;
      width: 100%;
      height: 100%;
      backface-visibility: hidden;
      border-radius: 15px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 10px;
      font-size: 16px;
      color: #fff;
      text-align: center;
    }

    .front {
      background: #00c9ff;
    }

    .back {
      background: #92fe9d;
      transform: rotateY(180deg);
    }

    .flashcard img {
      width: 80px;
      height: 80px;
      border-radius: 10px;
      object-fit: cover;
      margin-bottom: 10px;
      border: 2px solid white;
    }
  </style>
</head>
<body>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/7/7c/Pedro_Álvares_Cabral.jpg" alt="Cabral">
        Quem descobriu o Brasil?
      </div>
      <div class="back">Pedro Álvares Cabral</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/e/e2/Jupiter_by_Cassini-Huygens.jpg" alt="Júpiter">
        Qual é o maior planeta do sistema solar?
      </div>
      <div class="back">Júpiter</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/3/36/Proclamacao_republica.jpg" alt="Proclamação">
        Quando foi a Proclamação da República?
      </div>
      <div class="back">15 de novembro de 1889</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/7/76/Chlorophyll_molecule_ball.png" alt="Clorofila">
        Função da clorofila nas plantas?
      </div>
      <div class="back">Captar luz para fotossíntese</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/d/d9/Tiradentes_por_Oscar_Pereira_da_Silva.jpg" alt="Tiradentes">
        Quem foi Tiradentes?
      </div>
      <div class="back">Líder da Inconfidência Mineira</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/f/f7/DNA_Overview2.png" alt="DNA">
        O que é DNA?
      </div>
      <div class="back">Molécula que carrega material genético</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/6/65/Prise_de_la_Bastille.jpg" alt="Revolução Francesa">
        O que foi a Revolução Francesa?
      </div>
      <div class="back">Queda da monarquia na França (1789)</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/d/df/Human_lungs.png" alt="Pulmões">
        Órgão da respiração?
      </div>
      <div class="back">Pulmões</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/e/ef/Princess_Isabel_of_Brazil_c.1887.jpg" alt="Lei Áurea">
        Quando foi assinada a Lei Áurea?
      </div>
      <div class="back">13 de maio de 1888</div>
    </div>
  </div>

  <div class="flashcard" onclick="this.classList.toggle('flipped')">
    <div class="inner-card">
      <div class="front">
        <img src="https://upload.wikimedia.org/wikipedia/commons/0/0b/Unicellular_organism_diagram.svg" alt="Unicelulares">
        O que são seres unicelulares?
      </div>
      <div class="back">Organismos de uma única célula</div>
    </div>
  </div>

</body>
</html>
