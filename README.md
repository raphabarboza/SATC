<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sex and the City</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #ff69b4;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        h1 {
            font-size: 36px;
            font-family: "Times New Roman", Times, serif;
        }
        h2 {
            font-size: 24px;
            font-family: "Times New Roman", Times, serif;
        }
        p {
            font-size: 18px;
            line-height: 1.6;
            margin-bottom: 20px;
            font-family: "Times New Roman", Times, serif;
        }
        .container {
            width: 80%;
            margin: auto;
            padding: 20px;
        }
        .btn {
            display: inline-block;
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            text-align: center;
            text-decoration: none;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        .btn:hover {
            background-color: #45a049;
        }

        .slideshow-container {
            max-width: 600px;
            position: relative;
            margin: auto;
        }

        .slide {
            display: none;
        }

        .slide img {
            width: 100%;
            height: auto;
        }


        .prev, .next {
            cursor: pointer;
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            width: auto;
            padding: 16px;
            margin-top: -22px;
            color: white;
            font-weight: bold;
            font-size: 20px;
            transition: 0.6s ease;
            border-radius: 0 3px 3px 0;
            user-select: none;
        }

        .next {
            right: 0;
            border-radius: 3px 0 0 3px;
        }

        .prev:hover, .next:hover {
            background-color: rgba(0, 0, 0, 0.8);
        }
    </style>
</head>
<body>
    <img src="foto0.png" height="10%" width="100%">

    <header>
        <h1>Sex and the City</h1>
        <h2>Uma série icônica sobre amor, amizade e moda em Nova York</h2>
        <img src="foto1.jpeg" height="10%" width="100%">

    </header>

    <div class="container">
        <center>
        <h2 style="background-color: #ff69b4; color: #fff";>Sobre a Série</h2>
        <p>"Sex and the City" é uma série de televisão americana que foi ao ar de 1998 a 2004, 
            com um total de seis temporadas. Criada por Darren Star e baseada no livro de mesmo nome 
            de Candace Bushnell,
             a série se tornou um fenômeno cultural e um marco na história da televisão.
             A série acompanha as aventuras amorosas, as amizades leais e os desafios profissionais dessas
              quatro mulheres em busca de felicidade e realização pessoal na tumultuada Nova York dos anos 90 e 
              início dos anos 2000. Com diálogos afiados, moda deslumbrante, cenários icônicos e uma trilha sonora
               marcante, "Sex and the City" capturou a essência
              da vida urbana moderna e explorou temas como sexualidade,
               feminismo, casamento, carreira e autoestima. </p>

            <center>
            <img src="foto2.jpg" alt="Logo de Sex and the City" style="max-width: 300px;">
            <img src="foto3.jpeg" alt="Cena de Nova York em Sex and the City" style="max-width: 300px;">
            <img src="foto4.webp" alt="Cena de Nova York em Sex and the City" style="max-width: 300px;">
        </center>

        <h2 style="background-color: #ff69b4; color: #fff";>Personagens Principais</h2>
        <p>Ambientada na vibrante cidade de Nova York, "Sex and the City" gira em torno da vida de quatro amigas:
             Carrie Bradshaw, interpretada por Sarah Jessica Parker, uma escritora e colunista que explora os
             complexos meandros do amor e relacionamentos em sua coluna no jornal; Samantha Jones, 
             interpretada por Kim Cattrall, uma relações-públicas confiante e sexualmente liberada; 
             Charlotte York, interpretada por Kristin Davis, uma marchande de arte conservadora e
              romântica incurável; 
            e Miranda Hobbes, interpretada por Cynthia Nixon, uma advogada pragmática e independente.</p>

        <h2 style="background-color: #ff69b4; color: #fff"; >Assista Agora</h2>
        <p>Se você ainda não viu "Sex and the City", pode assistir agora em várias plataformas de streaming. 
            Clique no botão abaixo para encontrar onde assistir!</p>
        <a href="https://www.google.com/search?q=assistir+sex+and+the+city" class="btn">Onde Assistir</a>

        <h2 style="background-color: #ff69b4; color: #fff"; >Imagens da Série</h2>
    </center>

    <div class="slideshow-container">
        <div class="slide fade">
            <img src="foto6.jpg" alt="foto6">
        </div>
        <div class="slide fade">
            <img src="foto5.jpg" alt="foto5">
        </div>
        <div class="slide fade">
            <img src="foto4.webp" alt="foto4">
        </div>
        <div class="slide fade">
            <img src="foto3.jpeg" alt="foto3">
        </div>
        <div class="slide fade">
            <img src="foto2.jpg" alt="foto2">
        </div>
        <div class="slide fade">
            <img src="foto1.jpeg" alt="foto1">
        </div>
        <div class="slide fade">
            <img src="foto0.png" alt="foto0">
        </div>
       
        <a class="prev" onclick="plusSlides(-1)">❮</a>
        <a class="next" onclick="plusSlides(1)">❯</a>
    </div>

    <script>
        var slideIndex = 0;
        showSlides();

        function showSlides() {
            var i;
            var slides = document.getElementsByClassName("slide");
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";
            }
            slideIndex++;
            if (slideIndex > slides.length) {slideIndex = 1}
            slides[slideIndex-1].style.display = "block";
            setTimeout(showSlides, 2000); // Muda a imagem a cada 2 segundos (2000 milissegundos)
        }

        function plusSlides(n) {
            showSlides(slideIndex += n);
        }
    </script>
</body>
</html>
