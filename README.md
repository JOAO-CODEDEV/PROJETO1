# PROJETO1<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Azzure Redes - Sua Loja de Redes Esportivas</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <div class="logo">🏐 AZZURE REDES</div>
            <nav class="nav">
                <ul>
                    <li><a href="#produtos">Produtos</a></li>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#contato">Contato</a></li>
                    <li><a href="#carrinho" class="cart-link">🛒 Carrinho <span id="cart-count">0</span></a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Redes Esportivas de Qualidade</h1>
            <p>Encontre a rede perfeita para seu esporte favorito</p>
            <button class="btn-primary" onclick="document.getElementById('produtos').scrollIntoView({behavior: 'smooth'})">
                Comprar Agora
            </button>
        </div>
    </section>

    <!-- Produtos Section -->
    <section id="produtos" class="produtos">
        <div class="container">
            <h2>Nossos Produtos</h2>
            <div class="produtos-grid" id="produtosGrid"></div>
        </div>
    </section>

    <!-- Sobre Section -->
    <section id="sobre" class="sobre">
        <div class="container">
            <h2>Sobre Azzure Redes</h2>
            <p>Somos uma empresa especializada em redes esportivas de alta qualidade. Com mais de 10 anos de experiência, fornecemos produtos para atletas profissionais e amadores.</p>
            <p>Nossa missão é proporcionar o melhor equipamento esportivo com os melhores preços do mercado.</p>
        </div>
    </section>

    <!-- Contato Section -->
    <section id="contato" class="contato">
        <div class="container">
            <h2>Entre em Contato</h2>
            <form class="form-contato" onsubmit="enviarMensagem(event)">
                <input type="text" placeholder="Seu nome" required>
                <input type="email" placeholder="Seu email" required>
                <textarea placeholder="Sua mensagem" rows="5" required></textarea>
                <button type="submit" class="btn-primary">Enviar</button>
            </form>
        </div>
    </section>

    <!-- Carrinho Modal -->
    <div id="carrinhoModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h2>Seu Carrinho</h2>
                <span class="close" onclick="fecharCarrinho()">&times;</span>
            </div>
            <div class="modal-body">
                <div id="carrinhoItens"></div>
            </div>
            <div class="modal-footer">
                <div class="total">Total: R$ <span id="totalCarrinho">0.00</span></div>
                <button class="btn-primary" onclick="finalizarCompra()">Finalizar Compra</button>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2026 Azzure Redes. Todos os direitos reservados.</p>
            <p>Contato: contato@azzureredas.com.br | Tel: (11) 9999-9999</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
