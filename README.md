# Radio Iqra - Instructions de Configuration

## ✅ Fichiers Créés

### 1. **pubspec.yaml**
Contient toutes les dépendances nécessaires :
- `just_audio: ^0.9.36` - Pour le streaming audio
- `google_fonts: ^6.1.0` - Pour la police Poppins
- `flutter_launcher_icons: ^0.13.1` - Pour l'icône de l'application

### 2. **lib/main.dart**
Code source complet avec :
- ✅ Interface utilisateur avec dégradé vert
- ✅ Lecture/Pause du flux radio
- ✅ Indicateur "EN DIRECT" animé
- ✅ Gestion des erreurs de connexion
- ✅ Design Material 3 moderne

### 3. **android/app/src/main/AndroidManifest.xml**
Avec la permission INTERNET requise.

---

## 📋 Étapes Suivantes

### Étape 1 : Ajouter le Logo
Vous devez placer votre logo dans le dossier `assets/` :
```
assets/logo.png
```

**Recommandations pour le logo :**
- Format : PNG avec fond transparent
- Taille : 1024x1024 pixels minimum
- Couleurs : Vert (#2E7D32), or, blanc
- Style : Calligraphie arabe élégante, symboles islamiques (croissant, étoile), ondes radio

> **Note :** Le code inclut un fallback (icône radio) si le logo n'est pas trouvé.

### Étape 2 : Installer les Dépendances
```bash
flutter pub get
```

### Étape 3 : Générer les Icônes d'Application
```bash
flutter pub run flutter_launcher_icons
```

### Étape 4 : Compiler l'APK en Mode Release
```bash
flutter build apk --release
```

L'APK sera généré dans :
```
build/app/outputs/flutter-apk/app-release.apk
```

---

## 🎨 Caractéristiques de l'Interface

- **Dégradé** : Vert forêt → Blanc cassé
- **Police** : Poppins (Google Fonts)
- **Couleurs** :
  - Vert principal : `#2E7D32`
  - Fréquence : Ambre `#FFA726`
  - Live : Rouge `#E53935`
- **Animations** :
  - Pulsation de l'indicateur "EN DIRECT"
  - Transitions fluides Play/Pause

---

## 🔧 Dépannage

### Si Flutter n'est pas installé :
1. Téléchargez Flutter : https://flutter.dev/docs/get-started/install
2. Ajoutez Flutter au PATH
3. Exécutez `flutter doctor` pour vérifier l'installation

### Si l'audio ne fonctionne pas :
- Vérifiez votre connexion Internet
- Testez l'URL du flux : https://radioiqrabf-1.ice.infomaniak.ch/radioiqrabf-96.mp3

---

## 📱 Test de l'Application

### Sur Émulateur/Appareil :
```bash
flutter run
```

### Actions à Tester :
1. ✅ Appuyer sur Play → Le son démarre
2. ✅ Vérifier l'indicateur "EN DIRECT"
3. ✅ Appuyer sur Pause → Le son s'arrête
4. ✅ Tester sans connexion → Message d'erreur s'affiche

---

## 🎯 Résumé des Commandes

```bash
# 1. Installer les dépendances
flutter pub get

# 2. Générer les icônes
flutter pub run flutter_launcher_icons

# 3. Tester l'application
flutter run

# 4. Compiler l'APK final
flutter build apk --release
```

---

**Vibe attendue** : Une application spirituelle, élégante et simple d'utilisation. Une seule pression pour écouter la voix du Saint Coran. 🎙️📻
