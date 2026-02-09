# レポジトリのガイドライン
以下のガイドラインに従ってください。

## 使用する言語
- Node.js と TypeScript を使用します。
- Next.js を使用してフロントエンドとバックエンドを構築します。

## パッケージ管理
- pnpm を使用します。
  - 必要なパッケージは `pnpm add <package-name>` で追加してください。
  - その他の pnpm コマンドも `pnpm <command>` の形式で実行してください。
- Install, Dev, Build, Lint, Test なども pnpm のスクリプトとして package.json に定義してください。

## コードフォーマット
- biome をコードフォーマットに使用します。
