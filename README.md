# Mintlify ドキュメンテーション

このリポジトリは、Mintlifyを使用したドキュメンテーションプロジェクトです。

## 概要

このプロジェクトには以下の要素が含まれています：

- ガイドページ
- ナビゲーション設定
- カスタマイズ設定
- APIリファレンスページ
- 一般的なコンポーネントの使用例

## 開発環境のセットアップ

1. Mintlify CLIのインストール:
```bash
npm i -g mintlify
```

2. ローカル開発サーバーの起動:
```bash
mintlify dev
```

## 開発フロー

### メインブランチでの直接作業（小規模な更新の場合）

1. リポジトリのクローン:
```bash
git clone [リポジトリURL]
cd mintlify
```

2. 最新の状態に更新:
```bash
git pull origin main
```

3. 必要なパッケージのインストール:
```bash
npm install
```

4. ローカル環境での開発:
```bash
mintlify dev
```

5. 変更の即時反映:
```bash
git add .
git commit -m "変更の説明"
git push origin main
```

### フィーチャーブランチでの作業（大規模な更新の場合）

1. リポジトリのクローン:
```bash
git clone [リポジトリURL]
cd mintlify
```

2. 開発用ブランチの作成:
```bash
git checkout -b feature/[機能名]
```

3. 必要なパッケージのインストール:
```bash
npm install
```

4. ローカル環境での開発:
```bash
mintlify dev
```

5. 変更の保存とプッシュ:
```bash
git add .
git commit -m "変更の説明"
git push origin feature/[機能名]
```

6. クイックマージの手順:
   - GitHubのリポジトリページでプルリクエストを作成
   - 変更内容を簡潔に説明
   - 問題がなければ即時マージを実行
   - マージ後、フィーチャーブランチを削除

## ファイル更新方法

1. `docs/` ディレクトリ内のMarkdownファイルを編集
2. 変更をGitリポジトリにプッシュ
3. 自動的にデプロイが実行されます

## トラブルシューティング

- **Mintlify devが起動しない場合**
  - `mintlify install` を実行して依存関係を再インストール
  
- **404エラーが表示される場合**
  - `mint.json` ファイルが正しいディレクトリにあることを確認

## ディレクトリ構造

- `docs/`: ドキュメントのメインディレクトリ
  - Markdownファイル（.md, .mdx）
  - 画像ファイル
  - 設定ファイル（mint.json）

## 注意事項

- 変更を加える前に必ずローカルで確認してください
- `mint.json` の設定を変更する際は慎重に行ってください
- 画像ファイルは `docs/images/` ディレクトリに配置してください
- 小規模な更新はメインブランチで直接作業可能です
- 大規模な更新は機能ブランチを作成してください
- コミットメッセージは具体的で分かりやすい内容にしてください
- 問題がなければ即時マージを心がけてください 