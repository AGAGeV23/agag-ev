# Creating the HTML and CSS for the website
html_content = """
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AGAG e.V - Ensemble pour un avenir meilleur</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        header {
            background-color: #4a2c2a;
            color: #fff;
            padding: 1rem 0;
            text-align: center;
        }
        header img {
            max-width: 100px;
            display: block;
            margin: 0 auto;
        }
        header h1 {
            margin: 0.5rem 0;
        }
        nav {
            background: #6a4e4b;
            color: white;
            padding: 0.5rem;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 1rem;
            text-decoration: none;
        }
        .container {
            padding: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        .section {
            margin-bottom: 2rem;
        }
        .section h2 {
            color: #4a2c2a;
        }
        .team img {
            max-width: 200px;
            border-radius: 50%;
        }
        footer {
            background: #4a2c2a;
            color: white;
            text-align: center;
            padding: 1rem 0;
            margin-top: 2rem;
        }
        @media (max-width: 768px) {
            nav {
                font-size: 0.9rem;
            }
            .team img {
                max-width: 150px;
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="logo.png" alt="AGAG e.V Logo">
        <h1>AGAG e.V</h1>
        <p>Ensemble pour un avenir meilleur</p>
    </header>
    <nav>
        <a href="#about">À propos</a>
        <a href="#team">Équipe</a>
        <a href="#contact">Contact</a>
        <a href="#donation">Faire un don</a>
    </nav>
    <div class="container">
        <section id="about" class="section">
            <h2>À propos de nous</h2>
            <p>L'association est basée à Göttingen, et son objectif est d'aider les Guinéens à mieux s'intégrer en Allemagne. 
            Nous les accompagnons dans leur recherche de formations, de travail, de logement, dans leurs procédures d'asile et surtout pour aller à l'école.</p>
            <p>En Guinée, nous avons pour objectif d'aider les enfants orphelins à aller à l'école et de contribuer à améliorer la vie des villageois en leur offrant de l'eau potable en creusant des forages.</p>
        </section>
        <section id="team" class="section">
            <h2>Notre équipe</h2>
            <div class="team">
                <img src="president.png" alt="Président Ibrahim Barry">
                <p><strong>Président :</strong> Ibrahim Barry</p>
                <p><strong>Vice-président :</strong> Abdoul Karim Camara</p>
                <p><strong>Secrétaire général :</strong> Mohamed N’kony Taboure</p>
                <p><strong>Trésorier :</strong> Amadou Bella Diallo</p>
                <p><strong>Notaire :</strong> Kay-Niklas Elsaesser, LL.M.</p>
            </div>
        </section>
        <section id="contact" class="section">
            <h2>Contactez-nous</h2>
            <p><strong>Adresse :</strong> Europa-Allee 1, 37079 Göttingen, Allemagne</p>
            <p><strong>E-mail :</strong> teamrgag@gmail.com</p>
        </section>
        <section id="donation" class="section">
            <h2>Faire un don</h2>
            <p>Vous pouvez soutenir nos projets en effectuant un don via notre compte bancaire :</p>
            <p><strong>Banque :</strong> Sparkasse Göttingen</p>
            <p><strong>IBAN :</strong> DE43 2605 000100561171 04</p>
        </section>
    </div>
    <footer>
        <p>&copy; 2025 AGAG e.V. Tous droits réservés.</p>
    </footer>
</body>
</html>
"""

# Save HTML to a file
output_file_path = "/mnt/data/AGAG_eV.html"
with open(output_file_path, "w") as file:
    file.write(html_content)

output_file_path
