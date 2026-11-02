# 📒 Mon carnet de bord

**Nom :** 

**Prénom :** 

**Adresse de mon site :** https://______.pythonanywhere.com

> Modifiez ce fichier directement sur GitHub (icône crayon ✏️) pour répondre aux questions de chaque exercice.
> Écrivez avec vos propres mots : une réponse courte et juste vaut mieux qu'un long copier-coller ! 🙂

---

## 🟢 Exercice 1 — Mon premier déploiement

1. Où se trouve physiquement le code qui fabrique votre page : sur votre ordinateur, sur GitHub ou sur PythonAnywhere ?

  SurPythonAnywhere.

2. Pourquoi votre voisin(e) peut-il voir votre site, alors que vous n'avez rien installé sur son ordinateur ?

  Il est accessible par tout le monde car ...

---

## 🟢 Exercice 2 — Les URL et les routes

1. Dans l'URL `https://www.google.com/maps`, quel est le nom de domaine ? Quel est le chemin ?

   Nom de domaine : www.google.com
   Chemin: /maps 

2. Que veut dire le message *Not Found* ? Qui l'a envoyé : votre navigateur ou le serveur ?

   Le serveur qui envoie au navigateur

3. Que se passe-t-il si deux fonctions portent le même nom dans `flask_app.py` ? (Indice : essayez, puis lisez l'Error log.)

   La deuxième ecrase la première.

---

## 🔵 Exercice 3 — Le langage HTML

1. Quelle est la différence entre ce que le serveur **envoie** et ce que le navigateur **affiche** ?

  Le serveur envoie une réponse HTTP contenant des données (HTML, CSS, JavaScript, images, etc.).

Le navigateur affiche ces données en les interprétant pour les présenter sous forme de page web à l'utilisateur. 

2. À quoi servent les balises `<h1>`, `<p>`, `<ul>` et `<li>` ?

   <h1> : le titre
   <p> : paragraphe
   <ul> : liste non ordonné
   <li> : liste

3. Pourquoi l'image s'affiche-t-elle alors qu'elle n'est pas sur votre serveur ?

   Car l'image existe deja.

---

## 🔵 Exercice 4 — Les templates

1. Pourquoi est-ce une bonne idée de séparer le code Python et le HTML ? (Pensez à une équipe avec un développeur et un graphiste.)

  C'est une bonne idée de séparer le code Python et le HTML pour faciliter l'organisation, la maintenance et le travail en équipe.

   Par exemple :
   - Le développeur travaille sur le code Python (Flask), qui gère la logique et les données du site.
   - Le graphiste travaille sur le HTML et le CSS, qui gèrent la structure et l'apparence des pages.
   Ainsi, chacun peut travailler sur sa partie sans modifier le travail de l'autre.

2. Les `{{ prenom }}` sont-ils remplacés par le serveur ou par le navigateur ? Comment l'avez-vous vérifié ?

   Par le serveur, on peut les vérifier dans la page web et afficher le code source.

---

## 🔵 Exercice 5 — Le CSS et les liens

1. Quelle est la différence de rôle entre le HTML et le CSS ?

  HTML pour l'affichage des contenues des sites web (textes,images ect..) et le CSS son rôle est de styliser tout ca.

2. Pour afficher votre page `/presentation`, combien de fichiers le navigateur doit-il télécharger ? (Vous pourrez le vérifier à l'exercice suivant !)

   > _Ma réponse :_ 

3. Pourquoi faut-il parfois faire **Ctrl + F5** pour voir les changements de CSS ?

   Car il faut actualiser les changements pour voir les ajouts.

---

## 🟣 Exercice 6 — Espionner le navigateur

1. Que signifie HTTP ? Qui envoie la **requête** et qui envoie la **réponse** ?

  HYPEX TEXT TRANSFER PROTOCOL : la requête envoyé par le serveur qui répond.

2. Combien de requêtes votre page `/presentation` a-t-elle déclenchées ? Lesquelles ?

  2 : Présentation et style.css
3. Que signifie le code `200` ? Et le code `404` de la favicon ?

   Code 200 : OK
   Code 404 : le serveur a bien reçu la requête mais parvient pas à répondre à la demande.

4. Pourquoi les modifications faites dans l'onglet Éléments ne sont-elles pas visibles par les autres visiteurs ?

   Les modifications dans l'onglet Éléments sont visibles uniquement sur notre navigateur et ne sont pas enregistrées sur le serveur.

---

## 🟣 Exercice 7 — Envoyer des informations dans l'URL

1. Dans l'URL `https://www.youtube.com/results?search_query=chat`, quel est le nom du paramètre ? Quelle est sa valeur ?

   Nom : Search_queey 
   Valeur : chat

2. Pourquoi le serveur plante-t-il avec `a=bonjour` ? Que faudrait-il faire pour l'éviter ?

  Car il attend un nombre pour éviter cela il faut faire en sorte que le serveur attend un string

3. Pourquoi est-il dangereux d'afficher **tel quel** ce que l'utilisateur envoie ?

  Dangeureux en terme de confidentialité, tout le monde peut voir ce qu'il envoie.

---

## 🟣 Exercice 8 — Les formulaires

1. Quelle est la différence visible entre GET et POST ?

  Les données envoyées sont visibles dans l'URL pour GET et non POST

2. Pour un formulaire de **recherche**, quelle méthode choisiriez-vous ? Et pour un formulaire de **connexion avec mot de passe** ? Pourquoi ?

  Get pour recherche et POST pour le mot de passe car on veux pas que notre mot de passe apparaisse dans l'URL et la recherche n'est pas obligatoire.

3. Les données envoyées en POST sont-elles vraiment « secrètes » ? (Pensez à ce que vous avez vu dans l'onglet Réseau.)

   Elles peuvent être visible via l'onglet Network donc faut faire HTTPS.
---

## 🔴 Exercice 9 — Les codes de statut

1. Quelle est la différence entre une erreur `4xx` et une erreur `5xx` ? Qui est « fautif » dans chaque cas ?

   Erreur 4xx : erreur client
   Erreur 5xx : erreur serveur
2. Comment fonctionne une redirection ? Qui fait la deuxième requête : le serveur ou le navigateur ?

   Quand le serveur dis d'aller à une autre adresse URL et le navigateur fais la deuxième requête

3. Donnez un exemple de situation où un vrai site utilise une redirection.

   On arrive sur la page de connexion.
   On saisit son identifiant et son mot de passe.
   Après validation, le serveur vérifie les informations.
   Si elles sont correctes, le serveur redirige le navigateur vers la page d'accueil du compte utilisateur. 

---

## 🔴 Exercice 10 — Ce que le serveur sait de vous

1. Citez trois informations que le serveur connaît sur vous, sans que vous ayez rien rempli.

  Votre adresse IP : 86.247.171.252

Votre navigateur : Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/156.0.0.0 Safari/537.36

Vos langues : fr-FR,fr;q=0.9,en-US;q=0.8,en;q=0.7

2. À quoi peut servir l'en-tête `Accept-Language` pour un site comme Wikipédia ?
   Pour permettre à mettre pleins d'autres langues.

3. Dans l'Access log, retrouvez une requête qui a reçu un code `404`. Quelle page était demandée ?

   Style.css

4. Après cet exercice, que pensez-vous de la notion de « navigation anonyme » ?
   Elle permet de naviguer sur le web sans que les données soient enregistrés mais on reste quand meme visible par le fournisseur , l'entreprise...

---

## 🔴 Exercice 11 — Le Web des machines : API et JSON

1. Quelle est la différence entre une page HTML et une réponse JSON ? À qui chacune est-elle destinée ?

   > _Ma réponse :_ 

2. Dans la page `/horloge`, quel code s'exécute sur le **serveur** et quel code s'exécute dans le **navigateur** ?

   > _Ma réponse :_ 

3. Citez une application de votre téléphone qui, selon vous, utilise une API. Quelles données échange-t-elle ?

   > _Ma réponse :_ 

---

## 🏁 Pour conclure

En quelques phrases, expliquez à un ami ce qui se passe entre le moment où il tape une adresse dans son navigateur et celui où la page s'affiche :

> _Ma réponse :_ 
