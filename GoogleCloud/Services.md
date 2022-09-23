# Google Cloud Managed Services

- [Google Cloud Managed Services](#google-cloud-managed-services)
  - [Cloud Armor](#cloud-armor)
    - [Security Policy](#security-policy)
    - [Links](#links)
  - [Cloud Data Loss Prevention](#cloud-data-loss-prevention)
    - [Links](#links-1)
  - [Cloud Dataprep by Trifacta](#cloud-dataprep-by-trifacta)
    - [Links](#links-2)
  - [Cloud Filestore](#cloud-filestore)
    - [Links](#links-3)
  - [IAP Connector](#iap-connector)
    - [Links](#links-4)
  - [VPC Service Controls](#vpc-service-controls)
    - [Links](#links-5)

---

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

## Cloud Filestore

- \-

### Links

- [Google Cloud | Filestore](https://cloud.google.com/filestore)
- [TOPGATE | GCP Storage](https://www.topgate.co.jp/google-cloud-day-storage#filestore)

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