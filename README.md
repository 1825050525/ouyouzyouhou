# 応用情報技術者試験 学習リポジトリ

## 🎯 目標
- **午前試験：70〜80点以上**
- **午後試験：70〜80点以上**

## 👤 受験者プロフィール
| 項目 | 内容 |
|------|------|
| 開発経験 | 開発エンジニア 2年 |
| インフラ経験 | クラウドエンジニア 1年 |
| 保有資格 | AWS CLF / AIF / SAA / SOA / DVA / 基本情報技術者 |
| 学習環境 | GitHub + Claude Code |

---

## 📋 試験概要（2026年度版）

### ⚠️ 2026年度からの重要変更点
- **試験形式：ペーパー → CBT（Computer Based Testing）方式へ移行**
- **科目名称変更：午前 → 科目A、午後 → 科目B**
- 試験内容・出題形式・問題数・試験時間は変更なし
- 試験時期：前期（2026年11月頃）・後期（2027年2月頃）

### 試験構成

| 区分 | 時間 | 形式 | 問題数 | 合格基準 |
|------|------|------|--------|----------|
| 午前（科目A） | 150分 | 四肢択一 | 80問（全問必須） | 60点以上/100点 |
| 午後（科目B） | 150分 | 記述式 | 11問中5問選択（問1必須） | 60点以上/100点 |

### 午前問題 出題内訳
| 分野 | 問題数 | 割合 |
|------|--------|------|
| テクノロジ系（問1〜50） | 50問 | 62.5% |
| マネジメント系（問51〜60） | 10問 | 12.5% |
| ストラテジ系（問61〜80） | 20問 | 25% |

### 午後問題 選択戦略
- **問1（情報セキュリティ）：必須**
- **問2〜11：4問選択**

エンジニアバックグラウンドを活かした推奨選択分野：
1. 情報セキュリティ（必須）
2. ネットワーク
3. データベース
4. ソフトウェア設計 or アルゴリズム
5. プロジェクトマネジメント

---

## 📁 フォルダ構成

```
ap-study/
├── README.md                    # このファイル
├── 00_overview/                 # 試験概要・学習計画
│   ├── exam_overview.md         # 試験情報まとめ
│   ├── study_plan.md            # 学習計画（週次）
│   └── scoring_strategy.md     # 得点戦略
│
├── 01_morning/                  # 午前問題（科目A）カテゴリ別まとめ
│   ├── 01_basic_theory/         # 基礎理論
│   ├── 02_algorithms_data_structures/  # アルゴリズム・データ構造
│   ├── 03_computer_architecture/       # コンピュータ構成要素
│   ├── 04_os_middleware/               # OS・ミドルウェア
│   ├── 05_hardware/                    # ハードウェア
│   ├── 06_networks/                    # ネットワーク
│   ├── 07_databases/                   # データベース
│   ├── 08_information_security/        # 情報セキュリティ
│   ├── 09_system_development/          # システム開発
│   ├── 10_project_management/          # プロジェクトマネジメント
│   ├── 11_service_management/          # サービスマネジメント
│   ├── 12_system_audit/                # システム監査
│   ├── 13_management_strategy/         # 経営戦略
│   ├── 14_corporate_strategy/          # 企業戦略・ビジネス
│   └── 15_legal_ethics/                # 法規・倫理・標準化
│
├── 02_afternoon/                # 午後問題（科目B）分野別まとめ
│   ├── 01_security_required/    # 情報セキュリティ（必須）
│   ├── 02_software_design/      # ソフトウェア設計
│   ├── 03_algorithms/           # アルゴリズム
│   ├── 04_network/              # ネットワーク
│   ├── 05_database/             # データベース
│   ├── 06_embedded/             # 組込みシステム
│   ├── 07_information_systems/  # 情報システム
│   ├── 08_project_management/   # プロジェクトマネジメント
│   ├── 09_service_management/   # サービスマネジメント
│   ├── 10_system_audit/         # システム監査
│   └── 11_corporate_it_strategy/ # 企業と法務・IT戦略
│
├── 03_weak_points/              # 苦手問題まとめ（要復習）
│   ├── morning_weak.md          # 午前の苦手問題
│   └── afternoon_weak.md        # 午後の苦手問題
│
├── 04_tips_and_knowhow/         # 試験テクニック・ノウハウ
│   ├── morning_tips.md          # 午前の解き方・コツ
│   ├── afternoon_tips.md        # 午後の解き方・コツ
│   ├── time_management.md       # 時間配分戦略
│   └── exam_day_checklist.md    # 試験当日チェックリスト
│
├── 05_progress/                 # 進捗管理
│   ├── daily_log.md             # 日次学習ログ
│   ├── weekly_summary.md        # 週次サマリー
│   ├── mock_exam_results.md     # 模擬試験・過去問スコア
│   └── category_score.md        # カテゴリ別習熟度
│
└── 06_past_exam_analysis/       # 過去問傾向分析
    ├── trend_analysis.md        # 出題傾向分析
    └── frequently_wrong.md      # よく間違える問題パターン
```

---

## 🛠️ Claude Code での使い方

### 日々の学習フロー
```bash
# 1. 過去問を解く（ap-siken.com 等を活用）
# 2. 間違えた問題を記録
claude "午前問題でXXXについて間違えた。03_weak_points/morning_weak.md に追記して"

# 3. カテゴリ別まとめを充実させる
claude "01_morning/06_networks/ にTCP/IPの重要ポイントをまとめて"

# 4. 進捗を記録する
claude "今日の学習ログを05_progress/daily_log.md に追記して。午前80問中62点だった"
```

### 進捗確認
```bash
claude "05_progress/の内容をもとに今週の進捗をまとめて"
claude "03_weak_points/を分析して、優先的に復習すべきカテゴリを教えて"
```

---

## 📊 合格率・難易度
- 合格率：約25%（4人に1人）
- 偏差値：約65相当（TAC調べ）
- 推奨学習時間：200〜500時間（独学の場合）
- 合格者平均年齢：28歳

---

## 🔗 参考リソース
- [IPA公式 応用情報技術者試験](https://www.ipa.go.jp/shiken/kubun/ap.html)
- [応用情報技術者試験ドットコム（過去問）](https://www.ap-siken.com/)
- [シラバス Ver.7.2（最新）](https://www.ipa.go.jp/shiken/syllabus/gaiyou.html)

---

*最終更新：2026年4月*
