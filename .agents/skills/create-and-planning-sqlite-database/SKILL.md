---
name: create-and-planning-sqlite-database
description: SQLite データベースを扱う際の手順やTipsのスキルです。
---

# 使用するパッケージについて
`node` の環境で SQLite データベースを扱うには、通常 `sqlite3` パッケージを使用しますが、
`node`のバージョンが `v22.5.0` 以降であれば、ネイティブの `node:sqlite` モジュールを使用することもでき、`v22.16.0` 以降では安定版として利用可能です。

最新の情報は `https://nodejs.org/docs/latest-v22.x/api/sqlite.html` を参照してください。

# 初期化や初期データの投入について
SQLite データベースを初期化したり、初期データを投入する際には、`ts` ではなく `js` ファイルでスクリプトを作成することを許可します。
これは、`ts-node` を使用する必要がなくなり、環境構築が簡素化されるためです。
