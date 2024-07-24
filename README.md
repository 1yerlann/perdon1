<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Disculpas</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            font-family: Arial, sans-serif;
        }
        .container {
            text-align: center;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            margin: 10px;
            border: none;
            border-radius: 5px;
        }
        #yesButton {
            background-color: #28a745;
            color: white;
        }
        #yesButton:hover {
            background-color: #218838;
        }
        #noButton {
            background-color: #dc3545;
            color: white;
        }
        #noButton:hover {
            background-color: #c82333;
        }
        #thankYouMessage {
            display: none;
            margin-top: 20px;
            font-size: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>¿Me perdonas ?</h1>
        <img src="https://static-cdn.jtvnw.net/jtv_user_pictures/f1337a9b-dd5c-40c6-a4a9-fd07111cfd0b-profile_image-300x300.png" alt="Amor" width="200">
        <div class="buttons">
            <button id="yesButton">Sí</button>
            <button id="noButton">No</button>
        </div>
        <div id="thankYouMessage">
            <p>Gracias mi amorcito precioso, te debo tu pollito</p>
<img src="https://s12.gifyu.com/images/S5wwF.gif" alt="Amor" width="200">
            <img src="https://imgmedia.larepublica.pe/640x371/larepublica/original/2021/01/15/60023283c6959d0ec119a308.webp" alt="Amor" width="200">
<img src="https://c.tenor.com/Xzqqe8h_XogAAAAC/tenor.gif" alt="Amor" width="200">


        </div>
    </div>

    <script>
        const noButton = document.getElementById('noButton');
        const yesButton = document.getElementById('yesButton');
        const thankYouMessage = document.getElementById('thankYouMessage');

        noButton.addEventListener('mouseover', () => {
            const x = Math.random() * (window.innerWidth - noButton.clientWidth);
            const y = Math.random() * (window.innerHeight - noButton.clientHeight);
            noButton.style.position = 'absolute';
            noButton.style.left = `${x}px`;
            noButton.style.top = `${y}px`;
        });

        yesButton.addEventListener('click', () => {
            thankYouMessage.style.display = 'block';
        });
    </script>
</body>
</html>
