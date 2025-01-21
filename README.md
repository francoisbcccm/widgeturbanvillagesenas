# Widget de Calcul de Financement

Ce projet est un widget interactif permettant de calculer les mensualités de financement pour des villas. Il inclut également des fonctionnalités visuelles ludiques, comme des feux d'artifice, et donne accès aux plans détaillés des villas.

## Fonctionnalités principales

- **Choix de la villa** : Sélectionnez parmi 24 modèles de villas, chacun avec son prix et un lien vers le plan détaillé.
- **Apport personnel** : Indiquez votre apport initial à partir d'une liste déroulante allant de 5 000 € à 4 000 000 €, par tranches de 5 000 €.
- **Durée du prêt** : Choisissez une durée de remboursement entre 5 et 25 ans.
- **Taux d'intérêt** : Sélectionnez un taux d'intérêt annuel entre 2 % et 4 %, par tranches de 0,05 %.
- **Résultat instantané** : Calcule les mensualités en fonction des paramètres sélectionnés.
- **Lien vers les plans des villas** : Affiche un bouton pour accéder au plan PDF de la villa choisie.
- **Animations visuelles** : Des feux d'artifice colorés apparaissent après chaque calcul.

## Démo en direct

Pour tester ce widget, ouvrez le fichier HTML dans n'importe quel navigateur moderne.

## Installation

1. Clonez ce dépôt ou téléchargez les fichiers.
2. Assurez-vous que les fichiers suivants sont présents :
   - `index.html` : Le fichier principal contenant le code du widget.
   - `Logotype-EXE.jpg` : Le logo utilisé dans le widget.
3. Placez les fichiers dans un dossier accessible.
4. Ouvrez `index.html` dans un navigateur pour commencer à utiliser le widget.

## Utilisation

1. Ouvrez le fichier `index.html`.
2. Dans le menu déroulant, sélectionnez la villa souhaitée.
3. Indiquez l'apport personnel, la durée du prêt et le taux d'intérêt.
4. Cliquez sur le bouton **Calculer** pour afficher les mensualités.
5. Cliquez sur le bouton **Découvrir les plans de la villa** pour accéder au plan PDF de la villa.

## Structure des données

Les informations des villas sont stockées dans une liste JavaScript :

```javascript
const villas = [
    { name: "G1", price: 298200, plan: "https://drive.google.com/uc?id=13KsO8flDQ0VeRAY5WwRfWRhSvzBYXRfr" },
    { name: "G2", price: 332000, plan: "https://drive.google.com/uc?id=1UMUdHQnXcP22yUEqNE27iy2snVV1-U3K" },
    // ... Ajoutez les autres villas ici
];
```

Chaque villa a :
- `name` : Nom ou modèle de la villa (ex : G1, G2).
- `price` : Prix de la villa.
- `plan` : Lien vers le plan détaillé en PDF.

## Fonctionnalités avancées

### Feux d'artifice
Les feux d'artifice s'affichent après chaque calcul réussi. Ils sont générés dynamiquement avec des couleurs et des mouvements aléatoires.

### Lien vers les plans
Chaque villa a un lien unique vers un fichier PDF hébergé sur Google Drive. Assurez-vous que les fichiers PDF sont publics pour que les utilisateurs puissent y accéder.

## Contribution

1. Forkez ce dépôt.
2. Créez une nouvelle branche :
   ```bash
   git checkout -b nouvelle-fonctionnalite
   ```
3. Apportez vos modifications et testez-les.
4. Commitez vos changements :
   ```bash
   git commit -m "Ajout d'une nouvelle fonctionnalité"
   ```
5. Poussez la branche :
   ```bash
   git push origin nouvelle-fonctionnalite
   ```
6. Créez une Pull Request.

## Auteurs

- **François Desreumaux** : Créateur et coordinateur du projet.

## Licence

Ce projet est sous licence MIT. Vous êtes libre de l'utiliser, de le modifier et de le redistribuer à condition de conserver cette notice.

---

### Remarques
- Vérifiez que les liens vers les fichiers PDF des villas fonctionnent correctement.
- Assurez-vous que le fichier `Logotype-EXE.jpg` est dans le même répertoire que le fichier HTML.

