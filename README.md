# Routine Compléments Alimentaires - PWA

Une application web progressive (PWA) pour le suivi quotidien de vos suppléments nutritionnels.

## 🚀 Installation sur iPhone

### Méthode 1 : Via Safari (Recommandée)

1. **Ouvrez Safari** sur votre iPhone
2. **Naviguez vers votre site** hébergé sur GitHub Pages
3. **Appuyez sur le bouton de partage** (carré avec flèche vers le haut)
4. **Sélectionnez "Sur l'écran d'accueil"**
5. **Personnalisez le nom** si nécessaire (par défaut : "Compléments")
6. **Appuyez sur "Ajouter"**

Votre app sera maintenant installée sur votre écran d'accueil !

### Méthode 2 : Via le bouton d'installation

Si votre navigateur supporte l'installation automatique, un bouton "Installer l'app" apparaîtra automatiquement en bas à droite de l'écran.

## 📱 Fonctionnalités

- **Suivi quotidien** de vos compléments alimentaires
- **Gestion interactive des cures** avec dates de début/fin
- **Planning personnalisé** matin/soir
- **Calcul automatique** des coûts et stocks
- **Fonctionnement hors ligne** grâce au cache
- **Interface adaptée mobile** avec design moderne

## 🛠️ Développement

### Structure des fichiers

```
routine_complements_alimentaires/
├── routine_complements_alimentaires.html  # Application principale
├── manifest.json                          # Configuration PWA
├── sw.js                                  # Service Worker
└── README.md                              # Ce fichier
```

### Configuration PWA

Le fichier `manifest.json` contient :
- **Nom et description** de l'application
- **Icônes** en différentes tailles (192x192, 512x512)
- **Couleurs** du thème (#66BFFF)
- **Mode d'affichage** standalone (comme une vraie app)
- **Raccourcis** pour accès rapide

### Service Worker

Le fichier `sw.js` gère :
- **Mise en cache** des ressources
- **Fonctionnement hors ligne**
- **Mise à jour automatique** du cache

## 🎨 Personnalisation

### Couleurs du thème

Les couleurs principales utilisées :
- **Bleu principal** : `#66BFFF`
- **Violet secondaire** : `#D0B3FF`
- **Rose accent** : `#F8BFD8`
- **Fond sombre** : `#0F0F1A`

### Ajout de nouveaux compléments

Pour ajouter un nouveau complément, modifiez la section `<tbody>` dans le fichier HTML et ajoutez une nouvelle ligne avec la structure :

```html
<tr>
    <td class="supplement-name">Nom du complément</td>
    <td class="dosage">Dosage</td>
    <td class="ar-percentage">% AR</td>
    <td>Fréquence</td>
    <td class="timing">Moment</td>
    <td>Durée cure</td>
    <td>Durée pause</td>
    <td class="status active">✅ Actif</td>
    <td class="price">Prix</td>
    <td class="stock">Stock</td>
</tr>
```

## 📊 Fonctionnalités avancées

### Suivi des cures

- **Dates automatiques** : Calcul automatique des durées
- **Statuts visuels** : Actif, En pause, Terminé
- **Barres de progression** : Suivi visuel de l'avancement
- **Actions interactives** : Pause, reprise, reset

### Stock et coûts

- **Calcul automatique** du coût quotidien
- **Alertes de stock** pour les compléments critiques
- **Prix unitaires** et coûts quotidiens

## 🔧 Déploiement

### GitHub Pages

1. **Poussez vos fichiers** sur GitHub
2. **Activez GitHub Pages** dans les paramètres du repository
3. **Sélectionnez la branche** (généralement `main`)
4. **Votre site sera accessible** à l'URL : `https://votre-username.github.io/votre-repo`

### Autres hébergeurs

La PWA fonctionne sur tout hébergeur web statique :
- Netlify
- Vercel
- Firebase Hosting
- Serveur web classique

## 📱 Compatibilité

- ✅ **iPhone** (Safari)
- ✅ **Android** (Chrome, Firefox)
- ✅ **Desktop** (Chrome, Firefox, Safari, Edge)
- ✅ **iPad** (Safari)

## 🆘 Support

Si vous rencontrez des problèmes :

1. **Vérifiez que HTTPS** est activé (requis pour les PWA)
2. **Videz le cache** du navigateur
3. **Désinstallez et réinstallez** l'app depuis l'écran d'accueil
4. **Vérifiez la console** pour les erreurs JavaScript

## 📝 Licence

Ce projet est open source. Vous pouvez le modifier et l'adapter selon vos besoins.

---

**Bon suivi de vos compléments ! 💪**
