# albert-einshutoin

[English](./README.md) | **日本語**

エッジセキュリティ、CDNポリシー、CIエミュレーション、テスト基盤のOSS。  
Rust / TypeScript / Go。ポリシー as code、Docker-first、spec駆動。

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=albert-einshutoin&label=Views&color=0e75b6&style=flat" />
  <img src="https://img.shields.io/github/followers/albert-einshutoin?label=Followers&logo=github&style=flat" />
</p>

---

## Respect

Respect Albert Einstein.

> "Imagination is more important than knowledge."
>
> -- Albert Einstein

`albert-einshutoin` は、その精神への小さなリスペクトとして付けています。

---

## やっていること

- エッジ / CDN: セキュリティヘッダ、キャッシュポリシー、コスト最適化
- CI / QA: サービスエミュレータ、契約テスト、シークレットなし結合テスト
- メディア / i18n: 画像パイプライン、ローカライズツール
- アプリが import したり shell したりする低レイヤの lib / CLI
- エンドユーザー向けサービス

---

## リポジトリ

| プロジェクト | レイヤー | 状態 | 概要 |
|--------|-------|--------|--------------|
| [**cdn-security-framework**](https://github.com/albert-einshutoin/cdn-security-framework) | エッジ / セキュリティ | リリース済み | CloudFront / Cloudflare 向けポリシー駆動CDNセキュリティ |
| [**quant-cache**](https://github.com/albert-einshutoin/quant-cache) | CDN / 最適化 | 開発中 | 経済目的関数によるキャッシュポリシー評価 |
| [**lazy-image**](https://github.com/albert-einshutoin/lazy-image) | メディア / 性能 | リリース済み | CDN配信ワークロード向け Rust 画像最適化 |
| [**i18next-turbo**](https://github.com/albert-einshutoin/i18next-turbo) | DX / i18n | リリース済み | Rust + SWC による i18next キー抽出・ローカライズ |
| [**mockport**](https://github.com/albert-einshutoin/mockport) | テスト | MVP | シークレット不要の Docker-first サービスエミュレータ |
| [**roomci**](https://github.com/albert-einshutoin/roomci) | IoT / QA | PoC | ローカル / CI 向け MQTT / edge-device 契約エミュレータ |
| [**qzt**](https://github.com/albert-einshutoin/qzt) | ストレージ / 証跡 | 開発中 | 証跡アドレス可能な AI メモリのための、シーク可能で検証可能な zstd テキストコンテナ |

---

## コントリビュート

| プロジェクト | レイヤー | 内容 |
|--------|-------|------|
| [**floci**](https://github.com/floci-io/floci) | ローカル AWS | RDS の永続化と runtime 復元 |

---

## スタック

![](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![](https://img.shields.io/badge/OpenAPI-Spec%20Driven-6BA539?style=for-the-badge&logo=openapiinitiative&logoColor=white)
![](https://img.shields.io/badge/Cloudflare-Workers-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![](https://img.shields.io/badge/Amazon%20CloudFront-CDN-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![](https://img.shields.io/badge/GitHub%20Actions-CI-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

デプロイ先: CloudFront, Cloudflare Workers, GitHub Actions, ローカル Docker。

---

## アクティビティ

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=albert-einshutoin&theme=onedark" width="100%" />

<div align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=albert-einshutoin&theme=onedark" width="49%" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=albert-einshutoin&theme=onedark" width="49%" />
</div>

---

## SNS

- X: https://x.com/forte_grapher
- Note: https://note.com/albert_forte
