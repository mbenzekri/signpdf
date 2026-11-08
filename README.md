# signpdf

Application locale pour ajouter des images PNG sur les pages d'un PDF, les déplacer, les redimensionner et les faire pivoter, puis télécharger une nouvelle copie du document.

## Utilisation

1. Téléchargez ou clonez le dépôt complet.
2. Ouvrez `App Signature PDF.html` dans votre navigateur. Conservez le dossier `vendor` à côté du fichier HTML.
3. Chargez un PDF et importez une ou plusieurs images PNG. De nouveaux imports enrichissent la liste existante.
4. Cliquez sur **Ajouter** pour placer une image sur la page affichée. Chaque image peut être utilisée plusieurs fois.
5. Déplacez l'image par glisser-déposer. Le rond rouge en bas à droite permet de la redimensionner ; le bouton bleu en haut à gauche permet de la faire pivoter par glissement ou par clics de 15°.
6. Téléchargez le PDF complété avec le bouton d'export. Le fichier original n'est pas écrasé.

Le traitement reste dans le navigateur. L'application fonctionne hors ligne, sans installation ni chargement externe de bibliothèques. Les documents et images ne sont pas téléversés.

Les images ajoutées peuvent représenter une signature ou un paraphe ; l'application ne crée pas de signature numérique cryptographique.

## Bibliothèques incluses

- PDF.js 4.10.38, sous licence Apache-2.0.
- pdf-lib 1.17.1, sous licence MIT.

Les licences, les sources et les commandes de reconstruction sont conservées dans `vendor/NOTICE.txt` et les sous-dossiers de `vendor`.

## Vérifications effectuées

Vérifié dans Microsoft Edge en ouverture directe du fichier HTML et depuis un serveur local : import de plus de quatre images, ajout sur plusieurs pages et export sans requête externe. La rotation, le déplacement, le redimensionnement et la conservation de l'orientation dans le PDF exporté ont également été vérifiés.
