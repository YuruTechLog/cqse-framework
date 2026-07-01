# Glossary

単語を整理しよう。
学問分野別にまとめると分かりやすいらしい。


> Cokesで利用する概念・用語をまとめた用語集。
>
> 本書は新しい概念を定義することを目的とせず、既存の学術・技術分野で用いられている概念を、Cokesの文脈で整理・位置付けることを目的とする。

---

# 1. Cokes

## Cokes

...

## Context

...

## Context Engineering

...

## Skill

...

## Knowledge Asset

...

## Distillation

...

## Repository

...

## Pipeline

...

---

# 2. AI

## LLM

...

## Prompt

...

## Prompt Engineering

...

## Context Window

...

## RAG

...

## AI Agent

...

## MCP

...

---

# 3. 認知科学

## 認知負荷（Cognitive Load）

人が情報を理解・処理する際に必要となる認知資源の量。

Cokesでは、Knowledge AssetやSkillの粒度、Contextの設計に影響する重要な概念として扱う。

---

## ワーキングメモリ（Working Memory）

人が短時間に保持・処理できる情報領域。

---

## 長期記憶（Long-term Memory）

経験や知識を長期間保持する記憶。

---

## 認知的オフローディング（Cognitive Offloading）

外部ツールへ記憶や思考を委譲し、人間の認知負荷を軽減する考え方。

Repositoryは認知的オフローディングを支援する仕組みとして機能する。

---

## 分散認知（Distributed Cognition）

人間・道具・環境を含めた全体で認知活動を行うという考え方。

Cokesでは、人間・Repository・AIを一つの認知システムとして捉える。

---

# 4. 知識工学

## ナレッジマネジメント

...

## 知識表現（Knowledge Representation）

...

## オントロジー

...

## タクソノミー

...

---

# 5. ソフトウェア工学

## 関心の分離（Separation of Concerns）

...

## DRY

...

## Single Source of Truth

...

## 単一責任の原則（SRP）

...

## モジュール性

...

---

# 6. 情報アーキテクチャ

## 情報設計

...

## メタデータ

...

## 分類体系

...

## ナビゲーション

...

---

# 7. 運用

## Workflow

...

## Repository

...

## Versioning

...

## Traceability

...









# Cokes Glossary

> 本書は Cokes で使用する用語の定義をまとめたものである。
> 用語の解説や背景思想については `philosophy.md`、実装方法については `specification.md` を参照する。

---

## Cokes   ※AIつくったまんま、、、なんかちがう

Cognitive Key Output Engineering System

Context Engineering を中心とした Knowledge Management Framework。

知識を整理・再利用し、人間とAIの協調による継続的な成果創出を支援することを目的とする。


## AI

自然言語を理解し、指示に従って推論・生成・実行を行う大規模言語モデル（LLM）およびその実行環境。

---

## Context

AIがタスクを実行するために入力される情報の総体。

プロンプトだけでなく、Skill、Knowledge Asset、Memory、実行条件など、AIの判断に影響するすべての情報を含む。

---

## Context Engineering

目的に応じて最適な Context を設計・構築・供給する技術および設計手法。

Cokes が対象とする中核領域。

---

## Prompt

AIへ直接与える自然言語による指示。

Prompt は Context を構成する一要素であり、Context 全体を表すものではない。

---

## Skill

再利用可能な知識・手順・制約・ノウハウをまとめた実行単位。

Skill は複数のタスクから参照されることを前提として設計される。

---

## Knowledge Asset

再利用可能な知識資産。

記事、テンプレート、設計資料、チェックリスト、会話ログの蒸留結果などを含む。

---

## Distillation

会話・試行錯誤・経験から再利用可能な Knowledge Asset を抽出・整理するプロセス。

---

## Memory

継続的に利用される知識や状態。

AIが長期的に参照する情報を保持する仕組みを指す。

---

## Pipeline

Context を組み立て、AIへ供給し、成果物を生成するまでの一連の処理。

---

## Repository

Knowledge Asset、Skill、テンプレート、設定などを管理する保存構造。

---

## Workflow

人間とAIが協調して成果物を作成する作業の流れ。

Pipeline がシステム視点であるのに対し、Workflow は運用視点を表す。

---

## Human

目的を定義し、意思決定を行い、成果物の品質に責任を持つ主体。

---

## Cognitive Load（認知負荷）

人間が情報処理を行う際に消費する認知資源の量。

Cokesでは、Context設計やKnowledge Assetの粒度を決定する重要な設計指標として扱う。

---

## Working Memory（ワーキングメモリ）

人間が短時間保持・処理できる情報領域。

AIとの協調設計では、人間側のWorking Memoryを圧迫しないKnowledge構造が望ましい。

---

## External Memory

人間の外部に存在する記憶。

ノート、Repository、Skill、Knowledge Assetなどを含む。

CokesではRepositoryはExternal Memoryとして機能する。

---

## Abstraction（抽象化）

複数の具体例から本質を抽出し、再利用可能な知識へ変換する行為。

---

## Knowledge Management

知識を生成・蓄積・共有・再利用するための体系。

CokesはKnowledge Management Frameworkとして位置付けられる。

---

## Context Window

AIが一度に扱える入力範囲。

Context Engineeringでは重要な制約条件となる。

---

## Cognitive Offloading

人間の認知負荷を外部システムへ委譲すること。

RepositoryやKnowledge Assetはそのための仕組みとして機能する。
