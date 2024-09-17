<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Configuração do Roteador</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            padding: 20px;
        }

        .container {
            width: 300px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1 {
            text-align: center;
        }

        label {
            display: block;
            margin-top: 10px;
        }

        input[type="text"], input[type="password"], select {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            width: 100%;
        }

        input[type="submit"]:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Configurar Roteador</h1>
        <form action="configurar.php" method="POST">
            <label for="ssid">Nome da Rede (SSID):</label>
            <input type="text" id="ssid" name="ssid" required>

            <label for="senha">Senha da Rede:</label>
            <input type="password" id="senha" name="senha" required>

            <label for="seguranca">Tipo de Criptografia:</label>
            <select id="seguranca" name="seguranca">
                <option value="WPA2">WPA2</option>
                <option value="WPA3">WPA3</option>
                <option value="WEP">WEP</option>
            </select>

            <input type="submit" value="Salvar Configurações">
        </form>
    </div>
</body>
</html>
