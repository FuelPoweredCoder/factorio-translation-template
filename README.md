# Factorio Translation MOD Template

Factorio MODの日本語翻訳プロジェクト用Copierテンプレート

## 🚀 クイックスタート

```bash
# Copierをインストール
pip install copier

# テンプレートを使用して新しい翻訳MODを作成
copier copy gh:FuelPoweredCoder/factorio-translation-template .
```

## ✨ 特徴

- **標準的なディレクトリ構造** - Factorio MOD開発のベストプラクティスに準拠
- **自動命名** - `ja-translation-{元MOD名}` の規則で統一
- **適切な依存関係** - オプショナル依存でエラーを回避
- **changelog.txt** - Factorio独自形式で自動生成
- **Factorio 2.0対応** - 最新バージョンをデフォルト設定

## 📋 生成されるファイル

```
ja-translation-example-mod/
├── info.json          # MOD情報（自動設定）
├── changelog.txt      # 変更履歴（Factorio独自形式）
└── locale/
    └── ja/
        └── .gitkeep   # 翻訳ファイル用ディレクトリ
```

## 🔧 使用方法

### 1. テンプレートの実行

```bash
copier copy gh:FuelPoweredCoder/factorio-translation-template .
```

### 2. 質問への回答

- **元MOD名**: 翻訳対象のMOD名（例: `logistics-train-network`）
- **作者名**: あなたの名前
- **対応Factorioバージョン**: `1.1` または `2.0`（デフォルト: `2.0`）

### 3. 生成後の作業

サムネイルを追加する場合は、`thumbnail.png`を配置してください。推奨サイズは288×288pxです。

## 📝 生成される設定

### info.json
- **name**: `ja-translation-{元MOD名}`
- **title**: `{元MOD名} 日本語訳`
- **version**: `0.1.0`
- **author**: `あなたの名前`
- **description**: `{元MOD名} の日本語翻訳MODです`
- **dependencies**: `["? {元MOD名}"]` - オプショナル依存
- **factorio_version**: `2.0`（または選択したバージョン）

### changelog.txt
Factorio独自の厳格な形式に準拠：
```
---------------------------------------------------------------------------------------------------
Version: 0.1.0
Date: 2025-06-27
  Translations:
    - 元MODの日本語翻訳を追加
    - アイテム名・説明文の日本語化
    - GUI要素の日本語化
```

## 🛠️ 前提条件

- **Python 3.7+**
- **Copier** - `pip install copier`


## 📄 ライセンス

このテンプレートはMITライセンスです。生成されたMODには影響しません。

---

**Happy translating! 🎮🇯🇵**
