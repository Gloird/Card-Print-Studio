# Card Print Studio 🃏🖨️

**Card Print Studio** est une application web moderne, légère et entièrement exécutée côté client (zéro serveur requis). Elle a été conçue pour simplifier la création, l'organisation, la mise en page et l'impression de **jeux de cartes personnalisés** (Poker, Bridge, Tarot ou formats sur mesure) avec une gestion intelligente du recto-verso (duplex).

👉 **Tester l'application en ligne :** [https://sites.google.com/view/cardprintstudio](https://sites.google.com/view/cardprintstudio)

---

## ✨ Fonctionnalités clés

* **🎴 Gestion dynamique des cartes** :
* Import en masse ou individuel d'images recto (PNG, JPG, WebP).
* Compteurs de quantité ajustables pour chaque carte.
* Association d'une image de dos globale ou personnalisée par carte (avec synchronisation automatique du nombre de dos pour correspondre exactement au nombre total de cartes recto).


* **📐 Formats & Dimensions flexibles** :
* Formats prédéfinis standards : *Poker* (63.5 x 88.9 mm), *Bridge*, *Mini/Euro*, *Tarot*.
* Dimensions personnalisées en millimètres (`mm`).
* Choix du format de page d'impression (A4, A3, Letter) en mode Portrait ou Paysage.


* **🔄 Support Duplex & Effet Miroir** :
* Options de retournement par bord long ou bord court.
* Inversion horizontale automatique (`scaleX(-1)`) des pages de dos pour garantir un alignement parfait recto-verso après l'impression et la découpe.


* **✂️ Outils de découpe professionnels** :
* Ajout optionnel de repères de coupe (crop marks).
* Guides de coins arrondis pour faciliter le découpage aux ciseaux ou au rognoir.
* Ajustement des marges de page et des espacements (gaps) entre les cartes.


* **📄 Double mode d'export & Impression** :
* **Impression directe** : Masquage automatique de l'interface via des règles CSS `@media print` pour imprimer uniquement les planches.
* **Export PDF haute résolution** : Génération directe d'un fichier PDF multi-pages (rectos puis versos) grâce à `jsPDF` et `html2canvas`.



---

## 🚀 Utilisation rapide

Aucune installation, compilation ou serveur backend n'est nécessaire. L'application fonctionne directement dans votre navigateur web.

1. Téléchargez ou clonez ce dépôt.
2. Ouvrez le fichier `index.html` dans un navigateur moderne (Chrome, Firefox, Edge, Safari).
*(Ou visitez directement le site hébergé : [sites.google.com/view/cardprintstudio](https://sites.google.com/view/cardprintstudio))*
3. Glissez-déposez vos images de cartes (recto) et définissez le nombre d'exemplaires souhaité.
4. Importez ou sélectionnez l'image de dos des cartes.
5. Ajustez les dimensions, les marges et les options de coupe selon vos préférences.
6. Prévisualisez le résultat en temps réel, puis lancez l'impression ou téléchargez le PDF !

---

## 🛠️ Stack Technique

* **HTML5 / CSS3** : Interface moderne et responsive propulsée par **Tailwind CSS**.
* **JavaScript (ES6+)** : Algorithmes de pagination, calculs de grille en `mm` / pixels, et gestion des fichiers locaux (File API / Drag & Drop).
* **Bibliothèques tierces** :
* [jsPDF](https://github.com/parallax/jsPDF) (Génération de documents PDF)
* [html2canvas](https://html2canvas.hertzen.com/) (Capture haute fidélité des planches de cartes)
* [Lucide Icons](https://lucide.dev/) (Icônes vectorielles épurées)



---

## 📂 Structure du projet

```text
card-print-studio/
│
├── index.html       # Application complète (code unique autonome)
├── README.md        # Documentation du projet
└── LICENSE          # Licence du projet (MIT)

```

---

## 🤝 Contribution

Les contributions, signalements de bugs et suggestions d'améliorations sont les bienvenus ! N'hésitez pas à ouvrir une *Issue* ou à proposer une *Pull Request*.

---

## 📄 Licence

Ce projet est sous licence [MIT](https://www.google.com/search?q=LICENSE). Vous êtes libre de l'utiliser, de le modifier et de le partager à des fins personnelles ou professionnelles.
