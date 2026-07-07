# dataset knowledge: axis-log-01

## データセット概要
- ログセット: axis-log-01
- 対象: memo01〜memo09
- RUN_ID: 01
- 実行日: 2026-07-07

---

## このデータセットが持つ知識

axis-log-01は「Approach Axisという概念が生まれ、構造化され、命名され、Cokesの道具として位置づけられた」全過程を記録している。

単なる設計ドキュメントではなく、**設計の揺れ・失敗・修正・確定のリアルタイム記録**。

---

## 確定した知識ユニット（再利用可能）

| 知識ユニット | ファイル | 状態 |
|------------|---------|------|
| Approach Axis Framework全体 | `approach-axis-framework.md` | 確定 |
| 軸語彙5分類・磁力マップ・モデル特性 | `axis-words-magnet-map.md` | 確定 |
| 重力場テンソルモデル | `gravity-tensor-model.md` | 確定（Gemini承認済み） |
| Cokes設計思想・三原則・位置づけ | `cokes-design-philosophy.md` | 思想確定・三原則は草案 |

---

## インシデントから得た教訓（dataset-wide）

| インシデント | 教訓 |
|------------|------|
| 迎合問題（ユーザーの軸に乗り続ける） | 名前設計・概念設計には摩擦が必要 |
| CopilotのCokes/Axis混同 | Cokesと道具（Axis）の分離を明示する必要性 |
| 概念説明優先で操作設計が薄くなった | 概念と操作は同時設計する |
| Gemini批判（言いすぎ・比喩的すぎ） | 批判を全否定せず取り込むことで精度向上 |
| memo06の2540行・memo09の2439行 | 長大ログは分割読込が必要（ツール制約） |

---

## このログセット固有の文脈

- **Copilotとの対話が多い**：Copilot地形分析の精度はCopilot利用実績の反映
- **Geminiの敵対レビューを意図的に実施**：批判取り込みがフレームワーク精度を上げた
- **命名プロセスが残っている**：Approach確定までのSyncからの過程全体が記録
- **Cokes三原則は草案止まり**：このログセット内で確定には至っていない

---

## 次ログセット（axis-log-02等）があれば参照すべき項目

1. Cokes三原則の確定状況
2. Approach Axisの実際の使用例
3. Layer4テンプレートの運用状況
4. Cokesの理念文書の存在

---

## 参照関係

```
dataset_knowledge.md（本ファイル・全体俯瞰）
  ├─ approach-axis-framework.md（実務で使うフレームワーク）
  ├─ axis-words-magnet-map.md（操作語彙と効力の参照表）
  ├─ gravity-tensor-model.md（なぜ効くかの説明モデル）
  └─ cokes-design-philosophy.md（Cokesの思想とAxisの位置づけ）

蒸留ドキュメント（詳細）
  ├─ docs/distillation/axis-log-01/01_log_topics.md
  ├─ docs/distillation/axis-log-01/01_incident.md
  └─ docs/distillation/axis-log-01/01_integrated_summary.md

意思決定サマリー
  ├─ docs/chat-summary/axis-log-01_01/memo01-04_summary.md
  ├─ docs/chat-summary/axis-log-01_01/memo05-07_summary.md
  └─ docs/chat-summary/axis-log-01_01/memo08-09_summary.md
```
