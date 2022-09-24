# Google Cloud Managed Services

- [Google Cloud Managed Services](#google-cloud-managed-services)
  - [Binary Authorization](#binary-authorization)
    - [Links](#links)
  - [Cloud Armor](#cloud-armor)
    - [Security Policy](#security-policy)
    - [Links](#links-1)
  - [Cloud BigQuery](#cloud-bigquery)
    - [Materialized view](#materialized-view)
    - [Links](#links-2)
  - [Cloud Bigtable](#cloud-bigtable)
    - [Links](#links-3)
  - [Cloud Data Loss Prevention](#cloud-data-loss-prevention)
    - [Links](#links-4)
  - [Cloud Dataprep by Trifacta](#cloud-dataprep-by-trifacta)
    - [Links](#links-5)
  - [Cloud Filestore](#cloud-filestore)
    - [Links](#links-6)
  - [Cloud Audit Logs](#cloud-audit-logs)
    - [Links](#links-7)
  - [Compute Engine](#compute-engine)
    - [Viewing and applying idle vm recommendations](#viewing-and-applying-idle-vm-recommendations)
    - [Links](#links-8)
  - [IAP Connector](#iap-connector)
    - [Links](#links-9)
  - [VPC Service Controls](#vpc-service-controls)
    - [Links](#links-10)

---

## Binary Authorization

- \-

### Links

- [Google Cloud](https://cloud.google.com/binary-authorization?hl=ja)
- [TOPGATE | Google Cloud security application](https://www.topgate.co.jp/google-cloud-security-application#binary-authorization)

## Cloud Armor

- WAF(Web Application Firewall)
  - SQLインジェクション、クロスサイトスクリプティングといったアプリケーションレイヤの攻撃を検知し、防御する仕組み
- **Cloud Load Balancingの背後にあるWebアプリケーションのみ**を保護

### Security Policy

防御ルールの設定  
セキュリティポリシーを作成して、外部HTTP(S)ロードバランサのバックエンドサービスにアタッチすることで、ルールが効果を発揮する  

### Links

- [Ggen Tech Blog | Cloud Armor](https://blog.g-gen.co.jp/entry/cloud-armor-explained)
- [Google Cloud | Cloud Armor](https://cloud.google.com/armor)
- [OWASP | OWASP Top 10](https://owasp.org/www-project-top-ten/)

---

## Cloud BigQuery

### Materialized view

事前に計算されたビュー、結果を定期的にキャッシュに保存する
メンテナンス不要、最新のデータ、スマートな調整

### Links

- [Google Cloud | Materialized view](https://cloud.google.com/bigquery/docs/materialized-views-intro)

---

## Cloud Bigtable

- \-

### Links

- [Google Cloud | Bigtable overview](https://cloud.google.com/bigtable/docs/overview)
- [Google Cloud | Bigtable schema design](https://cloud.google.com/bigtable/docs/schema-design)
- [Google Cloud | Key Visualizer](https://cloud.google.com/bigtable/docs/keyvis-overview)

---

## Cloud Data Loss Prevention

- \-

### Links

- [DevelopersIO | Cloud DLP](https://dev.classmethod.jp/articles/cloud-dlp-inspect-bigquery/)
- [Google Cloud | Cloud Data Loss Prevention](https://cloud.google.com/dlp?hl=ja)

---

## Cloud Dataprep by Trifacta

- データクレンジングサービス
- フルマネージドかつサーバーレス

### Links

- [Google Cloud | Cloud Dataprep by Trifacta](https://cloud.google.com/dataprep?hl=ja)
- [TOPGATE | Cloud Dataprep](https://www.topgate.co.jp/cloud-dataprep)

---

## Cloud Filestore

- \-

### Links

- [Google Cloud | Filestore](https://cloud.google.com/filestore)
- [TOPGATE | GCP Storage](https://www.topgate.co.jp/google-cloud-day-storage#filestore)

---

## Cloud Audit Logs

管理アクティビティとGoogle Cloudリソース内のアクセスを記録する監査ログを書き込む
記録されたログはCloud Loggingに保存される

| #   | 名称                       | 説明                                                                                                               | 料金 | default                      |
| --- | -------------------------- | ------------------------------------------------------------------------------------------------------------------ | ---- | ---------------------------- |
| 1   | 管理アクティビティ監査ログ | リソースに対する更新系のAPIコールを記録                                                                            | 無料 | 有効（無効化できない）       |
| 2   | データアクセス監査ログ     | リソースに対する参照系のAPIコール、データの参照・更新系のAPIコールを記録。ログ容量が大きくなる可能性があるため注意 | 有料 | 無効（BigQueryのみ有効）     |
| 3   | システムイベント監査ログ   | Google Cloudサービスによって行われたリソース構成変更を記録                                                         | 無料 | 有効（無効化できない）       |
| 4   | ポリシー拒否監査ログ       | VPC Service Controls機能で拒否されたAPIコールを記録                                                                | 有料 | 有効（除外フィルタ設定可能） |

### Links

- [Google Cloud | Cloud Audit Logs](https://cloud.google.com/logging/docs/audit)
- [Ggen Tech Blog | Cloud Audit Logs](https://blog.g-gen.co.jp/entry/cloud-audit-logs-explained)

---

## Compute Engine

### Viewing and applying idle vm recommendations

使用されていないVMインスタンスを識別できるように、アイドル状態のVMに対して"推奨"が表示される
過去14日感の使用状況を指標に基づいてVMインスタンスに関する"推奨"を生成する

### Links

- [Google Cloud | Viewing and applying idle vm recommendations](https://cloud.google.com/compute/docs/instances/viewing-and-applying-idle-vm-recommendations)

## IAP Connector

GCP外のシステムをCloud IAPのバックエンドとして利用する仕組み  
実態はGKEクラスタ上で実行されるAmbassador API Gatewayコンテナ  

![IAP Connectorの構成図](https://cdn-ssl-devio-img.classmethod.jp/wp-content/uploads/2020/04/beyondcorpra01_1.png)

### Links

- [DevelopersIO | Cloud IAP Connector](https://dev.classmethod.jp/articles/beyondcorp-remote-access-getting-started1/)
- [Google Cloud | マネージドEnvoyを使用したIAPコネクタのデプロイ](https://cloud.google.com/architecture/deploying-iap-connector-using-managed-envoy?hl=ja)

---

## VPC Service Controls

Google Cloud サービスに対するAPIコールの接続元を制限する

### Links

- [Ggen Tech Blog | VPC Service Controls](https://blog.g-gen.co.jp/entry/vpc-service-controls-explained)
- [Google Cloud | VPC Service Controls](https://cloud.google.com/vpc-service-controls)