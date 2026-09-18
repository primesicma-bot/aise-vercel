# Aise — Site vitrine + application web

Projet statique prêt pour **GitHub + Vercel**.

## Structure

- `/` — site vitrine Aise
- `/app/` — application web Aise
- `/assets/` — ressources
- `vercel.json` — configuration Vercel + en-têtes de sécurité
- `sw.js` — service worker PWA

## Déployer avec GitHub + Vercel

1. Créer un dépôt GitHub.
2. Mettre **le contenu de ce dossier** à la racine du dépôt (pas le dossier parent lui-même).
3. Sur Vercel, choisir **Add New → Project**.
4. Importer le dépôt GitHub.
5. Framework Preset : **Other**.
6. Build Command : laisser vide.
7. Output Directory : laisser vide ou `.`.
8. Cliquer sur **Deploy**.

Vercel redéploiera automatiquement le site à chaque push sur la branche connectée.

## URLs

- `https://ton-domaine.vercel.app/` — présentation
- `https://ton-domaine.vercel.app/app/` — application

Les boutons du site qui servent à utiliser Aise pointent directement vers `/app/`.

## Sécurité

La configuration `vercel.json` applique des en-têtes de sécurité côté Vercel. Le frontend ne contient pas de secret serveur. Pour une future version avec comptes, SMS automatiques, base de données ou API, les secrets et contrôles d'accès devront rester côté serveur.

## SMS

L'application peut préparer un SMS depuis l'appareil. L'envoi automatique de SMS nécessite une API/backend sécurisé et un fournisseur SMS ; aucune clé de fournisseur n'est embarquée dans le frontend.
