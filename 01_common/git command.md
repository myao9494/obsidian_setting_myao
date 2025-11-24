# 設定 (Configuration)
- `git config --global user.name "Your Name"`: ユーザー名の設定
- `git config --global user.email "you@example.com"`: メールアドレスの設定
- `git config --list`: 設定の確認


# ブランチとマージ (Branch & Merge)
- `git branch`: ブランチ一覧表示
- `git branch <name>`: ブランチ作成
- `git checkout <name>`: ブランチ切り替え (または `git switch <name>`)
- `git checkout -b <name>`: ブランチ作成して切り替え (または `git switch -c <name>`)
- `git merge <branch>`: ブランチをマージ
- `git branch -d <name>`: ブランチ削除

# 同期 (Sync)
- `git fetch`: リモートの変更を取得
- `git push origin <branch>`: 特定のブランチをリモートへ送信

# 一時退避
- `git stash`: 変更を一時退避
- `git stash pop`: 退避した変更を戻す

# コミットをなかったことに
- `git reset --soft HEAD~`: 直前のコミットを取り消す（変更は残る） ※Windows/Mac共通
- `git reset --hard HEAD~`: 直前のコミットを取り消す（変更も消える）
- `git reset --soft <commit-hash>`: 指定したコミットまで戻る（変更は残る）
- `git reset --hard <commit-hash>`: 指定したコミットまで戻る（変更も消える）
