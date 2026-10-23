# Atelier pratique HTML

**Construction de la structure du site vitrine « Le Petit Bistro »**

*Phase 1 · Construire et publier un site web interactif — Document 2 / 3 · Atelier pratique*

> **Prérequis :** avoir réalisé le Sujet de veille (Document 1).
> **Durée :** 2 journées · **Modalité :** travail individuel, entraide autorisée.
> **Production attendue :** un dossier `petit-bistro` contenant deux pages HTML valides : `index.html` (accueil) et `contact.html`.
> **Règle :** aucun CSS dans cet atelier. On construit d'abord le contenu et la structure.

---

## PARTIE 1 : L'environnement de travail et le squelette de la page

**Objectif :** installer les outils du développeur, organiser les fichiers du projet et créer une première page HTML valide affichée dans le navigateur.

### 1. Installation et organisation :

a. Installez l'éditeur **Visual Studio Code** et l'extension **Live Server**. À quoi sert cette extension ?

b. Créez l'arborescence suivante et expliquez le rôle du dossier `images` :

```
petit-bistro/
├── index.html
├── contact.html
└── images/
```

### 2. Le squelette :

a. Dans `index.html`, écrivez la structure minimale d'une page HTML en français.

b. Donnez à la page le titre « Le Petit Bistro – Cuisine maison ». Où ce titre apparaît-il dans le navigateur ?

c. Ajoutez la balise qui garantit un bon affichage sur téléphone.

d. Ouvrez la page avec Live Server. Expliquez ce que vous voyez et pourquoi la page est encore vide.

> **Mission de recherche :** trouvez le raccourci de VS Code qui génère automatiquement le squelette d'une page HTML. Comparez le code produit avec le vôtre : quelles différences remarquez-vous ?

---

## PARTIE 2 : La page d'accueil

**Objectif :** structurer la page d'accueil en zones sémantiques et y intégrer les contenus du restaurant : textes, images, liens, listes et tableau.

### 1. Le découpage en zones :

a. Dessinez sur papier la maquette de la page avec ses zones : en-tête, navigation, contenu principal (trois sections), pied de page.

b. Traduisez cette maquette en balises sémantiques dans le `<body>`. Pourquoi ne pas utiliser uniquement des `<div>` ?

### 2. L'en-tête et la navigation :

a. Dans le `<header>`, ajoutez le logo (image) et le nom du restaurant en titre principal.

b. Créez un menu de navigation sous forme de **liste de liens** : « Présentation », « La carte », « Horaires », « Contact ».

c. Les trois premiers liens doivent mener à une section de la même page. Recherchez comment fonctionnent les **ancres** (attribut `id` et lien `href="#..."`) et appliquez-les.

d. Le lien « Contact » mène vers `contact.html`. S'agit-il d'un chemin relatif ou absolu ?

### 3. Section « Présentation » :

a. Ajoutez un titre de niveau 2 et deux paragraphes qui présentent le restaurant (histoire, cuisine, ambiance).

b. Mettez en valeur un mot important avec la balise adaptée.

c. Insérez une photo de la salle. Rédigez un texte alternatif utile. Qu'est-ce qu'un « bon » texte alternatif ?

### 4. Section « La carte » :

a. Organisez la carte en trois catégories (entrées, plats, desserts), chacune avec un titre de niveau 3.

b. Sous chaque catégorie, listez au moins trois plats avec leur prix. Quel type de liste avez-vous choisi et pourquoi ?

c. Vérifiez la hiérarchie des titres : h1 → h2 → h3. Expliquez pourquoi on ne saute pas de niveau.

### 5. Section « Horaires » :

a. Présentez les horaires d'ouverture de la semaine dans un **tableau** avec une ligne d'en-tête (jour, midi, soir).

b. Quel est le rôle des balises `<thead>`, `<tbody>`, `<th>` et `<td>` ?

### 6. Le pied de page :

a. Ajoutez l'adresse du restaurant dans la balise sémantique prévue pour les coordonnées.

b. Créez un lien qui **appelle** le restaurant au clic sur téléphone, et un lien qui ouvre un **e-mail**.

c. Ajoutez un lien vers le plan d'accès qui s'ouvre dans un nouvel onglet. Quel attribut faut-il ajouter ?

---

## PARTIE 3 : La page contact et le formulaire de réservation

**Objectif :** créer une deuxième page reliée à la première et construire un formulaire de réservation complet et accessible.

### 1. La page contact :

a. Créez `contact.html` en réutilisant le même en-tête, la même navigation et le même pied de page que l'accueil.

b. Adaptez les liens de navigation pour qu'ils ramènent aux sections de `index.html`.

### 2. Le formulaire de réservation :

a. Créez un formulaire contenant les champs suivants, chacun avec son `<label>` :

- nom complet et adresse e-mail (obligatoires) ;
- numéro de téléphone ;
- date et heure souhaitées ;
- nombre de personnes, de 1 à 12 ;
- motif de la demande dans une liste déroulante : réservation, question, événement privé ;
- message libre sur plusieurs lignes ;
- case à cocher « J'accepte d'être recontacté » ;
- bouton « Envoyer la demande ».

b. Pour chaque champ, justifiez le **type** choisi. Quel avantage apporte `type="email"` sur téléphone ?

c. Recherchez les attributs qui limitent le nombre de personnes entre 1 et 12, et appliquez-les.

d. Testez : essayez d'envoyer le formulaire vide, puis avec un e-mail invalide. Décrivez la réaction du navigateur.

> **Mission de recherche :** recherchez les balises `<fieldset>` et `<legend>`. Utilisez-les pour regrouper les champs « Vos coordonnées » et « Votre réservation ». Qu'apportent-elles à un utilisateur de lecteur d'écran ?

---

## PARTIE 4 : Le contrôle qualité

**Objectif :** vérifier, comme un professionnel, que les pages sont valides, accessibles et bien structurées avant de les livrer.

1. **Validation :** passez vos deux pages dans le validateur du W3C. Corrigez toutes les erreurs et expliquez les trois plus fréquentes que vous avez rencontrées.
2. **Navigation au clavier :** parcourez vos pages uniquement avec la touche **Tab**. Peut-on atteindre tous les liens et tous les champs du formulaire ?
3. **Inspection :** ouvrez les outils de développement du navigateur (F12), onglet « Éléments ». Retrouvez l'arborescence de votre page et expliquez ce que vous observez.
4. **Relecture :** échangez votre projet avec un autre apprenant. Chacun note trois points forts et trois améliorations sur le travail de l'autre.

---

> **Suite :** conservez votre dossier `petit-bistro`. Dans la **Mise en situation professionnelle (Document 3)**, vous l'utiliserez pour réaliser seul le site d'un nouveau client et serez évalué sur ce travail.
