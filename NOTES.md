# Notes d’intégration

- Ajout de `#fond-anime`, conteneur fixe dédié, non interactif, derrière le contenu.
- Remplacement du prototype injecté dans `body` par un module/IIFE isolé dans `script.js`.
- Correction de la référence `element` non déclarée qui interrompait l’initialisation du formulaire.
- Suppression des codes couleur invalides : les emojis sont affichés tels quels.
- Animation basée sur `translate3d` jusqu’à `110vh`, avec suppression via `animationend`.
- Un seul intervalle, plafonné à 34 éléments simultanés, et arrêt/reprise avec `document.hidden`.
- Désactivation avec `prefers-reduced-motion` et allègement sur petits écrans.
- Alignement du formulaire sur l’identifiant conventionnel `#rsvp-form` attendu par le moteur (sans doublon).
- Aucun autre identifiant métier ni classe existante modifié ; les guides (`z-index: 5`), le bouton skip (`z-index: 10`) et le moteur de formulaire restent prioritaires.
- Le `body` conserve son comportement de défilement : aucune hauteur fixe ni `overflow: hidden` n’a été ajouté.
