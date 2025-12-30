# llm-prompt-deck

A deck of reusable prompts for chatting with LLMs.

> “プロンプトを考える” を減らして、会話と作業に集中するための **プロンプトカードデッキ** です。  
> コピペで使える *cheat sheet / カンペ* みたいなノリで増やしていきます。

---

## What’s inside

- 目的別の「プロンプトカード」(再利用できる型)
- 役割・制約・出力フォーマットを毎回ぶらさずに指定できる
- 仕事/創作/調査/実装/レビューなど、LLMチャットで頻出のやつ

---

## Quick start

1. `prompts/` から使いたいカードを選ぶ
2. `foo` `bar` などのプレースホルダを埋める
3. そのまま LLM に投げる（ChatGPT / Claude / Gemini など）

---

## Prompt card format

このリポジトリでは、カードを txt で管理します。

推奨フォーマット:

- ファイル名: `prompts/<slug>.txt`
- 本文が “そのまま貼るプロンプト”

例:

````md
全角かっこ、全角コロンは決して使用しないでください。半角かっこを使用する際は "[space](" ")[space]" の形でスペースを挿入してください。半角コロンを使用する際は ":[space]" の形でスペースを挿入してください。 

悪い例1: 代替現実ゲーム（ARG）は、
悪い例2: 代替現実ゲーム ( ARG ) は、
良い例: 代替現実ゲーム (ARG) は、

悪い例1: ARG：代替現実ゲーム
悪い例2: ARG : 代替現実ゲーム
良い例: ARG: 代替現実ゲーム
````

---

## Tips

* **最初に “出力フォーマット” を固定**するとブレが減ります
  例: 箇条書き / 表 / JSON / diff など
* **禁止事項を明記**すると事故りにくいです
  例: 個人情報・秘密情報・推測禁止・確信度の提示 など
* 迷ったら、カードの末尾に **「追加で必要な情報があれば質問して」** を付ける

---

## Safety / etiquette

* このリポジトリのカードは “汎用テンプレ” です。 **機密情報・個人情報・契約情報** は貼らないでください。

---

## Contributing

PR / Issue welcome!

* 新しいカード追加: `prompts/` に txt を追加
* 既存カード改善: 説明、プレースホルダ、出力形式、注意点を強化
* 命名: ケバブケース + .txt 推奨（例: `code-review-security.txt`）

---

## License

MIT License. See `LICENSE`.

© 2025 AllegroMoltoV. Released under the MIT License.