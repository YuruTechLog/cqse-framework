# Cokes : Cognitive Key-Output Engineering System（出力品質工学）

Cokesは、楽して、いいモノを作るために、人間が道具・仕組みを選択して用いる工程を設計・運用するフレームワークです。

人・品質・コストの条件を踏まえ、
必要なKey-Outputを無理なく実現できる工程を設計・運用することを目的としています。

「コークス(Cokes)」は、化石燃料のコークス（cokes）を意識して決めた。
認知負荷の過剰摂取で燃え尽きる（バーンアウトする）人間が少しでも減るように、という燃料（リソース）への願いを込めている。

※旧記載「CQSE」、ドイツのTech企業と同じ名前と気づいてリファクタ実施

---

このプロジェクトは以下で構成されています。

- 理念 → philosophy.md
- 用語 → glossary.md
- Cokes版仕様（第1版） → specification.md
- CQSE期の仕様・問題提起 → specification_cqse.md（履歴として保持）
- 参考文献 → references.md
- Approach Axis Framework → docs/framework/approach-axis
- 生ログなど → docs

まずは philosophy.md を読むことで、全体像がつかめます。

---

## 📂 リポジトリ構成（Sitemap）

```text
cokes/
├── LICENSE
├── README.md
├── philosophy.md
├── specification.md
├── specification_cqse.md
├── glossary.md
├── references.md
├── docs/
│   ├── chat-archives/     生ログ（axis-log-01〜04, cqse-log-01, tide-logs-01）
│   ├── chat-summary/      生ログの要約
│   ├── distillation/      要約からのテーマ抽出（incident / log_topics / workflow）
│   ├── knowledge/         テーマ抽出からの再利用可能な知識ユニット
│   ├── framework/         知識を統合した実装ドキュメント
│   │   └── approach-axis/ Approach Axis Framework（README.mdあり）
│   └── note-draft/        note公開用ドラフト
└── tools/                 ログ変換などの作業ツール（README.mdあり）
    ├── cli/
    └── log_transformation/
