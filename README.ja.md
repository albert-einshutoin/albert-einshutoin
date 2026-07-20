# albert-einshutoin

[English](./README.md) | **日本語**

### 実務で見つけた課題と、将来を見据えた技術仮説をOSSとして形にするバックエンドエンジニアです。

特定の技術レイヤーにこだわらず、解くべき問題を追いかけています。技術を前へ進める可能性があり、その仮説をコードで検証できるなら、まず作って確かめます。

AI支援開発を活用し、探索できる領域を広げています。ただコードを生成するのではなく、その下で動く仕組みまで理解すること。検証の成果をOSSやWebサービス、アプリとして公開し、より多くの人が使い、確かめ、発展させられる形にすることを目指しています。

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

---

## 名前と原点

> "Imagination is more important than knowledge."
>
> — Albert Einstein

`albert-einshutoin` は、最も尊敬するAlbert Einsteinへの小さなオマージュです。自分にとって想像力は出発点であり、エンジニアリングはそれを現実の中で確かめるための手段です。

---

## 開発で大切にしていること

1. 実務や開発で出会った、具体的な問題から始める。
2. その問題を解く場所や、現在の抽象化が本当に適切なのかを問い直す。
3. 技術的な仮説を立て、動くソフトウェアで確かめる。
4. 結果をOSSとして公開し、他の人も検証し、議論し、発展させられるようにする。

現在は、Programmable Edge、Native Performance、安全なローカル・CI基盤、AI Memory Systemsに取り組んでいます。いずれも今の探究テーマであり、自分の活動領域を限定するものではありません。

---

## 主なプロジェクト

### Programmable Edge

- [**cdn-security-framework**](https://github.com/albert-einshutoin/cdn-security-framework) — `リリース済み` `JavaScript`

  実務でWAFの導入、アプリケーション層でのレート制限、Nginxによる制御を経験したことが出発点です。Edge Functionsによる軽量な前処理とWAFの防御を別々のレイヤーとして組み合わせ、Backendへ到達する前に明らかな異常を減らせるか検証しています。

- [**quant-cache**](https://github.com/albert-einshutoin/quant-cache) — `リリース済み` `Rust`

  キャッシュ効率を最大化するために、量子インスパイアド最適化を取り入れたパッケージです。経済性と容量の制約のもとで、オフラインのQUBO・シミュレーテッドアニーリング探索がCDNのキャッシュポリシー選択を改善できるか検証しています。

- [**TenantScript**](https://github.com/albert-einshutoin/TenantScript) — `開発中` `TypeScript`

  Cloudflare Workers系の実行プリミティブを土台に、テナント固有プラグインの権限、承認、バージョン、監査ログを管理するControl Planeを構築しています。Dynamic Workersを使った実環境での検証は現在も進行中です。

### Native Performance

- [**lazy-image**](https://github.com/albert-einshutoin/lazy-image) — `リリース済み` `Rust` `Node.js`

  実務でNode.jsの画像処理に`sharp`を選んだことが出発点です。長年の実績と性能でデファクトになっているなら、異なる強みを持つ選択肢を作れないかと考えました。画像処理は未経験の領域でしたが、AI支援を活用し、メモリ使用量の制御、安全なデフォルト、現在の基準ベンチマークにおけるJPEG出力サイズの削減に取り組んでいます。

- [**i18next-turbo**](https://github.com/albert-einshutoin/i18next-turbo) — `リリース済み` `Rust` `N-API`

  i18n関連のCIをできるだけ速くしたい、という思いから生まれました。RustとSWCでキー抽出を高速化し、N-APIを通じて従来のNode.jsワークフローから利用できるようにしています。

### 安全なローカル・CI基盤

- [**mockport**](https://github.com/albert-einshutoin/mockport) — `MVP` `Go` `Docker`

  AI支援開発で、AIエージェントに`.env`を読ませず、安全に結合テストを実行するにはどうすればよいか、という問題から始まりました。Secretの渡し方を工夫するだけでなく、依存サービスそのものをローカルに再現し、接続先と環境変数の切り替えだけでテストできる設計を目指しています。

- [**roomci**](https://github.com/albert-einshutoin/roomci) — `実験中` `Rust` `MQTT`

  `floci`へのコントリビュートと`mockport`の開発から得た発想を、IoTやSmart Homeの開発へ広げています。ローカルエミュレーションと契約テストによって、現場でしか起きない障害をCI上で再現できるか検証しています。

### AI Memory Systems

- [**qzt**](https://github.com/albert-einshutoin/qzt) — `開発中` `Rust` `zstd`

  `qzt`自体は、部分取得と検証可能な検索を備えたzstd圧縮テキスト証跡コンテナです。将来は、人間とAIの長期的な会話コンテキストを保持・再取得する上位システム、MemoryPagerの保存基盤として活用する構想を検証しています。

---

## 外部OSSへの貢献

- [**floci**](https://github.com/floci-io/floci) — ローカルAWS環境におけるRDSの永続化とランタイム状態の復元

  マージ済み: [#945](https://github.com/floci-io/floci/pull/945)、[#1014](https://github.com/floci-io/floci/pull/1014)、[#1071](https://github.com/floci-io/floci/pull/1071)

---

## アクティビティ

[![albert-einshutoinのGitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=albert-einshutoin&theme=github-compact&hide_border=true&area=true&radius=8)](https://github.com/albert-einshutoin)

<p align="center">
  <img src="./profile-summary-card-output/transparent/1-repos-per-language.svg" alt="公開リポジトリで使用している言語" width="340">
</p>

---

## 連絡先

- [X / @forte_grapher](https://x.com/forte_grapher)
- [Note / albert_forte](https://note.com/albert_forte)
