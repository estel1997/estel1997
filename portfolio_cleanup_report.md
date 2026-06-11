# Portfolio Cleanup Report

作業日: 2026-06-12

## 対象リポジトリ

- Blue-Archive_studentsQize
- Blue-Archive_Quiz_Public
- OKITOKU-
- reversi_tutorial
- Study_Code
- Jump_king_Unity
- git_sample
- estel1997 profile README

## 対応したこと

### GitHub Profile README

- `estel1997/estel1997` を public repo として作成
- プロフィール README を追加
- Main Portfolio、Learning Projects、Learning Focus、Repository Guide、Career Goal を整理
- アカウント bio の自動更新を試行
- 結果: 失敗
- 理由: GitHub token に `user` scope がなく、`gh auth refresh -h github.com -s user` は認可待ちでタイムアウト

### Blue-Archive_studentsQize

- README.md を iOS ポートフォリオ向けに作成
- SwiftUI / MVVM / URLSession / JSONDecoder / Supabase Ranking を説明
- docs を追加
  - docs/architecture.md
  - docs/app-flow.md
  - docs/api-design.md
  - docs/learning-notes.md
  - docs/future-improvements.md
- `.github` テンプレートを追加
- `.gitignore` を追加
- GitHub About / Topics を更新

### Blue-Archive_Quiz_Public

- 文字化けしていた README.md を Web / Supabase ポートフォリオ向けに置換
- docs を追加
  - docs/architecture.md
  - docs/database-design.md
  - docs/deployment.md
  - docs/security-notes.md
  - docs/learning-notes.md
- `.github` テンプレートを追加
- `.gitignore` を追加
- `.env.example` を service role 前提から anon key placeholder に修正
- GitHub About / Topics を更新

### OKITOKU-

- 前回作成済み README が Flutter テンプレートではないことを再確認
- Flutter / Dart の価格比較アプリ prototype として説明されていることを確認
- docs/learning-notes.md を追加
- `.github` テンプレートを追加
- `.env.example` を追加
- GitHub About / Topics を更新

### reversi_tutorial

- README.md を SwiftUI ロジック学習 repo として作成
- docs を追加
  - docs/game-logic.md
  - docs/learning-notes.md
- `.gitignore` を追加
- GitHub About / Topics を更新

### Study_Code

- README.md を Swift API 通信学習ログとして更新
- docs を追加
  - docs/api-learning-map.md
  - docs/urlsession-notes.md
- `.gitignore` を追加
- GitHub About / Topics を更新

### Jump_king_Unity

- private 化を実行
- 実行コマンド:
  - `gh repo edit estel1997/Jump_king_Unity --visibility private --accept-visibility-change-consequences`
- 結果:
  - 成功

### git_sample

- private 化を実行
- 実行コマンド:
  - `gh repo edit estel1997/git_sample --visibility private --accept-visibility-change-consequences`
- 結果:
  - 成功

## セキュリティ確認

確認観点:

- API key
- secret
- token
- service role
- password
- Bearer
- Supabase URL / anon key
- Firebase
- OpenAI
- JWT

確認結果:

- README / docs には API key、secret、token、service role key、個人情報の実値を追加していない
- Blue-Archive_studentsQize の Swift コード内に既存の Supabase anon key / project URL があるため、RLS と公開範囲の最終確認が必要
- `.env.example` には placeholder のみを記載

## 手動対応が必要なこと

- GitHub account bio の更新
- Pinned repositories の並び替え
- 各 repo の画面上で About / Topics / README 表示を最終確認
- Blue-Archive_studentsQize の Supabase anon key が公開前提で問題ないか確認
- スクリーンショットや demo URL は必要に応じて後日追加
