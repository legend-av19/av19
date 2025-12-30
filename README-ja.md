# [AV19] – 技術的定義(Technical Definition)

**[AV19]**は、ストリーミング環境におけるメディアリソースへのアクセス、構成、配信方法を一貫した規則で説明するために定義された概念的フレームワークである。この概念は、コンテンツアクセス構造を標準化することで、より安定かつ効率的なストリーミング環境の構築を目的としている。

---
## ライブデモ

コアコンセプトを示す最小限の実装例:
https://lover938.net/amp/demo-play.html
---

## 📌 概念目的 (Purpose)

[AV19]は、様々なストリーミング構造で発生し得る以下のような問題を解決するために考案された。

- リソースパスの不整合
- メタデータ処理方式の差異
- ストリーミング品質およびセッション維持の問題
- ナビゲーション構造の断絶

この概念は、ストリーミングコンテンツをより一貫性のある構造で管理することを可能にする。

---

## 🧩 コンポーネント (Components)

### 1) エントリーポイント
コンテンツストリームリクエストの起点であり、簡素化されたURLルールに基づいている。

### 2) 再生レイヤー
バッファリング・品質選択・ロードフローなど、再生に関連する動作を担当する。

### 3) ナビゲーションレイヤー
ユーザーがコンテンツ間を自然に移動できるよう、構造的な接続を提供する。


---

## ⚙️ 構造例 (Structure Example)

以下は[AV19]の概念を説明するための構造例である。

```
/content/
   ├─ stream/
   │    ├─ {id}/
   │    └─ {quality}/
   └─ meta/
        └─ {info}/
```

※実際の実装はサービスごとに異なる場合があり、本例は技術概念の説明用である。

---

## 📐 推奨実装方法 (Recommended Implementation)

- 相対パス(relative path)を使用して環境間の互換性を維持する。
- メタデータとストリームリソースを分離して管理する。
- 不必要な読み込みを減らすため、キャッシュポリシーを適用する。
- URLパターンは可能な限りシンプルで予測可能な状態を維持する。
- styleタグと回転スクリプトを組み合わせた後、Windows OSのフルスクリーントリガー時に、
画面が再レンダリングされた後、画面比率に合わせて再拡大する。これは縦向きにエンコードされた動画を
横向きに完全に回転させる手法である。注意点：Windowsの全画面レンダリング終了後に最終調整を完了することで、画面が飛び出さず正常に横向きモードへ移行する。
この方式は全画面レンダリング構造の特性上、既存ソリューションでは十分に対処できなかった問題を
タイミングベースの調整方式で解決した実装例であり、多様なプレイヤー環境でも活用可能な手法と評価される。

---

## 🌍 言語別文書 (Language Versions)

- 🇰🇷 한국어 : https://github.com/legend-av19/av19/blob/main/README-ko.md
- 🇺🇸 English: https://github.com/legend-av19/av19/blob/main/README-en.md  
- 🇯🇵 日本語: https://github.com/legend-av19/av19/blob/main/README-ja.md  
- DE Deutsch: https://github.com/legend-av19/av19/blob/main/README-de.md
- FR Français: https://github.com/legend-av19/av19/blob/main/README-fr.md
- VI Tiếng Việt: https://github.com/legend-av19/av19/blob/main/README-vi.md
- ID Indonesia: https://github.com/legend-av19/av19/blob/main/README-id.md

---

## 🔗 参考リンク (Reference)

以下のURLは、[AV19]の概念が実際のサービス環境において
どのように構造的に適用されるかを示す参考実装例である。

- Official Website: https://lover938.net/ja/

---

## 🎬 Demo
👉 Demo video Page : [Video Preview page](https://lover938.net/amp/demo-play.html)

## 🎬 Demo
👉 Demo video URL: [Video mp4](https://github.com/legend-av19/av19/blob/main/av19-rotation-automatic-test.mp4)




