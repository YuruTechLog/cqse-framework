# log_topics: tide-logs-01 / log02

## テーマ一覧

### T-01: ファイル構成設計
- public/disclaimer/ 配下にトーン別免責画像を配置
- loader.min.js / config.json / data.json / README / LICENSE で一式完結
- 設置者が必要なファイルをそのまま使える構成

### T-02: config.jsonスキーマ確定
- `disclaimer`: トーン識別子（strict/neutral/soft/light）
- `disclaimerPosition`: 表示位置（top/bottom）
- `disclaimerId`: DOM挿入先ID
- `autoLoadData`: data.json自動取得フラグ

### T-03: 免責文4トーン確定
- strict: 厳格表現（法的リスク最小化）
- neutral: 中立表現（標準推奨）
- soft: 柔らか表現（個人・趣味向け）
- light: 最小表現（開発・テスト向け）

### T-04: loader.min.js起動フロー
1. config.json fetch
2. 免責トーン確認
3. 免責画像DOMに挿入
4. data.json fetch
5. renderData（スコア・ラベル・まとめ文・最終更新時刻展開）
- 免責確認とデータ展開をセットで実行する構造

### T-05: 設置者向け警告文
- 免責が未選択（config.jsonのdisclaimerがnull/未設定）時に警告表示
- data.json展開を停止し設置者に設定を促す

### T-06: LICENSE追加条項
- 免責表示の保持を強く推奨
- ただし法的強制力はなし（削除も技術上可能）
- 心理的拘束力による抑止が目的

### T-07: 作業単位とマイルストーン
- デザイン → 実装 → 難読化 → README整備 → テスト → リリース
- 各フェーズを独立した作業単位として管理
