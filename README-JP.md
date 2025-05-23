# R2Money-Auto-Bot

Sepolia テストネット上の R2 Money プロトコルとやり取りするための自動ボットです。このボットにより、USDC と R2USD トークン間のスワップ、R2USD のステーキングによる sR2USD トークンの受け取りが可能になります。

## 機能

* USDC から R2USD へのスワップ
* R2USD から USDC へのスワップ
* R2USD を sR2USD にステーキング
* トークン残高の確認
* 複数ウォレットのサポート
* IP ローテーションのためのプロキシ対応

## 必要条件

* Node.js v16 以上
* プライベートキー付きの Ethereum ウォレット
* ガス代用の Sepolia ETH
* Sepolia USDC トークン

## インストール手順

1. リポジトリをクローン:

```bash
git clone https://github.com/taikoyaki/R2-money-BOT.git
cd R2-money-BOT
```

2. 依存関係をインストール:

```bash
npm install
```

3. `.env` ファイルを編集してプライベートキーを追加:

```
PRIVATE_KEY_1=your_private_key_here
PRIVATE_KEY_2=another_private_key_here
# 必要に応じてキーを追加
```

4. （任意）`proxies.txt` ファイルを作成してプロキシを1行ずつ記述:

```
http://username:password@host:port
http://host:port
```

## 使用方法

ボットを実行するには以下を実行:

```bash
node index.js
```

インタラクティブメニューに従って操作:

1. USDC を R2USD にスワップ
2. R2USD を USDC にスワップ
3. R2USD を sR2USD にステーキング
4. 残高を確認
5. 終了

## トークンアドレス（Sepolia）

* USDC: `0xef84994ef411c4981328ffce5fda41cd3803fae4`
* R2USD: `0x20c54c5f742f123abb49a982bfe0af47edb38756`
* sR2USD: `0xbd6b25c4132f09369c354bee0f7be777d7d434fa`

## セキュリティに関する注意

* このボットはプライベートキーを必要とします。プライベートキーは絶対に他人と共有しないでください。
* このボットは Sepolia テストネット専用です。
* 実行前にコードを確認してください。

## 免責事項

このボットは教育目的で提供されています。使用は自己責任でお願いします。作成者は資金の損失に関して一切の責任を負いません。

## ライセンス

MIT ライセンス
