# Maths Allophones

Le vocabulaire des mathématiques en français, pour les élèves allophones (UPE2A).

**En ligne :** https://tom-rougeaud.github.io/fls/

- 189 mots en 11 leçons, chacun avec une illustration, une définition simple, deux phrases à réutiliser et, pour 67 d’entre eux, plusieurs façons de dire la même chose
- La voix du professeur, enregistrée dans le studio intégré (plusieurs prises qui tournent), sinon une voix naturelle de synthèse (Piper), sinon la voix de l’appareil — une phrase est toujours dite en entier, jamais assemblée
- Des commentaires façon match de foot, variés, que le professeur peut compléter
- 3 niveaux d’exercices (je reconnais, je comprends, j’écris), 3 ateliers (nombres, opérations, consignes), une révision en spirale qui mélange les leçons déjà vues
- Zoom en haut à droite, glossaire, carnet personnel, fiche imprimable par leçon

## Fonctionnement

- `index.html` : l’application (contenu pédagogique dans le bloc `id="mm-data"`, configuration Supabase dans le bloc `id="fls-config"`).
- `vendor/` : moteur de la voix naturelle (ONNX Runtime Web, phonémiseur Piper) et encodeur MP3 du studio. Le modèle de voix française est téléchargé une seule fois par chaque navigateur, à la demande.
- Aucune donnée d’élève n’est envoyée : la progression reste dans le navigateur (export / import / effacement dans le carnet).

## Licence

© Tom Rougeaud — [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/deed.fr). Les fichiers du dossier `vendor/` gardent leurs propres licences (voir `vendor/LICENCES.md`).
