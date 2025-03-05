<!DOCTYPE html>
<html lang="ca">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Reduïm el malbaratament alimentari per un món més sostenible">
    <title>Alimentació Sense Desperdici</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; text-align: center; background-color: #f4f4f4; }
        header { background: #4CAF50; color: white; padding: 20px; font-size: 28px; font-weight: bold; }
        nav { background: #2E7D32; padding: 15px; }
        nav a { color: white; margin: 0 20px; text-decoration: none; font-size: 18px; font-weight: bold; transition: 0.3s; cursor: pointer; }
        nav a:hover { text-decoration: underline; }
        .menu-icon { display: none; font-size: 24px; cursor: pointer; }
        .menu { display: flex; justify-content: center; flex-wrap: wrap; }
        section { padding: 40px; max-width: 800px; margin: auto; background: white; margin-top: 20px; border-radius: 10px; box-shadow: 0px 0px 10px rgba(0,0,0,0.1); display: none; }
        footer { background: #4CAF50; color: white; padding: 15px; font-size: 14px; margin-top: 20px; }
        img { max-width: 100%; height: auto; border-radius: 8px; margin-bottom: 20px; }
        @media (max-width: 768px) {
            .menu { display: none; flex-direction: column; }
            .menu a { padding: 10px; display: block; }
            .menu-icon { display: block; }
        }
    </style>
    <script>
        function toggleSection(id) {
            var section = document.getElementById(id);
            if (section.style.display === "none" || section.style.display === "") {
                section.style.display = "block";
            } else {
                section.style.display = "none";
            }
        }
    </script>
</head>
<body>
    <header>
        Alimentació Sense Desperdici
        <p>Reduïm el malbaratament alimentari per un món més sostenible</p>
    </header>
    <nav>
        <span class="menu-icon" onclick="toggleMenu()">☰</span>
        <div class="menu">
            <a onclick="toggleSection('inici')">Inici</a>
            <a onclick="toggleSection('necessitat')">Necessitat</a>
            <a onclick="toggleSection('problema')">El Problema</a>
            <a onclick="toggleSection('solucio')">Solució</a>
            <a onclick="toggleSection('beneficis')">Beneficis</a>
            <a onclick="toggleSection('colaboracions')">Col·laboracions</a>
            <a onclick="toggleSection('ganxo')">Ganxo</a>
            <a onclick="toggleSection('contacte')">Contacte</a>
        </div>
    </nav>
    <section id="inici">
        <h2>Benvinguts a Alimentació Sense Desperdici</h2>
        <p>Som un grup d'alumnes de l'INS Abat Oliba de Ripoll: Alan, Gil, Àlex i Santi. El nostre projecte té com a objectiu conscienciar la gent sobre el malbaratament alimentari i com podem reduir-lo per construir un futur més sostenible.</p>
    </section>
    <section id="problema">
        <h2>📉 El Problema</h2>
        <p>Milions de tones d'aliments es llencen cada any arreu del món. Això no només suposa una pèrdua econòmica, sinó que també contribueix a l'augment de la fam mundial i el deteriorament del medi ambient. Quan es llença menjar, també es malgasten els recursos naturals com l'aigua i l'energia utilitzats per produir-lo.</p>
        <img src="https://residus.gencat.cat/web/.content/home/ambits_dactuacio/prevencio/setmana_europea_prevencio_de_residus/dies_tematics/2024/EWWR_2024_Factsheet1_Reducing_food_waste_EU.pdf" alt="Gràfic sobre el malbaratament alimentari">
    </section>
    <section id="contacte">
        <h2>📩 Contacte</h2>
        <p>Si vols saber més sobre el nostre projecte, envia’ns un missatge!</p>
        <form>
            <label for="nom">Nom:</label><br>
            <input type="text" id="nom" name="nom" required><br><br>
            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email" required><br><br>
            <label for="missatge">Missatge:</label><br>
            <textarea id="missatge" name="missatge" rows="4" required></textarea><br><br>
            <button type="submit">Enviar</button>
        </form>
    </section>
    <footer>
        &copy; 2025 Alimentació Sense Desperdici - Per un futur sostenible
    </footer>
</body>
</html>
