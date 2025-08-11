# ksawrld.github.io
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Défi - Lettre du mot secret</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #111; color: white; padding: 50px; }
        input { padding: 10px; font-size: 16px; margin-top: 20px; width: 250px; text-align: center; }
        button { padding: 10px 15px; font-size: 16px; background: #ff4757; border: none; color: white; cursor: pointer; }
        #secret { display: none; margin-top: 20px; font-size: 22px; color: #2ed573; }
    </style>
</head>
<body>
    <h1>🔍 Trouve la lettre du mot secret</h1>
    <p>Question : Spécialité culinaire de Meaux<br>Je suis un fromage crémeux, fabriqué près de la Seine.<br>On me nomme d’après ma ville, célèbre pour mon goût délicat.<br>Je suis souvent servi en dessert ou lors des repas gourmands.</p>
    
    <input type="text" id="answer" placeholder="Réponse...">
    <button onclick="checkAnswer()">Valider</button>
    
    <div id="secret">✅ La/les lettre(s) à garder est/sont : <b>VA</b></div>

    <script>
        function checkAnswer() {
            let input = document.getElementById("answer").value.trim().toLowerCase();
            let correctAnswer = "brie de meaux"; // ✅ Bonne réponse

            if (input === correctAnswer) {
                document.getElementById("secret").style.display = "block";
            } else {
                alert("Mauvaise réponse ❌");
            }
        }
    </script>
</body>
</html>
