# Zenn 公開手順

記事は完成済み（658行）。3つの方法から選べる。

---

## 🥇 方法A: GitHub連携（最もZennらしい方法）

Zennアカウント（Googleログイン）にGitHubリポジトリを連携させると、pushするだけで自動公開できる。

### 手順
1. https://zenn.dev/settings にアクセス
2. 「GitHub連携」→ `aether-yuki/thinking-vs-trial` リポジトリを連携
3. Zennが自動的に `zenn-article.md` を検出する
4. 公開するときはファイルの1行を変えてpush：
```bash
cd /Users/nyuki/.openclaw/workspace/projects/thinking-vs-trial
# published: false → true に変更
sed -i '' 's/published: false/published: true/' zenn-article.md
git add zenn-article.md
git commit -m "publish: 思考 vs 試行の最適バランス"
git push
```

**GitHubアカウント（nyukicorn）をZennに後から連携できる：**  
Zennの設定 → 「連携サービス」→「GitHubと連携」

---

## 🥈 方法B: Webエディタ（今すぐできる）

1. https://zenn.dev/articles/new にアクセス
2. 「Markdownで書く」を選択
3. `zenn-article.md` の中身をすべてコピペ（frontmatterごと）
4. プレビューで確認 → 「公開する」ボタン

**`zenn-article.md` の場所:**
```
/Users/nyuki/.openclaw/workspace/projects/thinking-vs-trial/zenn-article.md
```

または GitHub: https://github.com/aether-yuki/thinking-vs-trial/blob/main/zenn-article.md

---

## 📋 記事の現状

| 項目 | 内容 |
|------|------|
| タイトル | 思考（Thinking）vs 試行（Trial）の最適バランス — AIエージェント時代のコンパス |
| 絵文字 | 🧭 |
| タグ | AI, 生産性, 意思決定, エージェント, 行動科学 |
| 文字数 | 約30,000文字（658行）|
| 状態 | `published: false` → **1行変えるだけで公開** |
| GitHub | https://github.com/aether-yuki/thinking-vs-trial |

---

**nyukicorn はこのリポジトリのコラボレーター（admin）として招待済み。**  
GitHubでacceptすれば直接pushできる。
