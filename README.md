# WUBLS 新歓ランディングページ

早稲田大学バドミントン同好会 WUBLS の新歓用ランディングページ。

## 公開URL

http://160.251.232.198.nip.io/

## ホスティング

AsinstarのVPS（160.251.232.198）のnginxバーチャルホスト。
Netlifyはアカウントクレジット超過のため2026-04-06から使用不可。

### nginx設定（VPS上）
- ファイル: `/etc/nginx/conf.d/wubls.conf`
- ポート: 80（バーチャルホスト）
- server_name: `160.251.232.198.nip.io`
- root: `/var/www/wubls`

他ツール（asinstar・sedori-keihi）とはserver_nameで完全分離。

## 構成

- `index.html` — 単一HTMLファイル（全機能）
- `img/g*.jpg` — 切り出し画像
- `qrcode.png` — えんじ色QRコード（http://160.251.232.198.nip.io/ 対応）

## 機能

- 新歓練習8日程 → LINE申込リンク（line.me/ti/g/7AxaRDjeMz）
- SNSリンク: LINE / X(@WUBLS) / Instagram(@WUBLS, @WUBLS_shinkandayo)
- チラシPDF閲覧リンク（Google Drive）
- スクロールフェードインアニメーション

## デプロイ方法

```python
# paramiko SSHスクリプトで自動デプロイ
# C:\tmp\fix_wubls_nip.py を参照
python C:/tmp/fix_wubls_nip.py
```

## カラー

- えんじ色: `#8B2332`
- ゴールド: `#C6993E`
