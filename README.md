<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Histórico de Solicitações</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            display: flex;
            justify-content: center;
            padding: 20px;
        }
        .container {
            max-width: 800px;
            width: 100%;
            background-color: #fff;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
            padding: 20px;
            border-radius: 8px;
        }
        .header {
            text-align: center;
            margin-bottom: 20px;
        }
        .header img {
            width: 50px;
            margin-bottom: 10px;
        }
        .header h1 {
            color: #333;
        }
        .chamado {
            border-bottom: 1px solid #ddd;
            padding: 10px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .chamado:last-child {
            border-bottom: none;
        }
        .detalhes {
            color: #007bff;
            cursor: pointer;
        }
        .detalhes:hover {
            text-decoration: underline;
        }
        .button-container {
            display: flex;
            justify-content: flex-end;
            margin-top: 20px;
        }
        .button {
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <img src="https://via.placeholder.com/50" alt="Ícone Histórico">
            <h1>Histórico de Solicitações</h1>
        </div>
        <div id="listaChamados">
            <div class="chamado">
                <span>Chamado #1 - Problema no sistema</span>
                <span class="detalhes" onclick="verDetalhes(1)">Ver detalhes</span>
            </div>
            <div class="chamado">
                <span>Chamado #2 - Solicitação de atualização</span>
                <span class="detalhes" onclick="verDetalhes(2)">Ver detalhes</span>
            </div>
            <!-- Mais chamados podem ser adicionados aqui -->
        </div>
        <div class="button-container">
            <button class="button" onclick="adicionarChamado()">Novo Chamado</button>
        </div>
    </div>
    <script>
        function verDetalhes(id) {
            alert("Exibindo detalhes do chamado #" + id);
        }
        function adicionarChamado() {
            alert("Abrindo tela para novo chamado.");
        }
    </script>
</body>
</html>
