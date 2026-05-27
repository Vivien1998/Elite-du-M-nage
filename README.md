# Elite-du-M-nage
Création d'un site publicitaire
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Élite du Ménage | Services de Saisie & Solutions Excel Pro</title>
    <style>
        /* BASE & POLICES */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #F7FAFC;
            color: #2D3748;
            line-height: 1.6;
        }

        /* PALETTE COULEURS EXTRAITE D'EXCEL */
        :root {
            --navy-dark: #1A365D;
            --navy-light: #2B6CB0;
            --teal-medium: #319795;
            --teal-light: #E6FFFA;
            --gray-border: #CBD5E0;
            --accent-green: #C6F6D5;
        }

        /* EN-TÊTE / NAVIGATION */
        header {
            background-color: var(--navy-dark);
            color: white;
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            letter-spacing: 1px;
        }

        .logo span {
            color: #4FD1C5;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #4FD1C5;
        }

        /* HERO SECTION */
        .hero {
            background: linear-gradient(135deg, var(--navy-dark) 0%, var(--navy-light) 100%);
            color: white;
            padding: 5rem 2rem;
            text-align: center;
        }

        .hero-container {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 1.5rem;
            font-weight: 800;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .btn-main {
            background-color: var(--teal-medium);
            color: white;
            padding: 0.8rem 2rem;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            text-decoration: none;
            transition: background 0.3s, transform 0.2s;
            display: inline-block;
        }

        .btn-main:hover {
            background-color: #234E52;
            transform: translateY(-2px);
        }

        /* SERVICES SECTION */
        .services {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            color: var(--navy-dark);
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: var(--teal-medium);
            margin: 0.5rem auto 0;
            border-radius: 2px;
        }

        .grid-services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1000fr));
            gap: 2rem;
        }

        .card {
            background-color: white;
            padding: 2.5rem;
            border-radius: 8px;
            border: 1px solid var(--gray-border);
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: var(--teal-medium);
        }

        .card h3 {
            color: var(--navy-dark);
            font-size: 1.4rem;
            margin-bottom: 1rem;
        }

        /* SIMULATEUR / FORM INTÉGRÉ */
        .preview-section {
            background-color: var(--teal-light);
            padding: 4rem 2rem;
            border-top: 1px solid var(--gray-border);
            border-bottom: 1px solid var(--gray-border);
        }

        .preview-container {
            max-width: 700px;
            margin: 0 auto;
            background: white;
            padding: 2rem;
            border-radius: 8px;
            border: 1px solid var(--gray-border);
        }

        .form-group {
            margin-bottom: 1.2rem;
        }

        .form-group label {
            display: block;
            font-weight: bold;
            margin-bottom: 0.4rem;
            color: var(--navy-dark);
        }

        .form-group input, .form-group select {
            width: 100%;
            padding: 0.7rem;
            border: 1px solid var(--gray-border);
            border-radius: 4px;
            font-size: 1rem;
        }

        /* PIED DE PAGE */
        footer {
            background-color: var(--navy-dark);
            color: white;
            text-align: center;
            padding: 2rem;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo">ÉLITE DU <span>MÉNAGE</span></div>
            <nav>
                <a href="#services">Nos Outils</a>
                <a href="#simulation">Démonstration</a>
                <a href="mailto:contact@elitedumenage.fr" class="btn-main" style="padding: 0.5rem 1rem; margin-left: 1rem;">Contact</a>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="hero-container">
            <h1>Optimisez la gestion de vos bases clients</h1>
            <p>Fini les pertes de temps sur Excel. Nous concevons des interfaces de saisie intelligentes avec génération automatique de bases de données, calculs de cotations et suivi de trésorerie sur-mesure.</p>
            <a href="#simulation" class="btn-main">Tester le simulateur de démonstration</a>
        </div>
    </section>

    <section class="services" id="services">
        <h2 class="section-title">Ce que nous bâtissons pour vous</h2>
        <div class="grid-services">
            <div class="card">
                <h3>Formulaires de Remplissage Isoles</h3>
                <p>Vos collaborateurs ou vous-même remplissez une interface simplifiée et protégée sans risque de casser vos tableaux. Un simple clic génère l'archivage en arrière-plan.</p>
            </div>
            <div class="card">
                <h3>Bases de Données Structurées</h3>
                <p>Chaque entrée reçoit un ID unique incrémental. Les noms et prénoms sont automatiquement nettoyés et normalisés (ex: MAJUSCULES) pour garantir des listes parfaites.</p>
            </div>
            <div class="card">
                <h3>Calculateur de Tarification Intégré</h3>
                <p>Intégration instantanée des barèmes d'urgence, des calculs de distances kilométriques complexes avec zones de franchises, des remises séniors et des calculs d'avances URSSAF.</p>
            </div>
        </div>
    </section>

    <section class="preview-section" id="simulation">
        <h2 class="section-title">Aperçu visuel de l'interface de saisie</h2>
        <div class="preview-container">
            <div class="form-group">
                <label>Nom du Prospect / Client</label>
                <input type="text" placeholder="Ex: DEBUSSCHERE" value="Debusschere">
            </div>
            <div class="form-group">
                <label>Type de Prestation</label>
                <select>
                    <option>Standard (18.00 €/h)</option>
                    <option>Urgence (25.00 €/h)</option>
                </select>
            </div>
            <div class="form-group">
                <label>Distance du Domicile (Km)</label>
                <input type="number" value="14">
            </div>
            <button class="btn-main" style="width: 100%; margin-top: 1rem;" onclick="alert('Félicitations ! Les calculs automatiques s\'exécutent et l\'ID Client 001 est poussé vers votre feuille de données.')">⚡ Simuler l'enregistrement automatique</button>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Élite du Ménage - Systèmes d'automatisation Excel & VBA. Tous droits réservés.</p>
    </footer>

</body>
</html>
