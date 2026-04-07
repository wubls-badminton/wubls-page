# WUBLS 新歓ランディングページ

早稲田大学バドミントン同好会 WUBLS の新歓用ランディングページ。

## 公開URL

https://wubls-badminton.github.io/wubls-page/

## ホスティング

GitHub Pages（wubls-badminton org・masterブランチ）。
- リポジトリ: https://github.com/wubls-badminton/wubls-page
- 旧URL: http://160.251.232.198.nip.io/（VPS・2026-04-07移行）

## 構成

- `index.html` — 単一HTMLファイル（全機能）
- `img/g*.jpg` — 切り出し画像
- `qrcode.png` — えんじ色QRコード（https://wubls-badminton.github.io/wubls-page/ 対応）

## 機能

- 新歓練習8日程 → LINE申込リンク（line.me/ti/g/7AxaRDjeMz）
- SNSリンク: LINE / X(@WUBLS) / Instagram(@WUBLS, @WUBLS_shinkandayo)
- チラシPDF閲覧リンク（Google Drive）
- スクロールフェードインアニメーション

## デプロイ方法

```bash
# masterブランチにpushするだけで自動デプロイ
git push origin master
```

## カラー

- えんじ色: `#8B2332`
- ゴールド: `#C6993E`
