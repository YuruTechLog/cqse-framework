# Cokes Execution Template

---

## ■ 対象ログ
- パス：{LOG_PATH}
- ログセット名：{DATASET_NAME}

例：
- docs/chat-archives/tide-logs-01/
- tide-logs-01

---

# ■ Phase1：ログ解析（Log Scan）

## やること
- [ ] 全ログを横断的に読む
- [ ] テーマを抽出する

## 出力
- log_topics（テーマ一覧）

## メモ
{PHASE1_NOTES}

---

# ■ Phase2：Distillation生成（構造化）

## やること
- [ ] テーマを統合する
- [ ] 重複を削除する
- [ ] 構造として整理する

## 出力ファイル
- {NN}_log_topics.md
- {NN}_incident.md
- {NN}_distillation-workflow.md

## メモ
{PHASE2_NOTES}

---

# ■ Phase3：Summary生成（意思決定整理）

## やること
- [ ] 意思決定・判断の流れを整理する
- [ ] 重複した説明を統合する
- [ ] 時系列を維持する

## 出力
- chat-summary/{DATASET_NAME}_{NN}

## メモ
{PHASE3_NOTES}

---

# ■ Phase4：Knowledge生成（再利用化）

## やること
- [ ] distillation + summary を統合する
- [ ] テーマ別に再構造化する
- [ ] 再利用可能な形にする

## 出力
- knowledge/{DATASET_NAME}/

## メモ
{PHASE4_NOTES}

---

# ■ 制約（絶対ルール）

- ログ外情報は禁止
- 推測は禁止
- 重複は統合する
- 時系列は維持する
- 高校生でも読める表現にする
- 事実と考察は分離する（考察はLLM総括）

---

# ■ 優先順位

1. 忠実性（ログ準拠）
2. 再利用性（使える形）
3. 構造の明確さ（理解しやすさ）

---

# ■ 実行チェックリスト

実行前に確認：

- [ ] 対象ログは明確か
- [ ] Phase1でテーマ抽出できているか
- [ ] distillationとsummaryの役割が混ざっていないか
- [ ] knowledgeが再利用可能か

---

# ■ 補足（必要な場合のみ）

{EXTRA_NOTES}
