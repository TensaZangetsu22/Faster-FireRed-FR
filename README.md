# Pokémon Rouge Feu Ironmon Kaizo — Patch FR 1.3.1

> 🇬🇧 [Read this README in English](README_EN.md)

Adaptation française de **Faster FireRed** pour une ROM française de **Pokémon Version Rouge Feu**, destinée principalement aux runs **IronMON / Ironmon Kaizo**.

Ce dépôt / cette release fournit uniquement un **patch**. Aucune ROM Pokémon n'est distribuée.

---

## Sommaire

1. [Origine du patch](#1-origine-du-patch)
2. [Modifications apportées](#2-modifications-apportées)
3. [Appliquer le patch à une ROM française](#3-appliquer-le-patch-à-une-rom-française)
4. [Tracker Ironmon traduit en français](#4-tracker-ironmon-traduit-en-français)
6. [Liens externes et crédits](#6-liens-externes-et-crédits)

---

## 1. Origine du patch

Ce projet est basé sur le patch US **Faster FireRed** créé par **DrMaple** :

- **Faster FireRed** : https://github.com/DrMaple/Faster-FireRed

Le projet original est un patch pour **Pokémon FireRed (Rev 1 / 1.1)** qui ajoute plusieurs améliorations de confort spécialement pensées pour les runs IronMON.

La présente version française reprend ce travail comme base, puis adapte les modifications à une **ROM française vanilla de Pokémon Version Rouge Feu**.

La variante utilisée comme base est la version **No Hidden Item Marks**, afin de conserver les objets cachés réellement cachés.

### ROM française de référence

La version actuelle du patch a été développée et testée avec la ROM française de référence utilisée pendant le développement.

- **Format** : GBA
- **SHA-1 de la ROM FR de référence** : `FC663907256F06A3A09E2D6B967BC9AF4919F111`

Avant d'appliquer le patch, il est fortement recommandé de vérifier que votre dump correspond à cette ROM.

---

## 2. Modifications apportées

### Modifications héritées de Faster FireRed

Le patch conserve les principales améliorations de confort du projet Faster FireRed, notamment :

- démarrage de l'aventure accéléré ;
- quête du Colis de Chen raccourcie ;
- proposition automatique d'utiliser un nouveau Repousse lorsque le précédent expire ;
- renommeurs de Pokémon ajoutés dans les Centres Pokémon ;
- animation de soin aux centres Pokémon fortement raccourcie ;
- certains objets au sol des Passages Souterrains et des Îles Sevii garantis ;
- objet normalement récupéré depuis le PC déplacé dans le laboratoire du Professeur Chen ;
- Léo ne propose plus automatiquement le voyage vers les Îles Sevii après Auguste ; il reste disponible au Centre Pokémon de Cramois'Île pour lancer ce voyage manuellement ;
- ajout de certains ajustements / PNJ de confort destinés aux runs IronMON ;
- infirmière ajoutée dans la Forêt de Jade selon les règles du patch Faster FireRed ;
- **aucun marqueur visuel ajouté sur les objets cachés** dans cette variante.

Pour le détail complet des changements d'origine, consulter le dépôt de DrMaple :
https://github.com/DrMaple/Faster-FireRed

### Adaptations et modifications spécifiques à la version française

Cette version ajoute notamment :

- correction du **PNJ qui évalue le bonheur des Pokémon** dans la dernière version du patch (**1.3.1**) ;
- adaptation du patch Faster FireRed à une **ROM française de Pokémon Rouge Feu** ;
- traduction / adaptation en français des textes et dialogues concernés par le patch ;
- validation du déplacement de l'objet du PC vers le laboratoire du Professeur Chen sur la ROM FR ;
- raccourcissement supplémentaire du lancement d'une **nouvelle partie**, avec suppression d'écrans d'introduction intermédiaires afin d'arriver plus rapidement à la création de la partie ;
- réduction de la cinématique de **Léo dans sa maison de la Route 25** ;
- réduction du dialogue du **Président du Fan Club Pokémon à Carmin-sur-Mer** ;
- écran titre personnalisé avec :
  - **ROUGE FEU / IRONMON / KAIZO** ;
  - la mention **Patch FR 1.3 made by TensaZangetsu22** ;
- ajustements graphiques afin de conserver un rendu cohérent avec le style de l'écran titre original de Pokémon Rouge Feu.

L'objectif général est de conserver le gameplay et l'esprit du patch US tout en proposant une expérience entièrement adaptée à la version française du jeu.

---

## 3. Appliquer le patch à une ROM française

### Avant de commencer

Vous avez besoin de :

1. votre propre ROM française **vanilla** de Pokémon Version Rouge Feu ;
2. le fichier `Faster.FireRed.1.3.1.FR.Avec.Croix.PNJ.Bonheur.Corrige.ips` fourni avec cette release ;
3. un outil capable d'appliquer un patch IPS.

**Conservez toujours une copie intacte de votre ROM originale.**

Le patch ne doit pas être appliqué par-dessus une ROM déjà modifiée, randomisée ou déjà patchée.

### Vérification de la ROM

La ROM française de référence utilisée pour ce projet possède le SHA-1 suivant :

- `FC663907256F06A3A09E2D6B967BC9AF4919F111`

Si votre outil de patch affiche le SHA-1 de la ROM, vérifiez qu'il correspond avant d'appliquer le patch.

---

### macOS — méthode recommandée avec MultiPatch

Sur macOS, vous pouvez utiliser **MultiPatch**, une application native développée par Sappharad :

https://projects.sappharad.com/multipatch/

MultiPatch prend en charge notamment les formats **IPS, BPS, UPS, PPF, XDelta, BSDiff et RUP**.

> **Important : MultiPatch est une application macOS.**  
> Il n'existe pas de version officielle de MultiPatch pour Windows ou Linux.

#### Installation

1. Téléchargez MultiPatch depuis le site officiel :
   - https://projects.sappharad.com/multipatch/
2. Ouvrez l'application.
3. Si macOS bloque son lancement, faites un clic droit sur l'application puis **Ouvrir**, ou autorisez-la dans **Réglages Système > Confidentialité et sécurité**.

#### Appliquer le patch

1. Lancez **MultiPatch**.
2. Dans **Location of patch file**, sélectionnez le fichier `.ips` du patch FR.
3. Dans **Location of file to patch**, sélectionnez votre ROM française vanilla `.gba`.
4. Dans **Save patched file as**, choisissez un nouveau nom de fichier, par exemple :
   - `Pokemon_Rouge_Feu_Ironmon_Kaizo_FR.gba`
5. Cliquez sur **Apply Patch**.
6. Attendez le message confirmant que le patch a été appliqué.
7. Chargez la ROM nouvellement créée dans votre émulateur.

Ne remplacez pas directement votre ROM originale : conservez toujours une copie propre.

---

### Windows — Rom Patcher JS

MultiPatch n'est pas disponible officiellement sous Windows.

La solution la plus simple est **Rom Patcher JS** :

https://www.marcrobledo.com/RomPatcher.js/

1. Ouvrez Rom Patcher JS dans votre navigateur.
2. Dans **ROM file**, sélectionnez votre ROM française vanilla.
3. Vérifiez, si possible, que son SHA-1 correspond à :
   - `FC663907256F06A3A09E2D6B967BC9AF4919F111`
4. Dans **Patch file**, sélectionnez le fichier `.ips` du patch FR.
5. Cliquez sur **Apply patch**.
6. Enregistrez la ROM générée sous un nouveau nom.
7. Chargez cette ROM dans votre émulateur.

Vous pouvez également utiliser un patcher IPS Windows local compatible si vous préférez travailler hors ligne.

---

### Linux — Rom Patcher JS

MultiPatch n'est pas disponible officiellement sous Linux.

La méthode la plus simple reste **Rom Patcher JS** :

https://www.marcrobledo.com/RomPatcher.js/

1. Ouvrez Rom Patcher JS dans votre navigateur.
2. Chargez votre ROM française vanilla `.gba`.
3. Chargez le patch `.ips`.
4. Vérifiez le SHA-1 de la ROM si l'outil l'affiche.
5. Cliquez sur **Apply patch**.
6. Enregistrez la ROM générée sous un nouveau nom.

Vous pouvez également utiliser un patcher IPS natif pour Linux, à condition qu'il applique un patch IPS standard sans modifier la ROM d'une autre manière.

---

### Méthode alternative universelle — Rom Patcher JS

Rom Patcher JS fonctionne sous **Windows, macOS et Linux** directement dans un navigateur moderne :

https://www.marcrobledo.com/RomPatcher.js/

Il constitue donc une excellente solution de secours si vous ne souhaitez pas installer d'application dédiée.

### Vérification après application

Au lancement, vous devez notamment retrouver :

- l'écran titre **Rouge Feu Ironmon Kaizo** ;
- la mention **Patch FR 1.3 made by TensaZangetsu22** ;
- les textes français ;
- les modifications de confort de Faster FireRed adaptées à la ROM FR.

Si l'écran titre est corrompu ou si le jeu ne démarre pas, vérifiez en priorité que vous avez utilisé la **bonne ROM FR vanilla** et non une ROM déjà modifiée.

---

## 4. Tracker Ironmon traduit en français

Une traduction française complète du **Ironmon Tracker Gen 3** est disponible dans le fork suivant :

- **Tracker FR — branche `feature/french-complete-translation`**  
  https://github.com/TensaZangetsu22/Ironmon-Tracker/tree/feature/french-complete-translation

Ce projet est un fork du tracker Gen 3 original maintenu ici :

- **Ironmon-Tracker original — besteon**  
  https://github.com/besteon/Ironmon-Tracker

La traduction française est actuellement **complète mais en attente de validation** avant une éventuelle intégration dans une future version officielle du tracker.

### Utiliser la ROM patchée avec le Tracker dans BizHawk

Le Tracker Gen 3 utilise des scripts Lua. BizHawk **2.8 ou supérieur** est requis par le projet ; sur Linux, une version plus récente est recommandée.

1. Téléchargez la branche française du Tracker.
2. Extrayez le dossier dans un emplacement simple.
   - Évitez si possible les dossiers synchronisés par le cloud.
   - Évitez les chemins contenant des caractères spéciaux si vous rencontrez des problèmes.
3. Lancez **BizHawk / EmuHawk**.
4. Ouvrez votre ROM **Rouge Feu Ironmon Kaizo FR patchée**.
5. Dans BizHawk, ouvrez :
   - `Tools -> Lua Console`
6. Dans la console Lua :
   - `Script -> Open Script...`
7. Sélectionnez :
   - `Ironmon-Tracker.lua`
8. Le Tracker doit apparaître et détecter la ROM chargée.
9. Configurez ensuite le Tracker via son icône d'engrenage selon vos préférences IronMON.

### Windows

BizHawk est directement pris en charge. Pensez à installer les prérequis BizHawk si nécessaire.

### Linux

Utilisez de préférence la **version Linux native de BizHawk**, plutôt que la version Windows via Wine / Proton. Le projet recommande BizHawk 2.9 ou supérieur sous Linux pour une meilleure compatibilité.

### macOS

BizHawk n'est pas la solution native recommandée sur macOS. Si vous utilisez **Parallels Desktop**, placez de préférence le dossier du Tracker dans le système de fichiers Windows de la VM plutôt que dans un dossier macOS partagé si vous rencontrez des problèmes de droits.

Le Tracker peut aussi fonctionner avec **mGBA**, mais les capacités d'affichage Lua y sont plus limitées que dans BizHawk.

Guide d'installation officiel du Tracker :
https://github.com/besteon/Ironmon-Tracker/wiki/Installation-Guide

---

## 6. Liens externes et crédits

### Patch et outils

- **Faster FireRed — DrMaple**  
  https://github.com/DrMaple/Faster-FireRed

- **MultiPatch — Sappharad (macOS)**  
  https://projects.sappharad.com/multipatch/

- **Rom Patcher JS — Marc Robledo**  
  https://www.marcrobledo.com/RomPatcher.js/

### Tracker

- **Fork français du Ironmon Tracker — TensaZangetsu22**  
  https://github.com/TensaZangetsu22/Ironmon-Tracker/tree/feature/french-complete-translation

- **Ironmon Tracker Gen 3 original — besteon**  
  https://github.com/besteon/Ironmon-Tracker

- **Guide d'installation du Tracker**  
  https://github.com/besteon/Ironmon-Tracker/wiki/Installation-Guide

### README

- 🇬🇧 [English README](README_EN.md)

---

## Crédits

- **DrMaple** — créateur du patch original Faster FireRed.
- **besteon et les contributeurs du Ironmon Tracker** — développement et maintenance du Tracker Gen 3.
- **TensaZangetsu22** — adaptation française du patch, modifications spécifiques de la version FR, écran titre et traduction française du Tracker.

Pokémon est une marque de Nintendo / Creatures Inc. / GAME FREAK inc.  
Ce projet est un projet communautaire non officiel et n'est affilié ni à Nintendo, ni à Creatures Inc., ni à GAME FREAK.
