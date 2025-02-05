# deploy_with_streamlit


# requirements.txt を更新　作成/更新
poetry self add poetry-plugin-export
poetry export -f requirements.txt --output requirements.txt --without-hashes  

# githubのレポジトリ作成
1. githubにてレポジトリを作成 (httpsのURLが表示されるのでそこに留まる。)
2. Personal access tokens (classic) を作成
3. cd C:\Users\jinno\Desktop\scope_verify\myproject
4. git init
5. git add -A
6. git commit -m "first commit"
7. git branch -m "main"
8. git status
9. https://[user_name]:[access_token]@github.com/palakpaneerer/scope_verify.git
10. git push -u origin main
* git remote remove origin # git remoteに誤ったgitをセットしてしまった場合

# githubの更新
1. git add -A
2. git commit -m "[comment]"
3. git push
