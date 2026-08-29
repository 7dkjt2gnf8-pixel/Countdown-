# Countdown+

Application web autonome (un seul fichier `index.html` + icônes) pour suivre :
- des échéances simples (titre + date/heure de fin) ;
- des crédits immobiliers (montant, dates, taux) avec calcul du capital restant dû en temps réel, basé sur les vraies échéances mensuelles.

Toutes les données sont enregistrées automatiquement (stockage persistant lié à l'utilisateur, pas de backend nécessaire).

## Publier sur GitHub Pages

1. Sur GitHub, crée un nouveau dépôt (par ex. `comptes-a-rebours`).
2. Sur la page du dépôt vide, clique sur **uploading an existing file** (ou **Add file → Upload files**).
3. Glisse-dépose tous les fichiers reçus (`index.html`, `manifest.json`, `favicon.ico`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`) directement à la racine du dépôt — pas de sous-dossier à créer.
4. Valide le commit (**Commit changes**).
5. Va dans **Settings → Pages**.
6. Dans **Build and deployment**, choisis **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
7. Après une ou deux minutes, ton appli est en ligne à l'adresse indiquée en haut de la page Pages (du type `https://TON-PSEUDO.github.io/comptes-a-rebours/`).

## Avec Git en ligne de commande (alternative)

```bash
cd comptes-a-rebours       # dossier contenant tous les fichiers téléchargés (index.html, manifest.json, etc.)
git init
git add .
git commit -m "Première version de l'appli"
git branch -M main
git remote add origin https://github.com/TON-PSEUDO/comptes-a-rebours.git
git push -u origin main
```

Puis active GitHub Pages comme à l'étape 5-6 ci-dessus.

## Installer l'appli sur le téléphone

Une fois en ligne, ouvre le lien GitHub Pages dans Safari (iPhone) ou Chrome (Android) puis :
- **iPhone** : bouton Partager → **Sur l'écran d'accueil**.
- **Android** : menu ⋮ → **Ajouter à l'écran d'accueil**.

L'icône et le nom de l'appli apparaissent comme une vraie application.
