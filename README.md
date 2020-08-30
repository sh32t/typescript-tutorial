# TypeScriptチュートリアル
## プロジェクトの作成
```ps1
npm init -y
```
## TypeScriptのインストール
```ps1
npm install typescript
```
## tsconfig.jsonの作成
#### ※npx ・・・ インストールしていないパッケージを一度だけ実行
```ps1
npx tsc --init
```
## TSファイルの作成
```ts
const text:string = 'Hello TypeScript';

console.log(text);
```
## TSファイルのコンパイル
```ps1
npx tsc sample.ts
```
#### 下記のような`sample.js`が作成される。
```js
var text = 'Hello TypeScript';
console.log(text);
```
## TSファイルの即時実行
```ps1
npm install ts-node
./node_modules/.bin/ts-node sample.ts
```
## npm startでの実行
#### `package.json`の`"script"`を下記のように書き換える。
```json
  "scripts": {
    "start": "ts-node sample.ts"
  },
```
#### ※VScodeでNode.js Debug Terminalから実行すればブレークポイントを貼って実行することも可能
```ps1
npm start
```


### 参考
#### [TypeScript チュートリアル](https://qiita.com/EBIHARA_kenji/items/31b7c1c62426bdabd263)
#### [npm 5.2.0の新機能！ 「npx」でローカルパッケージを手軽に実行しよう](https://qiita.com/tonkotsuboy_com/items/8227f5993769c3df533d)
#### [ts-node で TypeScript + node をサクッと実行する](https://qiita.com/mangano-ito/items/75e65071c9c482ddc335)
