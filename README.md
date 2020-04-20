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




## 4. 設定ファイルを修正(練習)

### 1. jobの複数実行(並列)
1. `.circleci/config.yml` を開く
2. jobを複数実行するように修正する(goodbye-workflowを追加し、echo "goodbye!"を実行する)
3. `circleci config validate` でフォーマットチェックする
4. GitHubにpushする (ワークフローが自動的に実行されます)

### 2. echoの値を変更する

パラメータを与えるようにし、
echo "Hi!"にしてみる。

### 3. jobの順次実行(直列)

goodbye-workflowをhello-workflowが実行された後に実行されるようにする

### 4. ブランチを条件とする

特定のブランチに合致する場合や、合致しない場合にのみワークフローが実行されるようにする

### 5. CircleCIダッシュボード上でApproveしないと次のジョブが実行されないようにする



## 5. 環境変数について説明

環境変数はOrganizationにContextsとして共有利用できるものと、プロジェクト内でのみ参照できるものがあります。
