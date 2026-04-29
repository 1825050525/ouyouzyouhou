# 応用情報技術者試験 学習リポジトリ

## 🎯 目標
**2026年11月 前期試験 一発合格（午前・午後ともに75点以上）**

## 📋 試験概要
| 項目 | 内容 |
|------|------|
| 試験名 | 応用情報技術者試験（AP） |
| 2026年度の方式 | CBT（Computer Based Testing） |
| 科目A（旧午前） | 四肢択一 80問 150分 |
| 科目B（旧午後） | 記述式（キーボード入力）11問中5問選択 150分 |
| 合格基準 | 科目A・B ともに60点以上 |
| 前期試験予定 | 2026年11月頃 |

## 🤖 Claude Code エージェント構成

| エージェント | 役割 |
|------------|------|
| **PM** | 進捗記録・スケジュール管理・マイルストーン監視 |
| **チューター** | 概念解説・過去問解説・苦手克服アドバイス |
| **試験戦略アドバイザー** | 得点戦略・選択分野最適化・本番シミュレーション |
| **コンテンツ作成** | カテゴリ別まとめ・解説ページの自動生成 |
| **レビュアー** | 午後記述の採点・フィードバック・模範解答提示 |

## 📁 フォルダ構成

```
ouyouzyouhou/
├── CLAUDE.md                    ← Claude Code設定（エージェント・スキル定義）
├── README.md                    ← このファイル
├── .claude/
│   ├── agents/                  ← サブエージェント定義
│   │   ├── pm.md                ← PM（進捗管理）
│   │   ├── tutor.md             ← チューター
│   │   ├── strategist.md        ← 試験戦略アドバイザー
│   │   ├── content_creator.md   ← コンテンツ作成
│   │   └── reviewer.md          ← レビュアー（記述採点）
│   └── skills/
│       ├── log_progress.md      ← 進捗記録スキル
│       ├── add_weak_point.md    ← 苦手登録スキル
│       ├── generate_summary.md  ← まとめ生成スキル
│       └── score_exam.md        ← 模試採点スキル
├── 00_overview/                 ← 試験概要・学習計画・戦略
├── 01_morning/                  ← 科目A カテゴリ別まとめ（15カテゴリ）
│   ├── 01_basic_theory/
│   ├── 02_algorithms_data_structures/
│   ├── 03_computer_architecture/
│   ├── 04_os_middleware/
│   ├── 05_hardware/
│   ├── 06_networks/             ← ★重点（AWS経験活用）
│   ├── 07_databases/            ← ★重点（開発経験活用）
│   ├── 08_information_security/ ← ★最重点（必須・午後直結）
│   ├── 09_system_development/
│   ├── 10_project_management/   ← ★重点（午後選択）
│   ├── 11_service_management/   ← ★重点（午後選択）
│   ├── 12_system_audit/
│   ├── 13_management_strategy/
│   ├── 14_corporate_strategy/
│   └── 15_legal_ethics/
├── 02_afternoon/                ← 科目B 分野別まとめ（選択5分野）
│   ├── 01_security_required/    ← ★必須
│   ├── 02_software_design/
│   ├── 03_algorithms/
│   ├── 04_network/              ← ★選択
│   ├── 05_database/             ← ★選択
│   ├── 06_embedded/
│   ├── 07_information_systems/
│   ├── 08_project_management/   ← ★選択
│   ├── 09_service_management/   ← ★選択
│   ├── 10_system_audit/
│   └── 11_corporate_it_strategy/
├── 03_weak_points/              ← 苦手問題まとめ（要復習）
│   ├── morning_weak.md
│   └── afternoon_weak.md
├── 04_tips_and_knowhow/         ← 試験ノウハウ・コツ
├── 05_progress/                 ← 進捗管理
│   ├── daily_log.md
│   ├── weekly_summary.md
│   ├── mock_exam_results.md
│   └── category_score.md
└── 06_past_exam_analysis/       ← 過去問傾向分析
```

## ⚠️ 個人情報ポリシー
- 氏名・企業名・所属・連絡先等は**一切記載しない**
- パスワード・APIキー・トークン等は**絶対に記載しない**
- 職場名・学校名・プロジェクト名等の固有名詞は記載しない
- 記録してよいのはスコア・日付・学習内容のみ

## 🔗 参考リソース
- [IPA公式](https://www.ipa.go.jp/shiken/kubun/ap.html)
- [過去問演習（ap-siken.com）](https://www.ap-siken.com/)
