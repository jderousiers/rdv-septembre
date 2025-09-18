<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Rendez-vous secret ❤️</title>
<style>
body {
margin: 0;
font-family: Arial, sans-serif;
background: #fafafa;
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
text-align: center;
}
#content {
display: none;
padding: 20px;
}
img {
width: 100%;
border-radius: 10px;
margin-bottom: 20px;
}
input {
padding: 10px;
font-size: 18px;
width: 120px;
text-align: center;
border: 1px solid #ccc;
border-radius: 6px;
}
button {
padding: 10px 15px;
font-size: 16px;
margin-left: 10px;
border: none;
border-radius: 6px;
background: #c62828;
color: #fff;
cursor: pointer;
}
h1 {
color: #c62828;
}
</style>
</head>
<body>
<div id="lock">
<div>
<p>Entrez le code secret 🔒</p>
<input type="password" id="password" maxlength="4">
<button onclick="checkPassword()">Valider</button>
</div>
</div>

<div id="content">
<img src="https://cdn.website.dish.co/media/f2/8d/6314864/LE-BOUILLON-LIMOUSIN-IMG-20230227-125229-jpg.jpg" alt="Restaurant Le Bouillon Limousin">
<h1>Rendez-vous ❤️</h1>
<p>Je t’invite au <strong>Bouillon Limousin</strong></p>
<p><strong>Date :</strong> 25 septembre</p>
<p><strong>Heure :</strong> 20h00</p>
<p>Hâte de partager ce moment avec toi ✨</p>
</div>

<script>
function checkPassword() {
const input = document.getElementById("password").value;
if (input === "1208") {
document.getElementById("lock").style.display = "none";
document.getElementById("content").style.display = "block";
} else {
alert("Code incorrect, essaie encore !");
}
}
</script>
</body>
</html>
