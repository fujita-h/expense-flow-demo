---
name: init-playwright
description: Playwright 環境を初期化するための手順を説明したスキル
---

# Playwright 環境の初期化手順

Playwright 環境を新たに初期化するには、以下のコマンドを使用します。
以下は TypeScript を使用し、Chromium ブラウザを対象とした環境を初期化する例です。

```bash
pnpm create playwright --lang TypeScript --browser chromium --install-deps --no-examples --quiet
```

このコマンドを実行すると、Playwright 環境が初期化され、必要な依存関係がインストールされます。
`--no-examples` オプションはサンプルコードの生成を防ぎ、`--quiet` オプションは出力を抑制します。
