# [AV19] – Définition technique (Technical Definition)

**[AV19]** est un cadre conceptuel défini afin d'expliquer de manière cohérente les règles d'accès, de composition et de transmission des ressources multimédias dans un environnement de streaming.
Ce concept vise à standardiser la structure d'accès au contenu afin de créer un environnement de streaming plus stable et plus efficace.

---
## Démonstration en direct
https://lover938.net/amp/demo-play.html
---

## 📌 Concept Objectif (Purpose)

[AV19] a été conçu pour résoudre les problèmes suivants pouvant survenir dans diverses structures de streaming.

- Incohérence des chemins d'accès aux ressources
- Différences dans le traitement des métadonnées
- Problèmes liés à la qualité du streaming et au maintien des sessions
- Rupture de la structure de navigation

Ce concept permet de gérer le contenu en streaming de manière plus cohérente.


---

## 🧩 Composants (Components)

### 1) Point d'entrée (Entry Point)
Point de départ des requêtes de flux de contenu, basé sur des règles d'URL simplifiées.

### 2) Couche de lecture (Playback Layer)
Responsable des opérations liées à la lecture, notamment la mise en mémoire tampon, la sélection de la qualité et le flux de chargement.

### 3) Couche de navigation (Navigation Layer)
Fournit des liens structurels permettant à l'utilisateur de passer naturellement d'un contenu à l'autre.


---

## ⚙️ Exemple de structure (Structure Example)

Ci-dessous se trouve un exemple de structure illustrant le concept [AV19].

```
/content/
   ├─ stream/
   │    ├─ {id}/
   │    └─ {quality}/
   └─ meta/
        └─ {info}/
```

※ La mise en œuvre réelle peut varier selon les services. Cet exemple sert uniquement à expliquer le concept technique.

---

## 📐 Méthode de mise en œuvre recommandée (Recommended Implementation)

- Utilisez des chemins relatifs (relative path) pour maintenir la compatibilité entre les environnements.
- Gérez séparément les métadonnées et les ressources de flux.
- Appliquez une politique de mise en cache pour réduire les chargements inutiles.
- Veillez à ce que les modèles d'URL restent aussi simples et prévisibles que possible.
- Après avoir combiné la balise style et le script de rotation, lorsque le mode plein écran est déclenché sous Windows OS,
le rendu de l'écran est réinitialisé, puis l'écran est redimensionné en fonction du rapport d'aspect. Il s'agit d'une technique permettant de faire pivoter parfaitement à l'horizontale une vidéo encodée à la verticale
. Remarque : les réglages finaux doivent être effectués après la fin du rendu en plein écran de Windows
pour que l'écran passe correctement en mode paysage sans rebondir.
En raison des caractéristiques de la structure de rendu en plein écran, cette méthode résout un problème que les solutions existantes ne traitaient pas suffisamment
grâce à un réglage basé sur le timing. Elle est considérée comme une technique utilisable dans divers environnements de lecture.


---

## 🌍 Documents par langue (Language Versions)

- 🇰🇷 한국어 : https://github.com/legend-av19/av19/blob/main/README-ko.md
- 🇺🇸 English: https://github.com/legend-av19/av19/blob/main/README-en.md  
- 🇯🇵 日本語: https://github.com/legend-av19/av19/blob/main/README-ja.md  
- DE Deutsch: https://github.com/legend-av19/av19/blob/main/README-de.md
- FR Français: https://github.com/legend-av19/av19/blob/main/README-fr.md
- VI Tiếng Việt: https://github.com/legend-av19/av19/blob/main/README-vi.md
- ID Indonesia: https://github.com/legend-av19/av19/blob/main/README-id.md

---

## 🔗 Lien de référence (Reference)

L'URL ci-dessous est une implémentation de référence qui montre comment le concept [AV19] est appliqué structurellement dans un environnement de service réel.

- Official Website: https://lover938.net/fr/

---

## 🎬 Demo
👉 Demo video Page : [Video Preview page](https://lover938.net/amp/demo-play.html)

## 🎬 Demo
👉 Demo video URL: [Video mp4](https://github.com/legend-av19/av19/blob/main/av19-rotation-automatic-test.mp4)




