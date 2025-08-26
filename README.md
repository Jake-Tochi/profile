# 株式会社ウェルネシー 会社概要サイト

日本と海外の企業をつなぐ架け橋として、相性の良いパートナーとの出会いを創出し、低リスクで新市場への進出をサポートする会社概要サイトです。

## サイト概要

- **URL**: https://profile.jpn-travel.com/
- **技術**: 静的HTML + CSS + 最小限のJavaScript（フレームワーク不使用）
- **デザイン**: レスポンシブ対応、アクセシビリティ準拠
- **ホスティング**: GitHub Pages

## ファイル構成

```
/
├─ index.html              # メインページ
├─ assets/
│   ├─ styles.css          # スタイルシート
│   ├─ logo.svg            # 会社ロゴ
│   └─ favicon.svg         # ファビコン
├─ CNAME                   # カスタムドメイン設定
└─ README.md               # このファイル
```

## GitHub Pages 公開手順

### 1. リポジトリ作成

1. GitHubにログインし、新しいリポジトリを作成
2. リポジトリ名は任意（例：`wellnethy-profile`）
3. Publicに設定

### 2. ファイルアップロード

1. このリポジトリの全ファイルをGitHubリポジトリにアップロード
2. ファイル構成を維持すること

### 3. GitHub Pages設定

1. リポジトリの「Settings」タブを開く
2. 左メニューから「Pages」を選択
3. 「Source」で「Deploy from a branch」を選択
4. 「Branch」で「main」（または「master」）を選択
5. フォルダは「/ (root)」を選択
6. 「Save」をクリック

### 4. カスタムドメイン設定（重要）

1. GitHub PagesのPages設定画面で「Custom domain」に `profile.jpn-travel.com` を入力
2. 「Save」をクリック
3. **注意**: CNAMEファイルが既に含まれているため、このファイルが削除されないよう注意

### 5. DNS設定

ドメイン管理画面で以下のDNS設定を行ってください：

**Aレコードの場合（推奨）:**
```
Type: A
Name: profile
Value: 185.199.108.153
Value: 185.199.109.153
Value: 185.199.110.153
Value: 185.199.111.153
```

**CNAMEレコードの場合:**
```
Type: CNAME
Name: profile
Value: [GitHubユーザー名].github.io
```

### 6. HTTPS設定

1. DNS設定後、数時間待機
2. GitHub PagesのPages設定で「Enforce HTTPS」にチェックを入れる

## 技術仕様

### アクセシビリティ

- WCAG 2.1 AA レベル準拠
- コントラスト比 4.5:1 以上
- キーボードナビゲーション対応
- スクリーンリーダー対応
- `prefers-reduced-motion` 対応

### パフォーマンス

- 軽量な静的ファイル
- SVG画像使用（ビットマップ画像なし）
- フォント最適化
- 最小限のJavaScript

### SEO

- 構造化データ（JSON-LD）実装
- OpenGraph/Twitter Card対応
- セマンティックHTML
- 適切なメタタグ設定

### レスポンシブ対応

- モバイルファースト設計
- ブレイクポイント: 768px, 480px
- 最大コンテナ幅: 920px

## ライセンス

このサイトの著作権は株式会社ウェルネシーに帰属します。

## 免責事項

本サイトの掲載情報は予告なく変更される場合があります。

## お問い合わせ

- **Email**: info-wellnethy@jpn-travel.com
- **Tel**: 03-5967-1221
- **住所**: 東京都板橋区高島平1丁目24番6号

---

© 2024 Wellnethy Co., Ltd.