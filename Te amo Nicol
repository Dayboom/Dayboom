<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Serás mi San Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe6e6;
            overflow: hidden;
        }
        h1 {
            color: #ff4d4d;
        }
        .container {
            margin-top: 100px;
        }
        .btn {
            padding: 15px 30px;
            font-size: 20px;
            border: none;
            cursor: pointer;
            margin: 10px;
            border-radius: 10px;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #999;
            color: white;
            position: absolute;
        }
        .flower {
            position: absolute;
            width: 50px;
            height: 50px;
            transition: transform 2s ease-in-out;
        }
    </style>
    <script>
        function mostrarMensaje() {
            document.getElementById("mensaje").innerHTML = "¡Sabía que dirías que sí! ❤️";
            lanzarFlores();
        }

        function moverBoton() {
            let botonNo = document.getElementById("btnNo");
            let x = Math.random() * (window.innerWidth - botonNo.offsetWidth);
            let y = Math.random() * (window.innerHeight - botonNo.offsetHeight);
            botonNo.style.left = x + "px";
            botonNo.style.top = y + "px";
        }

        function lanzarFlores() {
            for (let i = 0; i < 15; i++) {
                let flor = document.createElement("img");
                flor.src = "https://upload.wikimedia.org/wikipedia/commons/thumb/4/40/Daisy_flower.JPG/120px-Daisy_flower.JPG";
                flor.className = "flower";
                flor.style.left = Math.random() * window.innerWidth + "px";
                flor.style.top = "-50px";
                document.body.appendChild(flor);
                
                setTimeout(() => {
                    flor.style.transform = `translateY(${window.innerHeight}px)`;
                }, 100);
            }
        }
    </script>
</head>
<body>
    <div class="container">
        <h1>¿Quieres ser mi San Valentín? ❤️</h1>
        <button class="btn yes" onclick="mostrarMensaje()">Sí</button>
        <button id="btnNo" class="btn no" onmouseover="moverBoton()">No</button>
        <h2 id="mensaje"></h2>
    </div>
</body>
</html>
