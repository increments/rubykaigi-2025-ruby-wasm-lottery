# 技術コンテキスト

## 使用技術
- Ruby Wasm: RubyコードをWebAssemblyにコンパイルし、ブラウザで実行
- Virtual DOM: 効率的なDOM更新を可能にするライブラリ
- ES6 JavaScript: モダンなJavaScript機能を活用
- CSS3 Animations: アニメーション効果の実装に使用

## Ruby-JavaScript相互運用の注意点
1. **JS値の型変換**
   - JS関数から返される値は`JS::Object`型
   - Ruby演算子で使用する前に`to_f`や`to_i`などでプリミティブ型に変換する必要がある
   - 例: `window[:Math].random` → `window[:Math].random.to_f`

2. **アクション連鎖の実装**
   - アクション内から別のアクションを呼び出す場合、アクションオブジェクト自体を引数として渡す必要がある
   - 形式: `actions[:action_name].call(state, { additional_data: data, actions: actions })`
