<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Nossa Cafeteria</title>
    <link rel="stylesheet" href="body.{css">
</head>
<body>
    <header>
        <h1>Bem-vindo à Nossa Cafeteria!</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="cadastro.php">Cadastro</a></li>
                <li><a href="compras.html">Compras</a></li>
                <li><a href="ajuda.html">Ajuda</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <h2>Nosso Destaque</h2>
        <img src="cafe-destaque.jpg" alt="Café Especial">
        <p>Experimente o nosso delicioso café especial!</p>
    </main>
    <footer>
        <p>&copy; 2024 Nossa Cafeteria</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Cadastro de Cliente</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Cadastro de Cliente</h1>
    </header>
    <main>
        <form action="processa_cadastro.php" method="post">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" name="nome" required>
            
            <label for="email">E-mail:</label>
            <input type="email" id="email" name="email" required>
            
            <button type="submit">Cadastrar</button>
        </form>
    </main>
    <footer>
        <p>&copy; 2024 Nossa Cafeteria</p>
    </footer>
</body>
</html>
<?php
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $nome = $_POST['nome'];
    $email = $_POST['email'];

    // Processar os dados (por exemplo, salvar no banco de dados)
    
    echo "Cadastro realizado com sucesso!";
}
?>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Opções de Compra</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Opções de Compra</h1>
    </header>
    <main>
        <div class="produto">
            <img src="cafe1.jpg" alt="Café 1">
            <p>Café Tradicional - R$10,00</p>
            <button>Adicionar ao Carrinho</button>
        </div>
        <div class="produto">
            <img src="cafe2.jpg" alt="Café 2">
            <p>Café Expresso - R$12,00</p>
            <button>Adicionar ao Carrinho</button>
        </div>
    </main>
    <footer>
        <p>&copy; 2024 Nossa Cafeteria</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Ajuda ao Cliente</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Ajuda ao Cliente</h1>
    </header>
    <main>
        <h2>FAQ</h2>
        <p>Perguntas frequentes e suas respostas.</p>
        
        <h2>Contato</h2>
        <form action="envia_contato.php" method="post">
            <label for="mensagem">Mensagem:</label>
            <textarea id="mensagem" name="mensagem" required></textarea>
            <button type="submit">Enviar</button>
        </form>
    </main>
    <footer>
        <p>&copy; 2024 Nossa Cafeteria</p>
    </footer>
</body>
</html>
