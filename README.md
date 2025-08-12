# 🗃️ GITnorm-Deploy

Dépôt Git centralisé contenant :

- Les releases `.zip` officielles de la suite GITnorm
- Les fichiers JSON de configuration dynamique (software, news, lang)

Ce dépôt est mis à jour automatiquement via l’application `GITnorm.Deploy`.

## 📦 Arborescence type

**• GITnorm.Manager/**  
*— GITnorm.Manager_v1.3.2.zip*

**• BIMnorm/**  
 **• BIMnorm.Revit2023/**  
 *— BIMnorm.Revit2023_v0.0.1.zip*  
  **• BIMnorm.Revit2024/**  
 *— BIMnorm.Revit2024_v0.0.1.zip*  
  **• BIMnorm.Revit2025/**  
 *— BIMnorm.Revit2025_v0.0.1.zip*  
  **• BIMnorm.Revit2026/**  
 *— BIMnorm.Revit2026_v0.0.1.zip*  
   **• packages/**  
 *— DynamoIronPython2.7-2.5.0.zip.zip*  
  *— DynamoIronPython2.7-3.2.1.zip*  
   **• scripts/**  
 *— AllPoints.git*  
 *— AssociateActiveWorkset.git*  
 *— CopyElementsWithAssociatedWorkset.git*  
 *— Create3dLinkedElements.git*  
 *— DefineActiveWorkset.git*  
 *— etc.*

**• CADnorm/**  
 **• CADnorm.Autocad2023/**  
 *— CADnorm.Autocad2023_v0.0.1.zip*  
  **• CADnorm.Autocad2024/**  
 *— CADnorm.Autocad2024_v0.0.1.zip*  
  **• CADnorm.Autocad2025/**  
 *— CADnorm.Autocad2025_v0.0.1.zip*  
  **• CADnorm.Autocad2026/**  
 *— CADnorm.Autocad2026_v0.0.1.zip*  
   **• packages/**  
   **• scripts/**  

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
