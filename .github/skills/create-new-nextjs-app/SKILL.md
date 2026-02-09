---
name: create-new-nextjs-app
description: 新たにnext.jsアプリケーションを作成するときに使用するスキル
---

next.jsアプリケーションを新たに作成するには、以下のコマンドを使用します。

```bash
npx create-next-app@latest [project-name] [options]
```

このとき、`project-name` のフォルダが生成され、その中にnext.jsアプリケーションの雛形が作成されます。
すでにプロジェクトのフォルダが存在する場合は、`project-name` を `.` にすることで、
現在のディレクトリにnext.jsアプリケーションを作成することもできます。

ただし、この時、現在のディレクトリが空である必要がありますが、
フォルダが空でない場合は、新規フォルダで作成して、後で必要なファイルを移動させる方法もあります。
したがって、以下のような手順で進めることができます。
移動の際には、不要なファイルを削除することを忘れないでください。

```bash
npx create-next-app@latest [project-name] [options]
rm -rf [project-name]/.next
rm -rf [project-name]/node_modules
rm -rf [project-name]/.gitignore
mv [project-name]/* .
mv [project-name]/.* .
rmdir [project-name]
```

## オプションについて

`https://nextjs.org/docs/app/api-reference/cli/create-next-app` に記載されているオプションを使用することで、
プロジェクトの設定をカスタマイズすることができます。

特に指定がない限り、以下のオプションを使用して初期化してください。

`--ts` : TypeScriptを使用する設定  
`--tailwind` : Tailwind CSSを使用する設定
`--biome` : Biomeを使用する設定  
`--app` : App Routerを使用する設定  
`--use-pnpm` : パッケージマネージャーにpnpmを使用する設定  
`--no-react-compiler` : React Compilerを使用しない設定  
`--no-src-dir` : srcディレクトリを作成しない設定  
`--no-import-alias` : import aliasを設定しない設定
