# 業務用エアコン専門店比較ナビ

人気の業務用エアコン専門店をランキング形式で徹底的に比較するサイト。

## 技術スタック

- **Next.js 14** - Reactフレームワーク（App Router）
- **TypeScript** - 型安全な開発
- **Tailwind CSS** - ユーティリティファーストなCSSフレームワーク
- **Recharts** - チャートライブラリ（価格比較、保証期間）
- **Leaflet / react-leaflet** - 施工エリアマップ
- **Lucide React** - アイコンライブラリ

## 機能

- ランキングTOP3の詳細表示
- 絞り込み検索（エリア、対応業種、支払い方法、保証期間）
- 価格比較チャート
- 保証期間比較チャート
- 施工エリアマップ
- 施工事例ギャラリー
- Before/Afterスライダー
- コラム記事

## ローカル開発

```bash
# 依存関係をインストール
npm install

# 開発サーバーを起動
npm run dev
```

http://localhost:3000 にアクセスしてください。

## ビルド

```bash
# 静的サイトとしてビルド
npm run build
```

`out/` ディレクトリに静的ファイルが生成されます。

## デプロイ

Cloudflare Pages に静的サイトとしてデプロイ可能です。

```bash
# Cloudflare Pages にデプロイ
npx wrangler pages deploy out --project-name=gyomuyou-aircon-ranking-navi
```

## プロジェクト構成

```
├── app/                    # Next.js App Router
│   ├── layout.tsx         # ルートレイアウト
│   ├── page.tsx           # トップページ
│   └── globals.css        # グローバルスタイル
├── components/            # Reactコンポーネント
│   ├── charts/           # チャートコンポーネント
│   ├── map/              # 地図コンポーネント
│   ├── images/           # 画像コンポーネント
│   ├── ranking/          # ランキングコンポーネント
│   ├── search/           # 検索コンポーネント
│   └── ui/               # UIコンポーネント
├── data/                 # データファイル
│   ├── stores.ts         # 店舗データ
│   ├── types.ts          # 型定義
│   └── column-articles.ts # コラム記事
└── lib/                  # ユーティリティ関数
```

## ライセンス

MIT
