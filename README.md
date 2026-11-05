# Automatismes Profs · Projeter des questions d'automatismes en classe

Console du professeur : choisissez le niveau (6e à 3e) ou les tables de multiplication, et projetez au tableau des questions d'automatismes avec correction. Sans compte, rien ne quitte l'appareil.

🔗 **Utiliser en ligne :** https://auriaphilippe.forge.apps.education.fr/Automatisme_Profs/
📄 Licence [GNU GPL v3](LICENSE) · 📜 [Nouveautés](CHANGELOG.md) · 🛡️ [Sécurité](SECURITY.md) · ♿ [Accessibilité](accessibilite.html)

## Pour quoi faire ?

Proposer en début de séance des questions d'automatismes (calcul mental, figures, tableaux, graphiques) à projeter au tableau, avec correction, chronomètre et bilan de fin de séance, du niveau 6e au niveau 3e. Un mode « Tables » entraîne les multiplications de 1 à 15.

## Pour qui ?

Les professeurs de mathématiques de collège (classe entière, vidéoprojecteur ou TNI).

## Comment l'utiliser

1. Ouvrez la page en ligne (rien à installer, pas de compte).
2. Choisissez le niveau (ou « Tables ×»), le nombre de questions, les thèmes et, si vous le souhaitez, un compte à rebours par question.
3. Cliquez sur « Commencer la séance » : les questions défilent, « Corriger » affiche la réponse, « Suivant » passe à la suite.
4. À la fin, le bilan reprend toutes les questions avec leur correction.

Pour l'utiliser hors ligne, téléchargez le dépôt et ouvrez `index.html` dans un navigateur : aucune dépendance, aucune connexion nécessaire.

## Fonctionnalités

- Niveaux 6e, 5e, 4e et 3e, avec choix des thèmes et sous-thèmes.
- Mode « Tables de multiplication » de 1 à 15.
- Questions générées au hasard à chaque séance, sans doublon.
- Figures, tableaux et graphiques générés en SVG.
- Compte à rebours avec pause, plein écran, formats 16:9 et 4:3.

## Données et vie privée

Aucun compte, aucun cookie, aucune mesure d'audience, aucun serveur. Le navigateur garde uniquement le thème clair ou sombre et le format d'affichage (clés `autodnb-profs-theme` et `autodnb-profs-format`) sur l'appareil. Rien n'est envoyé sur le réseau. Aucune donnée personnelle d'élève n'est traitée. Pour tout effacer, supprimer les données du site dans le navigateur.

## Accessibilité

**Accessibilité : non conforme** (aucun audit réalisé). Les contenus connus comme non accessibles sont listés dans la [déclaration d'accessibilité](accessibilite.html), avec les pistes d'amélioration.

## Sécurité

Aucune bibliothèque ni police chargée depuis un site tiers, aucune requête réseau, pas d'`eval`. Le détail, les limites de GitLab Pages et la façon de signaler une faille sont dans [SECURITY.md](SECURITY.md).

## Lancer en local / publier

- En local : ouvrir `index.html` dans un navigateur.
- Publication : GitLab Pages, via `.gitlab-ci.yml`, à chaque envoi sur la branche `main`. Aucune étape de construction.

## Architecture

```text
index.html             L'application (un seul fichier)
mentions-legales.html  Mentions légales
accessibilite.html     Déclaration d'accessibilité
assets/favicon.svg     Icône
assets/fonts/          Polices Syne et DM Sans (.woff2) et leur licence OFL
LICENSE                Licence GNU GPL v3
SECURITY.md            Sécurité
CHANGELOG.md           Historique des versions
.gitlab-ci.yml         Publication GitLab Pages
```

## Contribuer

- Signaler une erreur ou proposer une idée : [ouvrir un ticket](https://forge.apps.education.fr/auriaphilippe/Automatisme_Profs/-/issues).
- Proposer une modification : fourche du dépôt, puis demande de fusion.
- Règles : le français est la langue du projet (interface, commentaires, messages de commit) ; aucune dépendance externe ; tester l'application avant de proposer une modification.

## Crédits

- Les générateurs de questions sont écrits par l'auteur ; ils s'inspirent des programmes officiels, des ressources Éduscol « Les automatismes au collège » et des sujets du DNB publiés par le ministère.
- Polices **Syne** (© The Syne Project Authors) et **DM Sans** (© The DM Sans Project Authors), licence SIL Open Font License 1.1, voir `assets/fonts/`.
- Conçu par Philippe Auria, Collège Fernand Donatien, Fort-de-France.

## Licence

Logiciel libre sous licence [GNU GPL v3](LICENSE).
