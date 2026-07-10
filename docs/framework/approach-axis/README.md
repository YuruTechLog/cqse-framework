# docs/framework/approach-axis/

Approach Axis Frameworkの実装ドキュメント群。

## このディレクトリの位置づけ

```
docs/knowledge/      ← 蒸留成果物（ログから抽出した知識。ログ単位）
docs/distillation/   ← 蒸留中間成果物（テーマ別・incident）
docs/chat-summary/   ← 意思決定サマリー（ログ単位）
docs/framework/      ← ← ここ。知識を統合した実装向けドキュメント
```

知識の流れ:
```
chat-archives（生ログ）
  → distillation（テーマ抽出）
  → knowledge（再利用可能な知識ユニット）
  → framework（実装ドキュメント）  ← このディレクトリ
```

## ファイル一覧

| ファイル | 内容 | 状態 |
|---------|------|------|
| `opus_prompt_framework_draft.md` | 分析依頼プロンプト（章立て・骨子ドラフト生成用） | 完成 |
| `sonnet_work_procedure.md` | Sonnet実行用の作業手順書（Fable 5作成。章立てスケルトン確定済み・Cokes接続C1〜C9整理済み） | 完成（人間レビュー待ち） |
| `cokes_definition_layer_proposal.md` | Cokes一言定義の4レイヤー分離統合 提案（M1/M2解消案） | 提案（人間承認待ち） |
| `framework_draft.md` | 章立て・骨子ドラフト | ドラフト（人間レビュー待ち） |

## 参照ソース（axis-log-01〜04）

**Primary（axis-log-01）:**
- `docs/knowledge/axis-log-01/approach-axis-framework.md`
- `docs/knowledge/axis-log-01/axis-words-magnet-map.md`
- `docs/knowledge/axis-log-01/gravity-tensor-model.md`

**Secondary（axis-log-02）:**
- `docs/knowledge/axis-log-02/integrated_knowledge.md`

**Tertiary（axis-log-03）:**
- `docs/knowledge/axis-log-03/integrated_knowledge.md`

**Quaternary（axis-log-04）:**
- `docs/knowledge/axis-log-04/integrated_knowledge.md`
  - AXIS5軸確定版・論文裏付けマップ・比喩体系・日本語3原則・コアメッセージ確定版・画像生成拡張
