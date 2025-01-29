  Justification Technique du Projet HTML/CSS avec Git

  1. Workflow Git et Gestion des Branches

Pour assurer une bonne organisation du projet et faciliter la collaboration, nous avons suivi un workflow Git basé sur des branches dédiées :
- Main : Branche principale contenant la version finale et stable du projet.
- Feature-1 : Branche dédiée au développement de la Hero Section.
- Feature-2 : Branche dédiée au bouton stylisé.

  Processus de développement Git
1. Initialisation du dépôt : `git init`
2. Création de la branche `feature-1` et ajout de la Hero Section :
   ```bash
   git checkout -b feature-1
   # Ajout des fichiers et commit
   git add .
   git commit -m "Ajout de la Hero Section"
   ```
3. Création de la branche `feature-2` et ajout du bouton stylisé :
   ```bash
   git checkout -b feature-2
   # Ajout du bouton et commit
   git add .
   git commit -m "Ajout du bouton stylisé"
   ```
4. Fusion des branches dans `main` pour intégrer les fonctionnalités :
   ```bash
   git checkout main
   git merge feature-1
   git merge feature-2
   ```

### 2. **Choix Techniques en HTML & CSS**

- HTML :
  - Une structure simple avec une section `hero` contenant un titre et un bouton.
  - Respect des bonnes pratiques en HTML5.

- CSS :
  - Utilisation de `display: flex` pour centrer le contenu.
  - Utilisation d’un `background-color` pour la mise en avant de la section Hero.
  - Effet `hover` sur le bouton pour améliorer l’expérience utilisateur.

### 3. Pourquoi ce Workflow ?

- Modularité : Chaque fonctionnalité est développée séparément pour éviter les conflits.
- Clarté : Les branches spécifiques permettent un suivi aisé des modifications.
- Facilité de collaboration** : Permettrait à plusieurs développeurs de travailler sur différentes fonctionnalités sans interférer.

### Conclusion

Le projet respecte une bonne organisation en suivant un workflow Git bien structuré. 
L’utilisation de branches dédiées a permis de garantir un développement fluide et modulaire, facilitant l’intégration progressive des fonctionnalités.

