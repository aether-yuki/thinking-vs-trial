# Zenn 公開手順

記事は完成済み（658行）。あとはこれだけ：

## 方法A: Zenn GitHub連携（推奨）

Zennのアカウントにこのリポジトリを連携させてるなら：

```bash
# 1. published: false → true に変更
sed -i '' 's/published: false/published: true/' zenn-article.md

# 2. commit & push
git add zenn-article.md
git commit -m "publish: 思考 vs 試行の最適バランス"
git push
```

## 方法B: Zenn CLI

```bash
# Zenn CLI が入ってない場合
npm install -g zenn-cli

# 記事ファイルの場所に移動してプレビュー
npx zenn preview

# 公開は zenn-article.md の published: false → true に変えてpush
```

## 方法C: Web エディタ

1. https://zenn.dev/dashboard/articles にアクセス
2. 「記事を書く」→ テキストエリアに `zenn-article.md` の内容を貼り付け
3. 公開ボタンを押す

---

**現在の状態:** `published: false` — 1行変えるだけで公開できる状態
