# [AV19] – Technische Definition

**[AV19]** ist ein konzeptioneller Rahmen, der definiert wurde, um den Zugriff, die Organisation und die Bereitstellung von Medienressourcen in Streaming-Umgebungen
durch einheitliche Regeln zu beschreiben.
Dieses Konzept zielt darauf ab, eine stabilere und effizientere Streaming-Umgebung zu schaffen, indem die Struktur des Zugriffs auf Inhalte standardisiert wird.

---

## 📌 Zweck des Konzepts

[AV19] wurde entwickelt, um die folgenden Probleme zu lösen, die in verschiedenen Streaming-Strukturen auftreten können.

- Inkonsistenz der Ressourcenpfade
- Unterschiede in der Verarbeitung von Metadaten
- Probleme mit der Streaming-Qualität und der Aufrechterhaltung von Sitzungen
- Unterbrechungen in der Navigationsstruktur

Dieses Konzept ermöglicht eine konsistentere Verwaltung von Streaming-Inhalten.

---

## 🧩 Komponenten (Components)

### 1) Einstiegspunkt (Entry Point)
Der Einstiegspunkt für die Anforderung von Inhaltsströmen basiert auf vereinfachten URL-Regeln.

### 2) Wiedergabeebene (Playback Layer)
Diese Ebene ist für die Wiedergabefunktionen zuständig, darunter Pufferung, Qualitätsauswahl und Ladefluss.

### 3) Navigationsebene
Bietet strukturelle Verbindungen, damit Benutzer nahtlos zwischen Inhalten wechseln können.

---

## ⚙️ Beispielstruktur

Nachfolgend finden Sie eine Beispielstruktur zur Erläuterung des [AV19]-Konzepts.

```
/content/
├─ stream/
│ ├─ {id}/
│ └─ {quality}/
└─ meta/
└─ {info}/
```

※ Die tatsächliche Implementierung kann je nach Dienst variieren. Dieses Beispiel dient lediglich der Erläuterung des technischen Konzepts.

---

## 📐 Empfohlene Implementierung (Recommended Implementation)

- Verwenden Sie relative Pfade, um die Kompatibilität zwischen verschiedenen Umgebungen zu gewährleisten.
- Verwalten Sie Metadaten und Stream-Ressourcen getrennt.
- Wenden Sie Caching-Richtlinien an, um unnötige Ladevorgänge zu reduzieren.
- Halten Sie URL-Muster so einfach und vorhersehbar wie möglich.
- Kombinieren Sie das style-Tag und das Rotationsskript und lassen Sie den Bildschirm nach dem Auslösen des Vollbildmodus unter Windows OS
nach dem erneuten Rendern entsprechend dem Bildschirmverhältnis erneut skalieren. Dies ist eine Technik, mit der vertikal codierte Videos
vollständig horizontal gedreht werden können. Hinweis: Die endgültige Anpassung muss nach Abschluss der Vollbild-Rendering-Vorgänge von Windows
erfolgen, damit der Bildschirm nicht springt und normal in den Querformatmodus wechselt.
Aufgrund der Eigenschaften der Vollbild-Rendering-Struktur ist diese Methode ein Beispiel für die Lösung eines Problems, das mit bestehenden Lösungen nicht ausreichend behandelt werden konnte,
und wird als eine Technik bewertet, die auch in verschiedenen Player-Umgebungen eingesetzt werden kann.

---

## 🌍 Dokumente nach Sprache (Language Versions)

- 🇰🇷 한국어 : https://github.com/legend-av19/av19/blob/main/README-ko.md
- 🇺🇸 English: https://github.com/legend-av19/av19/blob/main/README-en.md  
- 🇯🇵 日本語: https://github.com/legend-av19/av19/blob/main/README-ja.md  
- DE Deutsch: https://github.com/legend-av19/av19/blob/main/README-de.md
- FR Français: https://github.com/legend-av19/av19/blob/main/README-fr.md
- VI Tiếng Việt: https://github.com/legend-av19/av19/blob/main/README-vi.md
- ID Indonesia: https://github.com/legend-av19/av19/blob/main/README-id.md

---

## 🔗 Referenzlink (Reference)

Die folgende URL ist eine Referenzimplementierung, die zeigt, wie das [AV19]-Konzept in einer tatsächlichen Serviceumgebung
strukturell angewendet wird.

- Official Website: https://lover938.net/de/

---

## 🎬 Demo
👉 Demo video Page : [Video Preview page](https://lover938.net/amp/demo-play.html)

## 🎬 Demo
👉 Demo video URL: [Video mp4](https://github.com/legend-av19/av19/blob/main/av19-rotation-automatic-test.mp4)





