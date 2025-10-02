# github-docs

# GitHub Commit Messageのプレフィックスルール
- feat: 新機能
- fix: バグ修正
- docs: ドキュメント変更
- style: フォーマット変更
- refactor: 構造変更
- test: テスト関連の変更
- chore: ビルドプロセスや依存関係の変更
- pref: パフォーマンス改善
- ci: CI/CDに関連する変更

---

## ~/.ssh/config確認してHost名確認する
ssh鍵の設定をしていなければ作成するこ
```
Host <hostname>
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_XXXX
```

---

## 初期設定
```
echo "# github-docs" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@[hostname]:[own]/github-docs.git
git push -u origin main
```