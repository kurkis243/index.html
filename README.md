# index.html
<!DOCTYPE html>
<html lang="sk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minikurz: Ako si určiť ciele a konečne ich splniť</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
            padding: 0;
            background: #f4f4f4;
            color: #333;
        }
        h1, h2 {
            color: #2c3e50;
        }
        .section {
            background: #fff;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.05);
        }
        button {
            margin-top: 10px;
        }
        .quiz {
            margin-top: 10px;
        }
    </style>
</head>
<body>

    <div class="section">
        <h1>Vitaj v minikurze!</h1>
        <p>Cieľ: Pomôcť ti jasne si určiť ciele a konečne ich splniť. Kurz trvá približne 1 hodinu a je rozdelený na viacero častí.</p>
    </div>

    <div class="section">
        <h2>1. Prečo si stanoviť ciele?</h2>
        <p>Bez cieľov nemáme smer. Ciele nám dávajú motiváciu, zmysel a pomáhajú nám rásť. Predstav si, aké by to bolo, keby si mal jasný plán a vedel, čo chceš dosiahnuť.</p>
    </div>

    <div class="section">
        <h2>2. SMART ciele</h2>
        <p>SMART je skratka pre:</p>
        <ul>
            <li><strong>S</strong> - špecifický</li>
            <li><strong>M</strong> - merateľný</li>
            <li><strong>A</strong> - dosiahnuteľný</li>
            <li><strong>R</strong> - relevantný</li>
            <li><strong>T</strong> - časovo ohraničený</li>
        </ul>
    </div>

    <div class="section quiz">
        <h2>Mini kvíz</h2>
        <p>Čo znamená „A“ v SMART?</p>
        <input type="text" id="answer1" placeholder="Tvoja odpoveď">
        <button onclick="checkAnswer()">Skontrolovať</button>
        <p id="result1"></p>
    </div>

    <div class="section">
        <h2>3. Rozdelenie cieľov na kroky</h2>
        <p>Každý veľký cieľ si rozdeľ na menšie časti. Takto nebudeš preťažený a budeš vidieť postup.</p>
    </div>

    <div class="section">
        <h2>4. Akčný plán</h2>
        <p>Napíš si: <br>
        - čo chceš dosiahnuť<br>
        - prečo to chceš<br>
        - do kedy<br>
        - konkrétne kroky</p>
    </div>

    <div class="section">
        <h2>5. Záver</h2>
        <p>Gratulujem! Teraz máš základný plán a vieš, ako si nastaviť reálne a dosiahnuteľné ciele. Začni ešte dnes!</p>
    </div>

    <script>
        function checkAnswer() {
            const answer = document.getElementById("answer1").value.toLowerCase();
            const result = document.getElementById("result1");
            if (answer.includes("dosiahnuteľný") || answer.includes("dosiahnutelny")) {
                result.textContent = "Správne!";
                result.style.color = "green";
            } else {
                result.textContent = "Nesprávne. Skús to ešte raz.";
                result.style.color = "red";
            }
        }
    </script>

</body>
</html>
