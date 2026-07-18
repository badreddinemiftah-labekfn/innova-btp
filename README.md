# Site vitrine INNOVA BTP

Site statique premium en français pour INNOVA BTP, entreprise marrakchie active dans la fabrication de plâtre et la projection d’enduit plâtre. Le contenu public utilise uniquement les informations présentes dans les fichiers sources fournis.

## Structure

- `index.html` : accueil, entreprise, expertises, approche, identité, FAQ et contact.
- `privacy-policy.html` : politique conforme au fonctionnement statique actuel.
- `404.html` : page d’erreur personnalisée.
- `assets/css/` : design system, animations et adaptations responsive.
- `assets/js/` : navigation, formulaire, accordéon, révélations et interactions.
- `assets/icons/favicon.svg` : monogramme temporaire créé pour le site.
- `robots.txt` et `sitemap.xml` : bases SEO à finaliser avec le domaine.

## Utilisation locale

Ouvrir `index.html` directement, ou lancer un serveur local depuis ce dossier :

```powershell
python -m http.server 8000
```

Puis ouvrir `http://localhost:8000`.

## Personnalisation

- Identité et textes : modifier les fichiers HTML.
- Couleurs, espacements et rayons : variables `:root` dans `assets/css/style.css`.
- Services : cartes dans la section `#expertise` de `index.html`.
- Logo : remplacer le monogramme `.brand-mark` par une image locale optimisée et mettre à jour le favicon.
- Images : déposer les fichiers dans `assets/images/`, utiliser des noms descriptifs, `loading="lazy"`, un texte alternatif et des dimensions explicites.
- SEO : remplacer le domaine fictif dans `robots.txt`, `sitemap.xml` et ajouter les URL canoniques/Open Graph de production.

## Contact et confidentialité

Il n’existe ni adresse email, ni téléphone, ni WhatsApp officiel dans les sources. Le formulaire valide les champs puis prépare le message uniquement dans le navigateur. Il ne contacte aucun serveur et n’affirme jamais que le message a été livré.

Pour brancher un backend, remplacer le traitement `submit` dans `assets/js/main.js` par un appel HTTPS sécurisé, afficher les états de chargement/erreur, protéger l’API contre le spam et mettre à jour la politique de confidentialité (finalité, base juridique, fournisseur, destinataires et conservation). Pour un email ou WhatsApp, n’ajouter que des coordonnées officiellement confirmées et utiliser respectivement `mailto:` ou `https://wa.me/NUMERO` au format international.

Le site ne dépose aucun cookie, n’utilise pas de stockage local, d’analytics, de carte intégrée, de pixel ou de police externe. Aucun bandeau cookie n’est donc justifié actuellement. Si un outil non essentiel est ajouté, bloquer son chargement avant consentement, proposer Accepter/Refuser et documenter le choix.

La politique doit être relue par un professionnel du droit avant publication et révisée dès qu’un hébergeur ou un service de formulaire est choisi.

## Déploiement

- GitHub Pages : pousser le dossier dans un dépôt, puis activer Pages sur la branche principale et la racine `/`.
- Netlify : déposer le dossier dans l’interface ou relier le dépôt ; aucun build n’est requis, dossier de publication `.`.
- Vercel : importer le dépôt comme site statique, sans commande de build, sortie à la racine.
- Hébergement classique : envoyer tous les fichiers en conservant exactement l’arborescence, puis activer HTTPS et configurer `404.html` comme page d’erreur.

Une politique Content Security Policy est recommandée au niveau de l’hébergeur. Base possible à tester : `default-src 'self'; img-src 'self' data:; style-src 'self'; script-src 'self'; object-src 'none'; base-uri 'self'; form-action 'self'`.

## Information required before production launch

- Domaine de production et URL canonique
- Logo officiel et éventuelle charte de marque
- Téléphone professionnel confirmé
- Numéro WhatsApp professionnel confirmé
- Email général et email confidentialité
- Horaires d’ouverture
- Hébergeur et politique de journaux techniques
- Backend du formulaire, destinataire et durée de conservation
- Responsable/représentant légal si publication souhaitée
- Choix analytics et exigences cookies, uniquement si nécessaires
- Photographies de projets avec droits d’utilisation
- Validation de l’adresse normalisée
- Relecture juridique de la politique de confidentialité

## Informations vérifiées et hypothèses

Nom : INNOVA BTP. Forme : SARL. Activité : fabricant de plâtre et projection d’enduit plâtre. Siège fourni : 34 rue du Lieutenant Lamure, Résidence Marrakchia 2, Guéliz, Marrakech, Maroc. ICE : 000221916000055. RC / identifiant fiscal fourni : 33845. D‑U‑N‑S fourni : 353931265 (non affiché publiquement car inutile au parcours visiteur).

Le monogramme « IB », les illustrations architecturales en CSS/SVG et le parcours en quatre étapes sont des éléments éditoriaux d’interface, sans constituer un logo officiel, une certification ou une promesse contractuelle. Aucun service externe n’est utilisé.
