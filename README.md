# cursor-global-rules

Cursor用の共通開発ルール集です。
Python / HTML / CSS / React / SQL (PostgreSQL) 向けに標準的なコーディングガイドラインとセキュリティルールをまとめています。

---

## 概要

このリポジトリは、**Cursorエディタ**で複数プロジェクトに共通適用できるルールを管理するためのものです。
各言語・技術スタックに合わせたルールファイル（MDC形式）が含まれています。

対象：
- Python
- HTML
- CSS
- JavaScript (React)
- SQL (PostgreSQL)

---

## 使い方

### 1. このリポジトリをクローンまたはダウンロードする

```bash
git clone https://github.com/ma0lab/cursor-global-rules.git
```

または、ZIPダウンロードして展開してください。

---

### 2. プロジェクトの `.cursor/rules/` 配下に手動でコピーする

```bash
cp -r path/to/cursor-global-rules/* your-project/.cursor/rules/
```

※ 必要なルールファイルだけコピーしてもOKです。

---

### 3. Cursorで自動的にルールが適用される

- Cursorは `.cursor/rules/` 以下の `.mdc` ファイルを自動的に読み込みます。
- 特別な設定は不要です。

---

## 運用ルール

- 複雑化しないため、サブモジュールやシンボリックリンク運用は行わず、**必要なときにコピーして使う運用**を推奨します。
- 共通ルールの更新があった場合は、各プロジェクトで手動でコピーし直してください。
- ルール内容にプロジェクト独自のカスタマイズが必要な場合は、コピー後に個別修正してOKです。

---

## 収録ファイル一覧

| ファイル名 | 内容 |
|:---|:---|
| `python.mdc` | Python開発ルール |
| `html.mdc` | HTML開発ルール |
| `css.mdc` | CSS開発ルール |
| `js.mdc` | JavaScript(React)開発ルール |
| `sql.mdc` | SQL(PostgreSQL)開発ルール |

---

## ライセンス

このリポジトリはMITライセンスで提供されています。
[LICENSE](./LICENSE) をご確認ください。

## 参考リポジトリ

- [kinopeee/cursorrules](https://github.com/kinopeee/cursorrules)
- [Shin-sibainu/shincode-tech-stack-rules](https://github.com/Shin-sibainu/shincode-tech-stack-rules)

本リポジトリは上記を参考にし、独自に再構成・編集を行ったものです。

---

## 注意事項

- 本リポジトリのルールはプロジェクトの標準化・品質向上を目的としていますが、適用は任意です。
- 各プロジェクトのポリシーに合わせて適宜調整してください。