<!DOCTYPE html>
<html lang="pt-BR">
	<head>
		<meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<link href="https://fonts.googleapis.com/css2?family=Inter&display=swap" rel="stylesheet">
		<link rel="stylesheet" href="desafio-de-codificacao.css">
		<title>Decodificador</title>
		
	</head>
	<body>
		<header>
			<img src="frame 6.png" alt="Logo da Alura com a inicial da letra a">
		</header>

		<main>

			<section>
			<textarea class="input-texto" cols="40" rows="6" id="texto" placeholder="digite seu texto"></textarea>
			<div id="div-desaparece">
				<h6 class="informacao"> Apenas letras minúsculas e sem acento</h6>
			</div>
			<div class="botoes">
				<button class="encriptar" onclick="btnEncriptar()">
				Criptografar
				</button>
				<button class="descriptar" onclick="btnDescriptar()">
				Descriptografar
				</button>
			</div>
			</section>

			<section>
			<textarea cols="18" rows="8" class="mensagem"></textarea>
			<div id="div-aparece">
				<button class="copiar" onclick="copiar()">Copiar</button>
			</div>
			</section>
			
		</main>
		<script src="script.js"></script>

	</body>
</html>

*{
	font-family: 'Inter', sans-serif;
	font-size: 32px;
	font-weight: 400;
	line-height: 150%;
}
body{
	background:#F3F5FC;
}

main{
	display: flex;
	margin-left: 80px;
	margin-bottom: 50px;
}

.input-texto{
	margin-top: 90px;
}

.mensagem{
	position: absolute;
    margin-top: 20px;
    margin-left: 90px;
    background-image: url("boneco.png");
    background-repeat: no-repeat;
    background-position: 18px;
    background-size: 300px;
   
}

.copiar{
	position: relative;
    margin-top: 330px;
    margin-left: 205px;
}

.botoes{
	display: flex;
	flex-direction: row;
	margin-top: 20px;
}

.encriptar{
	background-color: #0A3871;
    color:white;
}

.descriptar{
	margin-left: 30px;
}

.informação{
	 font-size: 15px;
}
