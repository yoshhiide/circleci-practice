# CircleCIハンズオン

## 1. サンプルコードのFork
個人アカウントにforkしてください



## 2. ローカル確認用のcliをインストール
インストール

https://circleci.com/docs/ja/2.0/local-cli/

フォーマットバリデーション
`circleci config validate`




## 3. CircleCIダッシュボードからGitHubのリポジトリをプロジェクトに登録

ダッシュボードからプロジェクトに追加してください

https://app.circleci.com/projects/project-dashboard/github/{user-name}/




## 4. 設定ファイルを修正

### jobの複数実行(並列)
1. `.circleci/config.yml` を開く
2. jobを複数実行するように修正する
3. `circleci config validate` でフォーマットチェックする
4. GitHubにpushする (ワークフローが自動的に実行されます)

### jobの順次実行(直列)






### ブランチを条件とする





### CircleCIダッシュボード上でApproveしないと次のジョブが実行されないようにする



## 5. 環境変数について説明

環境変数はOrganizationにContextsとして共有利用できるものと、プロジェクト内でのみ参照できるものがあります。