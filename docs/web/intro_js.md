# Introduction à Javascript


# Introduction au JavaScript pour débutants


## Les bases du langage

### Variables et types de données

```javascript
// Déclaration de variables
let nom = "Alice";  // chaîne de caractères
const age = 25;     // nombre
var estEtudiant = true;  // booléen

// Types de données
let nombre = 42;
let texte = "Bonjour";
let tableau = [1, 2, 3];
let objet = { cle: "valeur" };
```

### Opérateurs

```javascript
// Arithmétiques
let somme = 5 + 3;
let difference = 10 - 4;
let produit = 6 * 7;
let quotient = 15 / 3;
let resteDeLaDivision = 15 % 7;

// Comparaison
let estStrictementEgal = (5 === 5);  // true
let estStrictementDifferent = (4 !== 5) // true
let estPlusGrand = (10 > 5);  // true
let estInferieur = (5 < 10); // false
let estPlusGrandOuEgal =(10 >=  5) // true
let estPlusPetitOuEgal = (10 <= 5); // false
```

### Structures de contrôle

```javascript
// Condition if
if (age > 18) {
    console.log("Majeur");
} else if (age === 18) {
    console.log("nouveau majeur!");
} else {
    console.log("Mineur");
}

// Condition avec l'opérateur ternaire
const status = age >= 18 ? "majeur" : "mineur";


// Boucle for
for (let i = 0; i < 5; i++) {
    console.log(i);
}

// Boucle for ... of
const tableau = [123, 234, 345];
for (let element of tableau) {
    console.log(element);
}

// Boucle while
let compteur = 0;
while (compteur < 3) {
    console.log(compteur);
    compteur++;
}
```

### Fonctions
```javascript
function saluer(nom) {
    return "Bonjour, " + nom + " !";
}

console.log(saluer("Alice"));  // Affiche : Bonjour, Alice !
```

