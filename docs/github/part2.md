# Git戦略

## __[概要]__

案件ごとに最適なGit運用は異なりますが、判断の“軸”を持って選ぶことが重要です。<br>
ここでは**基本方針 → 戦略の選び方 → 具体例（2環境/3環境・リリース/ホットフィックス）**の順でまとめます。

![概要](../img/png/git.png "概要図")

## 基本方針

- Branch役割と命名規約

    - master = 公開環境

    - staging = 結合テスト

    - feature/* = 新規開発

    - fix/* = 計画的 BugFix

    - hotfix/* = 緊急 BugFix<br>※<span style="color:red">Masterへの直Pushあり</span>

    - releases/yyyy-mm-dd = Release

- 禁止事項

    - `master` / `staging` への<span style="color:red">直コミット・強制Push</span>は禁止とする

- 共通

    - `PR`は最低1~2名の承認を必須とする

## masterについて
- 目的：本番の単一の真実源（リリース済みの安定状態）

- 更新元：releases/* と hotfix/* のみをマージ 

- デプロイ：masterマージ

- 保護：レビュー必須・ステータスチェック必須・管理者の直push禁止。

## stagingについて

## featureについて

## hotfixについて
    