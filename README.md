# テスト・成績 総合ボード

試験の準備から成績の報告までを一元管理するウェブアプリです。ファイルは `index.html` 1つだけです。

## 公開の手順（最初の1回）
1. GitHubで新しいリポジトリを作る（例：`seiseki-board`、Public）
2. `index.html` をリポジトリの一番上の階層にアップロードする（Add file → Upload files）
3. Settings → Pages → Source を「Deploy from a branch」、Branch を `main` / `(root)` にして Save
4. 数分後、`https://（ユーザー名）.github.io/（リポジトリ名）/` で開けるようになる

## どのPCからでも使う設定
1. GitHubの Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token
2. Repository access は「Only select repositories」でこのリポジトリだけを選ぶ
3. Permissions → Contents を「Read and write」にして作成し、表示されたトークンをコピーする
4. アプリの「設定」タブ → GitHubで同期 に、ユーザー名・リポジトリ名（自動で入ります）・トークンを入れて「保存して同期」

データはリポジトリの `data.json` に保存されます。別のPCでは、同じページを開いて、トークンを一度入力するだけです。

## 注意
- Publicリポジトリのため、`index.html` と `data.json` は誰でも読めます。生徒名など個人情報は入力しないでください。
- トークンは入力したPCのブラウザにだけ保存されます。他人に見せないでください。
- トークンを入れていないPCでは、最新のデータを閲覧できますが、変更はそのPCにしか保存されません。
- リンク集・マニュアルはアプリ上で追加・編集・削除でき、`data.json` に保存されます。
