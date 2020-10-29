# Lionalfa.github.io<!DOCTYPE html>
<html>
  <head>
	<button>Connexion</button>
	<link href="https://fonts.googleapis.com/css2?family=Italianno&family=Open+Sans&display=swap" rel="stylesheet">
	<link href="styles/style.css" rel="stylesheet" type="text/css">
	<meta charset="utf-8">
    <title>Alfa Romeo Giulia</title>
  </head>
  <body>
	
	<h1>Alfa Romeo Giulia Gta</h1>
    <img src="images/firefox-icon.png" alt="Mon image de test">
	<p> La <strong>Giulia</strong> est une berline produite par le constructeur automobile italien Alfa Romeo. Remplaçante de la berline 159, 
	dont la production a été arrêtée à l'automne 20111, la Giulia est dévoilée le 24 juin 2015 à l'occasion du 105e anniversaire de la marque2,3 à l'usine d'Arese où se trouve le musée Alfa Romeo,
	en version sportive <strong>Quadrifoglio Verde</strong> (QV). 
	Le reste de la gamme a été présenté au Salon international de l'automobile de Genève début mars 2016.</p><br>
	
	
	<a href="https://www.alfaromeo.fr/">La Meccanica delle emozioni</a>
	

    <script src="scripts/main.js"></script>
 </body>
</html> html {
  font-size: 0px;
  font-family: 'Open Sans', sans-serif;
}
h1 {
  font-family: 'Italianno', cursive;
  font-size: 60px;
  text-align: center;
  color: red;
  margin: 0 auto;
  text-shadow: 2px 2px 1px black;let myImage = document.querySelector('img');

myImage.addEventListener('click', function() {
    let mySrc = myImage.getAttribute('src');
    if (mySrc === 'images/firefox-icon.png') {
      myImage.setAttribute('src', 'images/firefox2.png');
    } else {
      myImage.setAttribute('src', 'images/firefox-icon.png');
    }
});

let myButton = document.querySelector('button');
let myHeading = document.querySelector('h1');

function setUserName() {
  let myName = prompt('Entrer votre Nom.');
  localStorage.setItem('nom', myName);
  myHeading.textContent = 'Bienvenu, ' + myName;
}

if (!localStorage.getItem('nom')) {
  setUserName();
} else {
  let storedName = localStorage.getItem('nom');
  myHeading.textContent = 'Bienvenu, ' + storedName;
}


myButton.addEventListener('click', function() {
  setUserName();
});
}

a {
  font-family: 'Italianno', cursive;
  font-size: 30px;    
  line-height: 2;
  letter-spacing: 1px;
  color: red;
}

html {
  background-color: #010101;
}

body {
  width: 1000px;
  margin: 0px auto;
  background-color: #585858;
  padding: 0px 20px 20px;
  border: 3px solid green;
}


img {
  
  width: 1000px;
  display: block;
  margin: 0px auto;
}

p {
	font-size: 13px;
	width: 800px;
	color: white;
}

strong {
		color: green;
