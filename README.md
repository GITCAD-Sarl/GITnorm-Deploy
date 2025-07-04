# 🗃️ GITnorm-Deploy

Dépôt Git centralisé contenant :

- Les releases `.zip` officielles de la suite GITnorm
- Les fichiers JSON de configuration dynamique (software, news, lang)

Ce dépôt est mis à jour automatiquement via l’application `GITnorm.Deploy`.

## 📦 Arborescence type

**GITnorm-Deploy/**  
**• GITnorm.Core/**  
*— GITnorm.Core_v1.0.0.zip*

**• GITnorm.Manager/**  
*— GITnorm.Manager_v1.3.2.zip*

**• BIMnorm/**  
 **• BIMnorm.Revit2023/**  
 *— BIMnorm.Revit2023_v1.2.0.zip*

**• CADnorm/**  
 **• CADnorm.Autocad2024/**  
 *— CADnorm.Autocad2024_v1.0.4.zip*

**• json/**  
*— software.json*  
*— news.json*  
*— lang_fr.json*

## 📚 Contenu

- **Releases .zip** — Générées automatiquement via `GITnorm.Deploy`
- **JSON** — Chargés dynamiquement par `GITnorm.Manager`

## 📂 Fichiers JSON principaux

- *software.json* — Liste logicielle affichée dans le Manager
- *news.json* — Derniers messages/communications (format limité à 5 éléments)
- *lang_fr.json* — Traductions clés/valeurs en français (fallback EN/DE)

## 🔁 Processus de publication

1. L’utilisateur lance `GITnorm.Deploy`
2. Sélection du projet à publier
3. Compilation & création `.zip` versionné
4. Commit + tag Git (`vX.Y.Z`)
5. Push automatique sur `main`

## 🔐 Accès

- Accès restreint (interne GITCAD Sàrl)
- Aucun exécutable ne doit être publié ici manuellement
- Pas de Release GitHub : tout passe via le commit Git classique

## 🛠️ Utilisé par

- `GITnorm.Manager` (pour chargement logiciel et news)
- `GITnorm.Updater` (pour détection de version distante)

## 📦 Licence

Contenu propriétaire – Ne pas redistribuer.  
Contact : https://www.git-cad.ch
