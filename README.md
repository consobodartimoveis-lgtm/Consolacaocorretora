<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Imobiliária Horizonte</title>
  <style>
    /* ====== ESTILO GERAL ====== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: #f7f7f7;
      color: #333;
    }

    header {
      background: #004aad;
      color: white;
      padding: 15px 5%;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      font-size: 1.8em;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-weight: 500;
    }

    nav a:hover {
      text-decoration: underline;
    }

    /* ====== HERO ====== */
    .hero {
      background: url('https://images.unsplash.com/photo-1560185127-6ed189bf02ec?auto=format&fit=crop&w=1600&q=80') center/cover no-repeat;
      height: 70vh;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-shadow: 1px 1px 5px rgba(0,0,0,0.5);
      flex-direction: column;
      text-align: center;
    }

    .hero h2 {
      font-size: 2.5em;
    }

    .hero p {
      margin-top: 10px;
      font-size: 1.2em;
    }

    .btn {
      margin-top: 20px;
      background: #ffcc00;
      color: #004aad;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      font-weight: bold;
      cursor: pointer;
      transition: 0.3s;
    }

    .btn:hover {
      background: #ffaa00;
    }

    /* ====== SEÇÃO DE IMÓVEIS ====== */
    .imoveis {
      padding: 50px 5%;
    }

    .imoveis h2 {
      text-align: center;
      margin-bottom: 30px;
      color: #004aad;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .card {
      background: white;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .card-content {
      padding: 15px;
    }

    .card-content h3 {
      color: #004aad;
      margin-bottom: 10px;
    }

    /* ====== SOBRE ====== */
    .sobre {
      background: #004aad;
      color: white;
      padding: 50px 5%;
      text-align: center;
    }

    .sobre h2 {
      margin-bottom: 20px;
    }

    .sobre p {
      max-width: 700px;
      margin: 0 auto;
      line-height: 1.6;
    }

    /* ====== CONTATO ====== */
    .contato {
      padding: 50px 5%;
      background: white;
    }

    .contato h2 {
      text-align: center;
      color: #004aad;
      margin-bottom: 30px;
    }

    form {
      max-width: 600px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    input, textarea {
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
      width: 100%;
    }

    footer {
      background: #002b5c;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }

  </style>
</head>
<body>

  <!-- ====== CABEÇALHO ====== -->
  <header>
    <h1>Consolação Imóveis</h1>
    <nav>
      <a href="#home">Início</a>
      <a href="#imoveis">Imóveis</a>
      <a href="#sobre">Sobre</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>

  <!-- ====== HERO ====== -->
  <section class="hero" id="home">
    <h2>Encontre o imóvel dos seus sonhos</h2>
    <p>Casas, apartamentos e terrenos nas melhores localizações</p>
    <button class="btn" onclick="document.querySelector('#imoveis').scrollIntoView({behavior: 'smooth'})">Ver imóveis</button>
  </section>

  <!-- ====== IMÓVEIS ====== -->
  <section class="imoveis" id="imoveis">
    <h2>Nossos Destaques</h2>
    <div class="cards">
      <div class="card">
        <img src="https://images.unsplash.com/photo-1560448204-e02f11c3d0e2?auto=format&fit=crop&w=800&q=80" alt="Casa 1">
        <div class="card-content">
          <h3>Casa Moderna - Centro</h3>
          <p>3 quartos • 2 banheiros • 150m²</p>
          <p><strong>R$ 650.000</strong></p>
        </div>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=800&q=80" alt="Apartamento">
        <div class="card-content">
          <h3>Apartamento Luxo - Zona Sul</h3>
          <p>2 quartos • 1 suíte • 90m²</p>
          <p><strong>R$ 480.000</strong></p>
        </div>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1595526114035-0d45ed16cf5a?auto=format&fit=crop&w=800&q=80" alt="Terreno">
        <div class="card-content">
          <h3>Terreno Residencial</h3>
          <p>300m² • Bairro tranquilo</p>
          <p><strong>R$ 180.000</strong></p>
        </div>
      </div>
    </div>
  </section>

  <!-- ====== SOBRE ====== -->
  <section class="sobre" id="sobre">
    <h2>Sobre Nós</h2>
    <p>A Imobiliária Horizonte atua há mais de 10 anos no mercado, oferecendo as melhores opções de imóveis para compra e locação. Nosso compromisso é com a transparência, confiança e satisfação dos nossos clientes.</p>
  </section>

  <!-- ====== CONTATO ====== -->
  <section class="contato" id="contato">
    <h2>Entre em Contato</h2>
    <form>
      <input type="text" placeholder="Seu nome" required>
      <input type="email" placeholder="Seu e-mail" required>
      <input type="text" placeholder="Assunto">
      <textarea rows="5" placeholder="Mensagem"></textarea>
      <button class="btn" type="submit">Enviar</button>
    </form>
  </section>

  <!-- ====== RODAPÉ ====== -->
  <footer>
    <p>© 2025 Imobiliária Horizonte - Todos os direitos reservados.</p>
  </footer>

</body>
</html>
