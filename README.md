# MixCheck : versions de test

**MixCheck** vérifie un mix avant livraison : clics, pops, thumps, silences sans ambiance, ronflette, crêtes et écrêtage, et conformité loudness aux normes du streaming, du broadcast et des plateformes vidéo.

Ce dépôt contient seulement les **versions publiées**, pas le code source.

## Télécharger

👉 **[Dernière version](../../releases/latest)** (page *Releases*, à droite)

| Système | Fichier | Contenu |
|---|---|---|
| macOS (Apple Silicon et Intel) | `MixCheck-<version>-macOS.dmg` | Application, plug-ins AU, VST3, CLAP |
| Windows | `MixCheck-<version>-Windows.zip` | Application, plug-ins VST3 et CLAP, outil en ligne de commande (pas encore disponible pour la 0.2.1) |

Chaque version est accompagnée de l'empreinte **SHA-256** du DMG (fichier `.sha256`), pour vérifier que le téléchargement est intact. Cette vérification est facultative :
```bash
shasum -a 256 ~/Downloads/MixCheck-<version>-macOS.dmg
```

## Installer

### macOS
1. Ouvrez le DMG et glissez **MixCheck.app** dans **Applications**.
2. Double-cliquez sur **« Installer les plug-ins.command »** : il copie les plug-ins AU, VST3 et CLAP dans `~/Library/Audio/Plug-Ins`.
3. Relancez le DAW. Les plug-ins se trouvent chez le fabricant **MixCheck**.

L'application et les plug-ins sont **signés et notarisés par Apple** : macOS les ouvre normalement, après un simple message de confirmation au premier lancement.

### Windows
1. Décompressez le zip.
2. Copiez **MixCheck.vst3** dans `C:\Program Files\Common Files\VST3` et **MixCheck.clap** dans `C:\Program Files\Common Files\CLAP`.
3. L'application autonome est **MixCheck.exe**.

## Mises à jour

À partir de la version 0.2.2, au lancement, MixCheck vérifie s'il existe une version plus récente sur ce dépôt. Si c'est le cas, un bouton **« Mise à jour x.y.z »** apparaît en haut à droite. **Télécharger** ouvre la page de la version. **Ignorer cette version** masque le bouton jusqu'à la suivante. Vous pouvez désactiver cette vérification dans les **Réglages** (roue crantée), avec l'option **Vérifier les mises à jour au lancement**. Aucune donnée n'est envoyée : MixCheck lit seulement le numéro de la dernière version.

## Signaler un problème

Ouvrez une [issue](../../issues) en indiquant :
- la version de MixCheck (dans les Réglages : « Version installée ») ;
- le système (macOS ou Windows et sa version), le DAW, ou l'application autonome ;
- ce que vous avez fait, ce que vous attendiez et ce qui s'est passé ;
- si possible, une capture d'écran ou un court extrait audio.
