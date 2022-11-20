# eslint-rules

ESLint の設定共通化ライブラリです。個人用に作成しました。設定は[こちら](https://github.com/hosonokotaro/eslint-rules/blob/master/index.json)

## Install

eslint とそのプラグインが install されている環境が前提です。

```
npm i -D @hosonokotaro/eslint-rules
```

## .eslintrc.js

まず、一括で設定を入れる場合は下記の通り

```
// eslint-disable-next-line @typescript-eslint/no-var-requires
const rules = require('@hosonokotaro/eslint-rules')

module.exports = {
  ...rules,
}
```

もし、個別の設定をする場合は、各プロパティを個別で読み込んで上書きするなどの対応が必要（当面の間）
