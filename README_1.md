# Atelier SchemaCraft

Éditeur de schémas Minecraft dans le navigateur : ouvre un `.litematic`, `.schem`, `.schematic`
ou `.schema` (format du mod [SchemaCraft](https://github.com/ALK04/SchemaCraft)), change ses blocs,
et retélécharge-le.

- Aperçu 3D du schéma.
- Liste des blocs utilisés : clic sur un bloc pour le remplacer (avec ses propriétés) ou le supprimer.
- « Remplacer partout » : `oak` → `spruce` change d'un coup bûches, planches, escaliers, feuilles...
  en gardant leur orientation ; les blocs qui n'existent pas sont signalés et ignorés.
- Annuler (Ctrl+Z).
- Les anciens `.schematic` (avant 1.13) sont convertis et enregistrés en `.schem` (WorldEdit).

Tout se passe dans le navigateur, aucun fichier n'est envoyé sur un serveur.
Une seule page (`index.html`), sans compilation.

## Limites

- L'aperçu utilise des cubes colorés, pas les textures du jeu.
- Remplacer un coffre (ou autre bloc-entité) par un autre bloc retire son contenu du fichier.

## Crédits

Liste des blocs et table des anciens identifiants numériques :
[PrismarineJS/minecraft-data](https://github.com/PrismarineJS/minecraft-data) (licence MIT).
Aperçu 3D : [three.js](https://threejs.org/) (licence MIT).
