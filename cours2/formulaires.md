
<html>
<head>
	
	<meta charset="UTF-8">
	<style>
		body{background-color:#E1D5D2;}
		h1{color:#9C370E;}
		fieldset {
			border:#000000 dotted 1px;
			border-radius: 10px;
			background-color:#FAF9F2;
			width:500px;
		}
		legend{
			font-style: bold;
		}
		.obligatoire {
			color:#FF0000;
		}
	</style>
</head>
<body>
<h1>Les formulaires</h1>
<p>La balise du formulaire c'est la balise &lt;form&gt;, qui est une balise ouvrante fermante. 
<form method="post" action="http://portail.jacquenod.net/Prog/capteur.php" target="_blank">

<fieldset><legend>Identité</legend>
<p><label for="Fname">Nom <sup class="obligatoire">*</sup></label><input type="text" name="Nom" id="Fname" required="required"></p>
<p><label for="Lname">Prénom <sup class="obligatoire">*</sup></label><input type="text" name="Nom" id="Lname" required></p>
<p>Quel est votre âge</p>
<p><input type="radio" name="age" value="18-30">Entre 18 et 30 ans<br>
<input type="radio" name="age" value="31-50">Entre 31 et 40 ans<br>
<input type="radio" name="age" value="51-60">Entre 51 et 60 ans<br>
<input type="radio" name="age" value="Plus de 61">Plus de 60 ans<br>
</p>
<p>Les langues parlées</p>
<select name="langue" multiple="multiple" size="2">
	<option value="anglais" selected="selected">Anglais</option>
	<option value="français">Français</option>
	<option value="espagnol">Espagnol</option>
	<option value="japonais">Japonais</option>
	<option value="italien">Italien</option>
	<option value="arabe">Arabe</option>
</select>
<p class="obligatoire">* cet élément est obligatoire</p>
<p>Quelques zones de saisie enrichies</p> <!--PAS ECRIT DANS LE COURS-->
<p>Couleurs <input type="color" name="couleur"></p>
<p>Email <input type="email" name="email"></p>
<p>Votre site web <input type="url" name="url"></p>
<p>Votre téléphone <input type="tel" name="tel" placeholder="+33000000000"></p>


</fieldset>

<fieldset><legend>Production</legend>
<p>Quelle est votre destination préférée en vacances</p>
<p><label for="Mer">Mer</label>
<input type="checkbox" name="Mer" id="Mer"><br>
<label for="Montagne">Montagne</label>
<input type="checkbox" name="Montagne" id="Montagne"><br>
<label for="Maison avec chat">Maison avec chat</label>
<input type="checkbox" name="Maison avec chat" id="Maison avec chat"><br>
<label for="Mon lit">Mon lit</label>
<input type="checkbox" name="Mon lit" id="Mon lit">
</p>
<p>
Laissez-nous un commentaire</p>
<textarea name="commentaire" rows="6" cols="50" placeholder="Ajouter un texte"></textarea>
<p>
J'accepte les conditions d'utilisation suivantes</p>
<textarea name="CGV" rows="6" cols="50" readonly="readonly">text only....</textarea><!--on peut pas modifier ce qu'il y'a dedans-->
</fieldset>

<input type="submit" name ="envoyer" value="send">
</form>
</p>
</body>
</html>
