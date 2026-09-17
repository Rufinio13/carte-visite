# cartes-contact

Dépôt GitHub Pages regroupant les cartes de contact digitales (QR code) de l'équipe.

## Structure

```
cartes-contact/
├── README.md
├── .gitignore
├── assets/                     ← logos/photos communs (optionnel)
│   └── logo-naturea.png
└── raphael-evariste/
    └── index.html               ← carte de Raphaël (une page par personne)
```

Chaque nouvel employé = un nouveau dossier `prenom-nom/` contenant son propre
`index.html`. Pas d'autre fichier requis pour que GitHub Pages fonctionne.

Une fois le dépôt en ligne (Settings > Pages > Deploy from a branch > main > /root),
chaque carte sera accessible à :

```
https://<ton-pseudo-github>.github.io/cartes-contact/raphael-evariste/
https://<ton-pseudo-github>.github.io/cartes-contact/prenom-nom/
```

## Pour ajouter Raphaël

Colle dans `raphael-evariste/index.html` le contenu du fichier HTML autonome
("naturea-carte-contact-standalone.html") déjà généré précédemment — celui
avec les liens mail/tél standards et le bouton "Ajouter aux contacts" qui
fonctionne sans dépendre de claude.ai.

## Pour ajouter une nouvelle personne

1. Copie le dossier `raphael-evariste/` et renomme-le `prenom-nom/`
2. Dans son `index.html`, remplace : nom, poste, téléphone, email, photo,
   liens réseaux sociaux et la vCard générée par le bouton "Ajouter aux contacts"
3. Commit + push
4. Le lien final me sera transmis pour générer le QR code correspondant
