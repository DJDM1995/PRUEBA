<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Acceso Protegido</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; margin-top: 50px; }
        input { padding: 10px; margin: 10px; }
        button { padding: 10px 20px; cursor: pointer; }
    </style>
    <script>
        function verificar() {
            var password = document.getElementById("password").value;
            if (password === "1234") {  // Reemplaza "1234" con la contraseña real
                window.location.href = "https://google.com";  // Reemplaza con tu enlace real
            } else {
                alert("❌ Contraseña incorrecta. Intenta de nuevo.");
            }
        }
    </script>
</head>
<body>
    <h2>🔒 Página Protegida</h2>
    <p>Ingrese la contraseña para acceder al contenido:</p>
    <input type="password" id="password" placeholder="Escriba la contraseña">
    <button onclick="verificar()">🔑 Acceder</button>
</body>
</html>
