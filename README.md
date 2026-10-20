# MOUNKO Outdoor Furniture

Site vitrine de MOUNKO, mobilier d'extérieur à Jarry (Guadeloupe).

- 300 modèles classés en 10 collections, avec leur référence `MK-xxxx`
- Recherche par référence, fiche agrandie, copie de la référence
- Contact WhatsApp et WeChat (boutons et QR codes)

## Structure

- `index.html` : la page complète (HTML, CSS et JS dans un seul fichier, données produits incluses)
- `img/` : photos des modèles (`MK-xxxx.webp`) et image d'accueil (`hero.webp`, `hero-wide.webp`)
- `vercel.json` : configuration Vercel (cache des images)

## Déploiement sur Vercel

Site statique, aucune compilation nécessaire.

1. Sur vercel.com : **Add New… → Project**, puis importer ce dépôt GitHub.
2. Framework Preset : **Other**. Laisser *Build Command* et *Output Directory* vides.
3. **Deploy**.

Chaque `git push` sur la branche `main` redéploie automatiquement le site.

## Modifier le site

- **Ajouter un modèle** : déposer la photo dans `img/MK-xxxx.webp`, puis ajouter une ligne `["MK-xxxx","img/MK-xxxx.webp","categorie"]` dans le tableau `const P=` de `index.html`.
- **Catégories** : `salons`, `repas`, `fauteuils`, `bar`, `daybeds`, `transats`, `suspendus`, `pergolas`, `exterieur`, `parasols`.
- **Contacts** : rechercher `wa.me` (WhatsApp) et `u.wechat.com` (WeChat) dans `index.html`.
