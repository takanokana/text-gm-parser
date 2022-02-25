# text-gm-parser README

自作ゲームの会話テキストを管理するための独自拡張子`gm.txt`ファイルに
シンタックスをつけるためのVSCode拡張機能です。

## パッケージのインストール方法

```
code --install-extension text-gm-parser-0.0.1.vsix
```

＊codeコマンドが効かない場合はコマンドぱレッドで`Shell Command: Install 'code' command in PAT`を選択して
パスを通してください。

## ビルド
```
npx vsce package
```

## シンタックスルール

### コメント
`#` で始まる行はコメント。

### コマンド
`@`で始まる行はコマンド。

### コメントコマンド
`# @`で始まる行はコメントコマンド。（通常は解析されないが、コマンドによって再度解析される可能性のあるもの）
