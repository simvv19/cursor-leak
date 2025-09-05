# Plateforme de Partage de Vidéos

Une application web moderne pour partager et télécharger des vidéos avec une interface d'administration.

## 🚀 Fonctionnalités

- **Landing Page** : Affichage des vidéos avec titre et tags
- **Interface d'Administration** : Upload et gestion des vidéos
- **Recherche et Filtres** : Recherche par titre/tags et filtrage par tags
- **Téléchargement** : Téléchargement direct des vidéos
- **Design Responsive** : Interface moderne et adaptative
- **Gestion des Fichiers** : Support des formats vidéo courants

## 📋 Prérequis

- Node.js (version 14 ou supérieure)
- npm (Node Package Manager)

## 🛠️ Installation

1. **Cloner ou télécharger le projet**
   ```bash
   cd "Cursor XXX"
   ```

2. **Installer les dépendances**
   ```bash
   npm install
   ```

3. **Démarrer le serveur**
   ```bash
   npm start
   ```
   
   Ou pour le développement avec rechargement automatique :
   ```bash
   npm run dev
   ```

4. **Accéder à l'application**
   - Page principale : http://localhost:3000
   - Interface admin : http://localhost:3000/admin

## 📁 Structure du Projet

```
├── server.js              # Serveur Express principal
├── package.json           # Configuration npm
├── videos.json           # Base de données des vidéos (créé automatiquement)
├── uploads/              # Dossier des vidéos uploadées
└── public/               # Fichiers frontend
    ├── index.html        # Page d'accueil
    ├── admin.html        # Interface d'administration
    ├── styles.css        # Styles CSS
    ├── script.js         # JavaScript pour la page principale
    └── admin.js          # JavaScript pour l'administration
```

## 🎯 Utilisation

### Page d'Accueil
- Consultez toutes les vidéos disponibles
- Utilisez la barre de recherche pour filtrer par titre ou tags
- Cliquez sur les tags pour filtrer par catégorie
- Triez les vidéos par date, titre ou taille
- Téléchargez les vidéos en cliquant sur le bouton "Télécharger"

### Interface d'Administration
1. **Upload de Vidéos** :
   - Sélectionnez un fichier vidéo (MP4, AVI, MOV, WMV, FLV, WebM)
   - Ajoutez un titre obligatoire
   - Optionnellement, ajoutez des tags séparés par des virgules
   - Cliquez sur "Uploader la Vidéo"

2. **Gestion des Vidéos** :
   - Consultez toutes les vidéos uploadées
   - Téléchargez ou copiez le lien de téléchargement
   - Supprimez les vidéos si nécessaire

## 🔧 Configuration

### Formats Vidéo Supportés
- MP4
- AVI
- MOV
- WMV
- FLV
- WebM

### Limite de Taille
- Taille maximale par fichier : 100MB

### Port
- Port par défaut : 3000
- Modifiable via la variable d'environnement `PORT`

## 🚀 Déploiement

### Variables d'Environnement
```bash
PORT=3000  # Port du serveur (optionnel)
```

### Production
```bash
npm start
```

## 🛡️ Sécurité

- Validation des types de fichiers
- Limitation de la taille des uploads
- Échappement HTML pour éviter les injections XSS
- Gestion des erreurs côté serveur et client

## 📱 Responsive Design

L'interface s'adapte automatiquement aux différentes tailles d'écran :
- Desktop (1200px+)
- Tablette (768px - 1199px)
- Mobile (< 768px)

## 🎨 Personnalisation

### Couleurs
Les couleurs principales peuvent être modifiées dans `public/styles.css` :
- Couleur principale : `#667eea`
- Couleur secondaire : `#764ba2`
- Couleur de succès : `#28a745`
- Couleur d'erreur : `#dc3545`

### Limites
- Modifiez la limite de taille dans `server.js` (ligne 47)
- Ajoutez de nouveaux formats vidéo dans `server.js` (ligne 40)

## 🐛 Dépannage

### Problèmes Courants

1. **Erreur "Port déjà utilisé"**
   ```bash
   # Changer le port
   PORT=3001 npm start
   ```

2. **Erreur d'upload**
   - Vérifiez que le dossier `uploads/` existe
   - Vérifiez les permissions d'écriture
   - Vérifiez la taille du fichier (max 100MB)

3. **Vidéos non affichées**
   - Vérifiez que le fichier `videos.json` existe
   - Vérifiez les permissions de lecture

## 📄 Licence

MIT License - Libre d'utilisation et de modification.

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Signaler des bugs
- Proposer des améliorations
- Soumettre des pull requests

---

**Développé avec ❤️ pour le partage de vidéos**
