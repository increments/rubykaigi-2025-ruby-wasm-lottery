# Ruby Wasmくじ引き

[![GitHub](https://img.shields.io/badge/GitHub-increments%2Frubykaigi--2025--ruby--wasm--lottery-green?style=flat-square&logo=github)](https://github.com/increments/rubykaigi-2025-ruby-wasm-lottery)

RubyKaigi 2025 Qiitaブース展示用のRuby WebAssemblyデモアプリケーションです。ruby-wasm-vdomを使用したインタラクティブなくじ引きゲームを実装しています。

[こちらからデモを試せます](https://increments.github.io/rubykaigi-2025-ruby-wasm-lottery/)

![くじ引きデモ画像](https://placehold.jp/55c500/ffffff/400x200.png?text=Ruby%20Wasm%E3%81%8F%E3%81%98%E5%BC%95%E3%81%8D)

## 特徴

- **Ruby Wasm**: ブラウザ上でRubyコードを実行
- **Virtual DOM**: 効率的なDOM更新による高速なUIレンダリング
- **インタラクティブ抽選**: 確率ベースのくじ引きロジック
- **アニメーション効果**: 抽選中の動的な視覚効果と紙吹雪

## 賞品

抽選では以下の賞品が当たります：

- **Qiitan ストレスボール** (大当たり！)
- **お菓子詰め合わせ** (当たり！)

## 技術スタック

- [Ruby Wasm](https://github.com/ruby/ruby.wasm): ブラウザで実行可能なRuby
- [ruby-wasm-vdom](https://github.com/getty104/ruby-wasm-vdom): Ruby WasmとVirtual DOMの統合
- HTML5 / CSS3: モダンなUI実装
- JavaScript: ブラウザAPIとのインターフェース

## 開発プロセス

このプロジェクトは、AIアシスタント「Cline」を活用して効率的に開発されました。Clineを使用することで、以下のメリットがありました：

- **メモリバンク管理**: プロジェクトの要件や技術的な決定事項をメモリバンクに保存し、一貫した開発を実現
- **効率的なコーディング**: Ruby Wasmの知識を活用した迅速な実装
- **構造化された開発**: システムパターンとアーキテクチャの設計を支援
- **自動ドキュメント化**: コードとともにドキュメントを同時に生成

Clineはプロジェクトの計画段階から実装まで一貫してサポートし、ruby-wasm-vdomの特性を活かしたアプリケーション開発を可能にしました。

## 動作環境

- モダンなWebブラウザ (Chrome, Firefox, Safari, Edgeの最新版)
- JavaScript有効設定

## ローカルでの実行方法

1. このリポジトリをクローン:
   ```bash
   git clone https://github.com/increments/rubykaigi-2025-ruby-wasm-lottery.git
   cd rubykaigi-2025-ruby-wasm-lottery
   ```

2. 以下のいずれかの方法で実行:
   ```bash
   # 直接ファイルを開く
   open docs/index.html

   # または簡易Rubyサーバーを起動
   ruby -run -e httpd . -p 8000
   # その後ブラウザで http://localhost:8000/docs/ にアクセス
   ```

## 開発について

このプロジェクトは、Qiita株式会社が開発した[ruby-wasm-vdom](https://github.com/getty104/ruby-wasm-vdom)の可能性を示すデモアプリケーションです。Ruby WebAssemblyを使用したウェブアプリケーション開発の柔軟性と可能性を体験していただけます。

## 開発者

Qiita株式会社 - [https://qiita.com](https://qiita.com)

RubyKaigiについての詳細は[公式サイト](https://rubykaigi.org)をご覧ください。
