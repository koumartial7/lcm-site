# Site LCM : mise en ligne et modification

Contenu du dossier : `index.html` (le site), `images/` (toutes les photos), `robots.txt`.
Gardez toujours `index.html` et le dossier `images` ensemble.

## Mettre en ligne (Netlify, gratuit)
1. app.netlify.com > créer un compte > « Add new site » > « Deploy manually ».
2. Glissez-déposez le dossier `lcm-site`. Vous obtenez une adresse `nom.netlify.app`.
3. Pour modifier le site plus tard : refaites un glisser-déposer du dossier mis à jour, il remplace l'ancienne version.

## Modifier un numéro ou un texte
Ouvrez `index.html` avec Notepad++ ou VS Code, utilisez « Rechercher et remplacer » (Ctrl+H) et enregistrez.
- WhatsApp : `2250152211642` (liens) et `+225 01 52 21 16 42` (affichage).
- Téléphones : `2250757943843` / `+225 07 57 94 38 43` et `2250709672972` / `+225 07 09 67 29 72`.
- Courriel : `koumartial7@gmail.com`.

## Ajouter ou supprimer une photo
1. Réduisez la photo à environ 1000 px de large (taille idéale : moins de 200 Ko).
2. Copiez-la dans le dossier `images`.
3. Dans `index.html`, cherchez « AJOUTER UNE PHOTO » : le modèle à copier s'y trouve, avec les consignes.
4. Pour supprimer : effacez le bloc `<figure>...</figure>` de la photo (et le fichier dans `images`).

## Ajouter une vidéo
Publiez-la sur YouTube, puis dans `index.html` cherchez « AJOUTER UNE VIDEO » et suivez les consignes (retirer les commentaires et mettre le code de la vidéo).

## Apparaître sur Google
1. Ajoutez le site sur search.google.com/search-console et demandez l'indexation.
2. Créez la fiche Google Business Profile « LCM – Leader des Constructions Modernes », San-Pédro.
3. Avec votre adresse définitive, créez un `sitemap.xml` et placez-le à côté de `index.html`.

## Formulaire
Il ouvre WhatsApp (+225 01 52 21 16 42) avec la demande pré-remplie ; le client appuie sur « Envoyer ».

## Sécurité
- Le fichier `_headers` active des protections dans le navigateur des visiteurs (HTTPS forcé, blocage de l'intégration du site dans d'autres sites, limitation des scripts extérieurs). Il fonctionne sur **Netlify** ; GitHub Pages l'ignore sans danger. Déposez-le avec le reste du dossier.
- Il autorise uniquement : vos propres fichiers, les polices Google et les vidéos YouTube. Si vous ajoutez un autre service (carte Google Maps, Facebook Pixel, chat…), il faudra l'ajouter dans la ligne `Content-Security-Policy`, sinon il sera bloqué.
- Activez la double authentification sur Netlify/GitHub, sur le registraire du domaine et sur votre Gmail. Activez le renouvellement automatique du domaine.
- Ne mettez jamais de mot de passe ni de jeton dans `index.html` : tout y est public.
- Gardez une copie du dossier `lcm-site` sur Google Drive ou une clé USB.
- Après la mise en ligne, testez le site sur securityheaders.com : la note doit être A ou A+.
