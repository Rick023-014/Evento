<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Evento Felix</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; }
        nav { background: #333; padding: 10px; }
        nav a { color: white; margin: 0 15px; text-decoration: none; }
        .container { padding: 20px; }
        .hidden { display: none; }
        .button { padding: 10px 20px; background: green; color: white; border: none; cursor: pointer; }
        .home-image, .churrasco-image { width: 80%; max-width: 600px; margin-top: 20px; }
    </style>
</head>
<body>
    <nav>
        <a href="#" onclick="showSection('home')">Home</a>
        <a href="#" onclick="showSection('churrasco')">Churrasco</a>
        <a href="#" onclick="showSection('agendamento')">Agendamento</a>
    </nav>
    
    <div id="home" class="container">
        <h1>Bem-vindo ao Evento Felix</h1>
        <p>Organizamos eventos incríveis para você!</p>
        <img src="c:\Users\rickl\Downloads\felix eventos.jpg" alt="Imagem do Evento" class="home-image">
    </div>
    
    <div id="churrasco" class="container hidden">
        <h1>Churrasco</h1>
        <p>Nosso evento de churrasco inclui:</p>
        <ul>
            <li>Carne de primeira</li>
            <li>Arroz</li>
            <li>Vinagrete</li>
            <li>Farofa</li>
            <li>Bebidas geladas</li>
        </ul>
        <img src="c:\Users\rickl\Downloads\churrasco.jpg" alt="Imagem do Churrasco" class="churrasco-image">
    </div>
    
    <div id="agendamento" class="container hidden">
        <h1>Agendamento</h1>
        <p>Para agendar um evento, clique no botão abaixo:</p>
        <button class="button" onclick="window.location.href='https://wa.me/5511989132689'">Agendar via WhatsApp</button>
    </div>
    
    <script>
        function showSection(sectionId) {
            document.querySelectorAll('.container').forEach(div => div.classList.add('hidden'));
            document.getElementById(sectionId).classList.remove('hidden');
        }
    </script>
</body>
</html>
