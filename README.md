# Cyber Cafe Smart

Site vitrine statique en HTML, CSS et JavaScript. Aucun gestionnaire de paquets ni
service backend n'est nécessaire.

## Lancer avec XAMPP

1. Placez le dossier `Site_Cyber_Smart` dans `C:\xampp\htdocs\`.
2. Ouvrez le panneau XAMPP et démarrez **Apache**.
3. Visitez :
   `http://localhost/MES_PROJETS/APPLICATIONS_WEB/Site_Cyber_Smart/`

Cette adresse correspond à l'emplacement actuel du projet sous `htdocs`. Si vous
déplacez le dossier directement dans `C:\xampp\htdocs\Site_Cyber_Smart`, utilisez
`http://localhost/Site_Cyber_Smart/`.

Les pages sont également accessibles sans extension `.html` grâce à la règle de
réécriture Apache du fichier `.htaccess`.

## Préparer une mise en production

1. Confirmez le nom de domaine définitif et activez un certificat HTTPS chez
   l'hébergeur.
2. Déposez le contenu du projet dans le dossier web public, en conservant
   `assets/`, `favicon/` et `pages/`.
3. Vérifiez que l'hébergement Apache autorise `.htaccess` et active les modules
   `mod_rewrite` et `mod_headers`.
4. Après confirmation du domaine, remplacez les URLs locales des balises
   `canonical`, Open Graph et Twitter dans les pages, puis mettez à jour
   `robots.txt` et `sitemap.xml`.
5. Testez les pages, le formulaire WhatsApp, la carte, le sitemap et le fichier
   robots sur le domaine HTTPS.

En attendant la confirmation du domaine, les URLs SEO utilisent
`http://localhost/MES_PROJETS/APPLICATIONS_WEB/Site_Cyber_Smart/`. Si le dossier
est déplacé sous `htdocs`, adaptez cette base locale dans les pages HTML,
`robots.txt` et `sitemap.xml`. Les URLs localhost ne sont pas destinées à être
indexées par les moteurs de recherche.

## Avant la mise en ligne

- Confirmez que le numéro WhatsApp `+223 92 73 12 09`, l'adresse
  `cybersmart223@gmail.com`, l'adresse à Djélibougou et les tarifs de formation
  affichés sont toujours exacts.
- Le formulaire prépare un message dans WhatsApp : il ne l'envoie pas et le site
  ne stocke aucune donnée de formulaire.
- Le fichier `.well-known/security.txt` contient les coordonnées de contact pour
  signaler une vulnérabilité. Mettez à jour les URLs du domaine réel avant la
  mise en production.
- Le portrait d'Alou est facultatif. Sans photo, ses initiales sont affichées.
  Pour ajouter sa photo, déposez `assets/images/team/alou.jpg` puis remplacez le
  bloc d'initiales de sa fiche dans `pages/about.html` par une balise `<img>`.
