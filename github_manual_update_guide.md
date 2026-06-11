# GitHub Manual Update Guide

このガイドは、GitHub 上で最後に目視確認する順番とチェック項目です。

## 0. GitHub アカウント bio

自動更新は token scope 不足で失敗しました。GitHub のプロフィール編集画面で以下を入れてください。

```text
iOS / Flutter を中心に、API連携・Supabase・README整備まで学習中の開発者志望です。
```

確認場所:

1. GitHub 右上のアイコン
2. Your profile
3. Edit profile
4. Bio 欄

## 1. Profile README

確認場所:

1. `https://github.com/estel1997`
2. プロフィール上部の README 表示

チェック:

- `estel1997` の README が表示されている
- Main Portfolio が上から順に表示されている
- Repository Guide のリンクが開ける
- `portfolio_cleanup_report.md` と `github_manual_update_guide.md` へのリンクがある

## 2. Pinned repositories

以下の順番で pin してください。

1. Blue-Archive_studentsQize
2. Blue-Archive_Quiz_Public
3. OKITOKU-
4. reversi_tutorial
5. Study_Code

pin から外す:

- Jump_king_Unity
- git_sample

## 3. Private 化確認

| Repository | Expected Visibility | Check |
|---|---|---|
| Jump_king_Unity | Private | GitHub 上で鍵マークを確認 |
| git_sample | Private | GitHub 上で鍵マークを確認 |

## 4. Main Portfolio 巡回順

### 4-1. Blue-Archive_studentsQize

確認すること:

- README が空ではない
- SwiftUI / MVVM / API / Supabase Ranking が説明されている
- docs がある
- `.github` テンプレートがある
- About:
  - `SwiftUI quiz app using external API, MVVM state management, URLSession, and Supabase ranking.`
- Topics:
  - `swift`, `swiftui`, `ios`, `mvvm`, `urlsession`, `api`, `supabase`, `portfolio`
- 既存の Supabase anon key が公開前提で問題ないか確認

### 4-2. Blue-Archive_Quiz_Public

確認すること:

- README の文字化けが解消されている
- Web / Supabase / Cloudflare Pages のポートフォリオとして説明されている
- docs がある
- `.github` テンプレートがある
- `.env.example` が placeholder だけになっている
- 既存の Supabase anon config が公開前提で問題ないか確認
- About:
  - `Fan-made quiz web app with JavaScript, Supabase/PostgreSQL, ranking, and Cloudflare Pages deployment.`
- Topics:
  - `javascript`, `html`, `css`, `supabase`, `postgresql`, `cloudflare-pages`, `quiz-app`, `portfolio`

### 4-3. OKITOKU-

確認すること:

- Flutter テンプレート README が残っていない
- 価格比較アプリ prototype として説明されている
- 実装済み、検証中、今後予定が分かれている
- docs/learning-notes.md がある
- `.github` テンプレートがある
- `.env.example` が placeholder だけになっている
- About:
  - `Flutter shopping price watch app prototype for store, product, and price comparison.`
- Topics:
  - `flutter`, `dart`, `mobile-app`, `price-tracker`, `supabase`, `firebase`, `portfolio`

## 5. Learning Repositories 巡回順

### 5-1. reversi_tutorial

確認すること:

- 完成アプリではなく SwiftUI ロジック学習 repo として説明されている
- README に盤面管理、合法手判定、石の反転が書かれている
- docs/game-logic.md がある
- About:
  - `SwiftUI reversi practice project focused on board state management and legal move detection.`

### 5-2. Study_Code

確認すること:

- Swift API 通信学習ログとして説明されている
- README に `URL` / `URLComponents` / `URLRequest` の役割がある
- docs/api-learning-map.md がある
- About:
  - `Swift API learning notes covering URL, URLComponents, URLRequest, JSONDecoder, and HTTP basics.`

## 6. 最終確認

- README が空ではない
- テンプレート文言が残っていない
- 実装済みと今後予定が混ざっていない
- API key / secret / token / service role key の実値が README / docs にない
- Supabase anon key / URL が公開前提の設計であり、RLS で守られている
- private 対象 repo が public に残っていない
- profile README が表示されている
- About / Topics が README 内容と一致している
