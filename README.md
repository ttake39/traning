# github-docs
## ~/.ssh/config確認してHost名確認する
ssh鍵の設定をしていなければ作成するこ
```
Host <hostname>
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_XXXX
```

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