# Qiita記事管理リポジトリ

このリポジトリはQiita CLIを使用して記事を管理しています。

## 記事一覧

- [【RPG風】venv魔王を倒せ!伝説の剣「uv」でPython開発を救う冒険](public/uv-rpg-adventure.md)

## セットアップ
```bash
# Qiita CLIのインストール
npm install -g @qiita/qiita-cli

# ログイン
npx qiita login

# プレビュー
npx qiita preview

# 記事を公開
npx qiita publish <記事ファイル名>
```

## 記事の公開方法

### 下書きとして保存
```yaml
private: true
```

### 公開する
```yaml
private: false
```

GitHubにプッシュすると、GitHub Actionsが自動的にQiitaに反映します。

## ディレクトリ構成
```
.
├── .github/workflows/  # GitHub Actions設定
├── public/             # 公開記事
├── .gitignore
├── qiita.config.json
└── README.md
```

## 参考リンク

- [Qiita CLI公式ドキュメント](https://github.com/increments/qiita-cli)
- [Peaky AI LAB](https://peaky.co.jp/)
