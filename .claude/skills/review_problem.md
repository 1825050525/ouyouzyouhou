# スキル：問題レビュー記録（review_problem）

## 概要
ユーザーが問題文・解説・正誤・難易度を貼り付けたとき、
復習用サマリーを自動生成して適切なファイルに追記するスキル。

## トリガー
ユーザーが以下をまとめて送ってきたとき：
- 問題文（全文）
- 解説文（全文）
- 正誤：「正解」or「不正解」
- 難易度：「難」「中」「易」

## 処理手順

### 1. カテゴリを判定して保存先を決める

| カテゴリ | 保存先 |
|---------|--------|
| セキュリティ | `01_morning/08_information_security/summary.md` |
| ネットワーク | `01_morning/06_networks/summary.md` |
| データベース | `01_morning/07_databases/summary.md` |
| アルゴリズム・データ構造 | `01_morning/02_algorithms_data_structures/summary.md` |
| OS・ミドルウェア | `01_morning/04_os_middleware/summary.md` |
| コンピュータ構成 | `01_morning/03_computer_architecture/summary.md` |
| ハードウェア | `01_morning/05_hardware/summary.md` |
| 基礎理論 | `01_morning/01_basic_theory/summary.md` |
| システム開発 | `01_morning/09_system_development/summary.md` |
| プロジェクトマネジメント | `01_morning/10_project_management/summary.md` |
| サービスマネジメント | `01_morning/11_service_management/summary.md` |
| システム監査 | `01_morning/12_system_audit/summary.md` |
| 経営戦略 | `01_morning/13_management_strategy/summary.md` |
| 法規・倫理 | `01_morning/15_legal_ethics/summary.md` |

### 2. サマリーを以下フォーマットで生成して末尾に追記

```markdown
---
## [トピック名]｜★難/中/易｜✅正解 or ❌不正解｜YYYY-MM-DD

### 概要
（何を問う問題か、1〜2文で）

### ポイント
- （重要な概念・定義を箇条書き、3〜5個）

### 要点（これだけ覚える）
> （試験で即答するために必要な核心、1〜2行）

### ひっかかりやすい罠
- （間違いやすいポイント、あれば）
---
```

### 3. 不正解だった場合は追加で weak_points にも記録

保存先：`03_weak_points/morning_weak.md`

```markdown
## [トピック名]｜★難/中/易｜YYYY-MM-DD

- カテゴリ：[カテゴリ名]
- 間違えた理由：（解説から読み取って推定）
- 復習ポイント：（summary.md の該当エントリを参照）
```

## 注意事項
- 問題文・解説をそのまま転記しない（著作権対応）
- 自分の言葉で概念を要約して記録する
- ファイルが存在しない場合は新規作成する
