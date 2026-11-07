# Okane, ton carnet de comptes

Une appli de budget perso inspirée de la méthode kakeibo. Elle fonctionne sans compte, sans pub et sans connexion. Toutes tes données restent sur l'appareil où tu l'utilises.

## Ce qu'elle fait

- Saisie rapide au pavé numérique : montant, catégorie (les plus utilisées en premier), compte choisi parmi tes cartes, Aujourd'hui ou Hier en un geste.
- Opérations récurrentes et abonnements : ils s'ajoutent tout seuls chaque mois, avec le total mensuel et annuel de tes abonnements. Plus de 80 services connus (streaming, musique, opérateurs, salles de sport, énergie…) à choisir dans une liste avec recherche.
- Reste à vivre du mois (revenus − épargne prévue − dépenses), montant par jour restant, opérations à venir.
- Jour de début du mois budgétaire réglable (par exemple du 25 au 24 si ton salaire tombe le 25).
- Calendrier du mois : intensité des dépenses par jour, plus grosses dépenses, revenus, jours sans dépense.
- Budgets par catégorie avec alerte de dépassement.
- Objectifs d'épargne avec jauge, échéance et montant à mettre de côté par mois (suivi manuel, ou lié au solde de comptes).
- Patrimoine : tes comptes sous forme de cartes bancaires dans un carrousel animé (couleur, motif et image au choix, aperçu en direct qui s'incline au doigt), total et courbe sur 12 mois. Plus de 45 banques, néobanques, courtiers et plateformes crypto à choisir dans une liste.
- Images perso : ajoute une image de ta photothèque sur n'importe quel compte ou abonnement, elle remplace les initiales.
- Mode voyage : les dépenses sont étiquetées automatiquement et chaque voyage a son propre budget (option pour le sortir du budget mensuel).
- Bilan du mois avec les 4 questions du kakeibo, répartition Besoins / Envies / Culture / Imprévus et dépenses des 6 derniers mois.
- Sauvegarde et changement de téléphone : export et restauration d'un fichier qui contient tout (images comprises), envoi par AirDrop ou iCloud Drive, export des opérations en CSV.
- Animations : transitions entre les pages, jauges et courbes qui se dessinent, montants qui défilent, feuilles qu'on ferme en les glissant vers le bas. Elles se coupent si « Réduire les animations » est activé sur l'iPhone.
- Mode sombre automatique, et l'appli fonctionne hors ligne une fois installée.

## Sur le Mac

Double-clique sur `index.html` : l'appli s'ouvre dans ton navigateur et tes données sont enregistrées dans ce navigateur.

## Sur l'iPhone

Un iPhone ne sait pas ouvrir une appli web depuis un simple fichier. Il faut la charger une fois depuis une adresse https. Ensuite elle s'installe sur l'écran d'accueil et marche hors ligne. Seul le code est en ligne : tes données restent sur le téléphone.

Avec GitHub Pages, c'est gratuit et ça prend environ 5 minutes. Utilise un compte **perso**, pas celui du travail.

1. Crée un compte gratuit sur github.com avec ton adresse mail perso.
2. Clique sur **New repository**, nomme-le `okane`, laisse-le en **Public**, puis **Create repository**.
3. Clique sur **uploading an existing file**, puis glisse dedans tout le contenu du dossier : `index.html`, `manifest.webmanifest`, `sw.js` et le dossier `icons`. Valide avec **Commit changes**.
4. Va dans **Settings → Pages**. Choisis Source : *Deploy from a branch*, branche `main`, dossier `/ (root)`, puis **Save**.
5. Après une minute environ, ton appli est disponible à l'adresse `https://TON-PSEUDO.github.io/okane/`.
6. Sur l'iPhone, ouvre cette adresse dans **Safari**, touche **Partager** puis **Sur l'écran d'accueil**, et valide avec **Ajouter**.
7. Ouvre Okane **depuis l'icône** et fais la configuration de départ.

Le dépôt public ne contient que le code de l'appli, aucune donnée.

Autres options : un dépôt GitLab perso (le fichier `.gitlab-ci.yml` fourni publie le site sur GitLab Pages), ou Netlify Drop (glisser-déposer du dossier, compte gratuit nécessaire pour garder le site en ligne).

## À savoir sur l'iPhone

- Ce que tu saisis dans un onglet Safari n'est **pas** partagé avec l'appli installée sur l'écran d'accueil. Utilise toujours l'icône.
- Si tu supprimes l'icône de l'écran d'accueil, iOS efface aussi les données de l'appli. **Exporte une sauvegarde régulièrement** (Plus → Sauvegarde et changement de téléphone → Exporter une sauvegarde, puis Enregistrer dans Fichiers ou iCloud Drive). L'appli te le rappelle tous les 30 jours.

## Changer de téléphone

1. Sur l'ancien téléphone : Plus → Sauvegarde et changement de téléphone → **Exporter une sauvegarde**, puis AirDrop vers le nouveau téléphone (ou Enregistrer dans Fichiers, sur iCloud Drive).
2. Sur le nouveau téléphone : ouvre l'adresse de ton appli dans Safari, puis Partager → Sur l'écran d'accueil.
3. Ouvre Okane depuis l'icône et touche **Restaurer une sauvegarde** dès le premier écran. Le fichier reçu par AirDrop est dans Fichiers → Téléchargements.

Même chose pour passer du Mac à l'iPhone ou l'inverse.
- Rappel quotidien : crée un rappel répété tous les jours dans l'app Rappels (marche à suivre dans les Réglages de l'appli).

## Mettre à jour l'appli

Remplace les fichiers sur GitHub (ou GitLab). L'iPhone récupère la nouvelle version à la prochaine ouverture avec du réseau. Tes données ne sont pas touchées.

## Renommer l'appli

Change `Okane` dans `manifest.webmanifest` (champs `name` et `short_name`) et dans `index.html` (balises `<title>` et `apple-mobile-web-app-title`).
