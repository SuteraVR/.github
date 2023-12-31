# CONTRIBUTING GUIDE

This guide was written for Japanese-speaking contributors. If you are an English speaker and would like to contribute, please post on [GitHub Discussion in SuteraVR](https://github.com/SuteraVR/SuteraVR/discussions).

このガイドは日本語話者のコントリビューターの為に書かれました。もしもあなたが英語話者でコントリビュートしたい場合は[GitHub Discussion in SuteraVR](https://github.com/SuteraVR/SuteraVR/discussions)に投稿してください。

現在コントリビューティングガイドが作成しきれていない為、記述が及ばない点があるかもしれません。ご了承ください。コントリビューティングガイドについて改善点を考えついた場合は[GitHub Discussion in SuteraVR](https://github.com/SuteraVR/SuteraVR/discussions)に投稿してください。

## 開発フロー

開発フローは以下の様にしてください。

1. イシューを立てる
2. プルリクエストをイシューに関連付けて作成する
3. レビューを誰かから受ける
4. Approveを貰ったらマージする

### イシュー

- イシューは、[Conventional Commits:v1.0.0](https://www.conventionalcommits.org/ja/v1.0.0/)のタイトルと同じように名前を付けてください。
- イシューを立てる前には必ず同様のイシューが存在しない事を確認してください。もしもイシューの内容が被っていた場合には`Not Planned`としてイシューを閉じてください。

### ブランチ

- `{イシューの型}/{実装内容を簡潔に、かつハイフンで区切って記す}`のように作成してください。以下に例を記載します。
```txt
fix/rewrite-contributing-md
feat/add-clocking-server
docs/write-some-docs
```

### マイルストーン

- マイルストーンはバージョン毎に管理します。
- バージョン規則は[セマンティック バージョニング:v2.0.0](https://semver.org/lang/ja/)に従います。
- マイルストーンはサーバーとクライアントでは分けずに管理します。

### プルリクエスト

- プルリクエストは必ずイシューに関連づけて作成してください。関連づける方法は[GitHub Docs](https://docs.github.com/ja/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)を参照してください。以下にコメントの例を記載します。
```txt
- close #35

Fix typo in `CONTRIBUTING.md`.
```
- 現在パブリックベータである[Issueのためのブランチの作成機能](https://docs.github.com/ja/issues/tracking-your-work-with-issues/creating-a-branch-for-an-issue)は、コメントに`- close #35`のような記法を使用した場合にログが二個出現してしまうために使用しないでください。

### CI/CDの追加

- 現在存在するCIは、`cargo test`と`cargo fmt`、`cargo clippy`をそれぞれのRustクレートに対して走らせるもののみです。もしも他にCIを走らせるべきだと感じたならば、その点を纏めてイシューを作成してください。

## GitHub Discussions

[GitHub Discussion in SuteraVR](https://github.com/SuteraVR/SuteraVR/discussions)

## GitHub Projects

現在SuteraVRはGitHub Projectを活用しています。[SuteraVR's Project](https://github.com/orgs/SuteraVR/projects/1)
以下に注意事項を記載します。

- プルリクエストはイシューの欄にデフォルトで記載されているため、含める必要はありません。プルリクエストはProjectに登録しないでください。特に@haruki7049は気を付けてください。
