<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Thynk Unlimited - Le Monde des Bateaux</title>
  <style>
    /* Reset et style global */
    * {
      margin: 0; padding: 0; box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      background: #f0f7fa;
      color: #1a1a1a;
      line-height: 1.6;
    }
    header {
      background: #004d99;
      color: white;
      padding: 20px 40px;
      text-align: center;
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }
    nav {
      background: #003366;
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 12px 0;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      font-size: 1.1rem;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #ffcc00;
    }
    main {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }
    section {
      margin-bottom: 60px;
      background: white;
      padding: 30px 40px;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgb(0 0 0 / 0.1);
    }
    section h2 {
      margin-bottom: 20px;
      color: #004d99;
      border-bottom: 3px solid #ffcc00;
      display: inline-block;
      padding-bottom: 6px;
    }
    /* Présentation magasin */
    #accueil p {
      font-size: 1.2rem;
      margin-top: 10px;
    }

    /* Recrutement */
    #recrutement ul {
      list-style: inside square;
      font-size: 1.1rem;
      color: #333;
    }
    #recrutement li {
      margin-bottom: 10px;
    }

    /* Localisation */
    #localisation iframe {
      width: 100%;
      height: 350px;
      border: none;
      border-radius: 6px;
      margin-top: 20px;
      box-shadow: 0 3px 8px rgba(0,0,0,0.15);
    }

    /* Catégories */
    #categories .category-list {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
    }
    #categories .category-item {
      background: #004d99;
      color: white;
      padding: 20px 30px;
      border-radius: 8px;
      font-weight: 700;
      flex: 1 1 180px;
      text-align: center;
      cursor: pointer;
      transition: background 0.3s ease;
      user-select: none;
    }
    #categories .category-item:hover {
      background: #003366;
    }

    /* Liste bateaux */
    #bateaux .boat-list {
      display: grid;
      grid-template-columns: repeat(auto-fill,minmax(280px,1fr));
      gap: 25px;
    }
    #bateaux .boat-card {
      background: #fff;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgb(0 0 0 / 0.1);
      overflow: hidden;
      transition: transform 0.2s ease;
      cursor: default;
    }
    #bateaux .boat-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgb(0 0 0 / 0.15);
    }
    #bateaux img {
      width: 100%;
      height: 160px;
      object-fit: cover;
    }
    #bateaux .boat-info {
      padding: 15px 20px;
    }
    #bateaux .boat-info h3 {
      color: #004d99;
      margin-bottom: 8px;
    }
    #bateaux .boat-info p {
      font-size: 0.95rem;
      color: #555;
    }
    footer {
      text-align: center;
      padding: 20px 0;
      background: #003366;
      color: white;
      font-size: 0.9rem;
      margin-top: 40px;
    }
  </style>
</head>
<body>

<header>
  <h1>Thynk Unlimited - Le Monde des Bateaux</h1>
</header>

<nav>
  <a href="#accueil">Accueil</a>
  <a href="#recrutement">Recrutement</a>
  <a href="#localisation">Localisation</a>
  <a href="#categories">Catégories</a>
  <a href="#bateaux">Bateaux</a>
</nav>

<main>

  <section id="accueil">
    <h2>Bienvenue chez Thynk Unlimited</h2>
    <p>
      Depuis des années, nous sommes fiers d’être votre concessionnaire de confiance pour tous vos besoins en bateaux.  
      Découvrez notre savoir-faire, notre passion et notre engagement à vous offrir la meilleure expérience nautique possible.  
      Que vous soyez débutant ou marin expérimenté, nous avons le bateau parfait pour vous.
    </p>
  </section>

  <section id="recrutement">
    <h2>Recrutement</h2>
    <p>Nous recherchons des passionnés pour rejoindre notre équipe dynamique !</p>
    <ul>
      <li>Conseiller commercial bateau</li>
      <li>Mécanicien naval</li>
      <li>Agent service client</li>
      <li>Marketing & communication</li>
    </ul>
    <p>Envoyez votre CV à <a href="mailto:contact@thynkunlimited.com">contact@thynkunlimited.com</a></p>
  </section>

  <section id="localisation">
    <h2>Notre localisation</h2>
    <p>Venez nous rendre visite à notre magasin principal :</p>
    <!-- Google Maps intégré -->
    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2624.9998427972726!2d2.2944813156748677!3d48.85837007928721!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e66ef7b9f619bb%3A0x6f06d2f0b904b30b!2sTour%20Eiffel!5e0!3m2!1sfr!2sfr!4v1687665947000!5m2!1sfr!2sfr"
      allowfullscreen=""
      loading="lazy"
      referrerpolicy="no-referrer-when-downgrade"></iframe>
  </section>

  <section id="categories">
    <h2>Nos catégories de bateaux</h2>
    <div class="category-list">
      <div class="category-item">Bateaux à moteur</div>
      <div class="category-item">Voiliers</div>
      <div class="category-item">Bateaux de pêche</div>
      <div class="category-item">Bateaux de luxe</div>
      <div class="category-item">Bateaux gonflables</div>
    </div>
  </section>

  <section id="bateaux">
    <h2>Nos bateaux disponibles</h2>
    <div class="boat-list">
      <div class="boat-card">
        <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80" alt="Bateau à moteur" />
        <div class="boat-info">
          <h3>Bateau à moteur X100</h3>
          <p>Puissant et performant, parfait pour les amateurs de vitesse.</p>
        </div>
      </div>
      <div class="boat-card">
        <img src="https://images.unsplash.com/photo-1469474968028-56623f02e42e?auto=format&fit=crop&w=800&q=80" alt="Voilier élégant" />
        <div class="boat-info">
          <h3>Voilier Elegance 3000</h3>
          <p>Conçu pour les amoureux de la voile traditionnelle et du grand large.</p>
        </div>
      </div>
      <div class="boat-card">
        <img src="https://images.unsplash.com/photo-1504215680853-026ed2a45def?auto=format&fit=crop&w=800&q=80" alt="Bateau de pêche" />
        <div class="boat-info">
          <h3>Bateau de pêche FisherPro</h3>
          <p>Robuste et pratique, idéal pour la pêche en mer ou en lac.</p>
        </div>
      </div>
      <div class="boat-card">
        <img src="https://images.unsplash.com/photo-1493558103817-58b2924bce98?auto=format&fit=crop&w=800&q=80" alt="Bateau de luxe" />
        <div class="boat-info">
          <h3>Yacht Luxe 500</h3>
          <p>Alliant confort et élégance pour une expérience haut de gamme.</p>
        </div>
      </div>
    </div>
  </section>

</main>

<footer>
  &copy; 2025 Thynk Unlimited - Tous droits réservés

        &copy; 2025 Thynk Unlimited - Tous droits réservés
    </footer>
</body>
</html>
