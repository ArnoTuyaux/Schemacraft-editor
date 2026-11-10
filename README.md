# Atelier SchemaCraft

Éditeur de schémas Minecraft (26.3) dans le navigateur : ouvre un `.litematic`, `.schem`, `.schematic`
ou `.schema` (format du mod [SchemaCraft](https://github.com/ALK04/SchemaCraft)), change ses blocs,
et retélécharge-le dans le même format.

- **Aperçu 3D**, en couleurs ou avec les **vraies textures** : choisis une fois le `.jar` de ton jeu
  (`%appdata%\.minecraft\versions\26.3\26.3.jar`), la page le lit sur place et s'en souvient.
  Un pack de ressources `.zip` peut s'ajouter par-dessus.
- **Liste des blocs** utilisés : clic sur un bloc pour le remplacer (avec ses propriétés),
  le supprimer, ou le remplacer par un **mélange** de plusieurs blocs en pourcentages
  (ex. 50 % herbe, 30 % podzol, 20 % terre grossière ; positions tirées au hasard).
- **Remplacer partout** : `oak` → `spruce` change d'un coup bûches, planches, escaliers, feuilles...
  en gardant leur orientation ; les blocs qui n'existent pas sont signalés et ignorés.
- Annuler (Ctrl+Z).
- Les anciens `.schematic` (avant 1.13) sont convertis et enregistrés en `.schem` (WorldEdit).

Tout se passe dans le navigateur : aucun fichier n'est envoyé sur un serveur, et aucune texture
de Minecraft n'est publiée ici. Une seule page (`index.html`), sans compilation.

## Limites

- Les blocs sans modèle (coffres, panneaux, bannières, têtes...) sont dessinés en boîtes colorées.
- Remplacer un coffre (ou autre bloc-entité) par un autre bloc retire son contenu du fichier.

## Crédits

Liste des blocs et table des anciens identifiants numériques :
[PrismarineJS/minecraft-data](https://github.com/PrismarineJS/minecraft-data) (licence MIT),
complétée avec les blocs de 26.2 et 26.3.
Aperçu 3D : [three.js](https://threejs.org/) (MIT). Lecture des `.jar` : [JSZip](https://stuk.github.io/jszip/) (MIT).
