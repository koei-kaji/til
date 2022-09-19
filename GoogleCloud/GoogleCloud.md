# Google Cloud

- [Google Cloud](#google-cloud)
  - [Best practices for operating containers](#best-practices-for-operating-containers)
    - [Links](#links)
  - [BeyondCorp Enterprise](#beyondcorp-enterprise)
    - [構成要素](#構成要素)
    - [Links](#links-1)
  - [Cloud Armor](#cloud-armor)
    - [セキュリティポリシー](#セキュリティポリシー)
    - [Links](#links-2)
  - [Connect to Google Cloud](#connect-to-google-cloud)
    - [Links](#links-3)
  - [IAP Connector](#iap-connector)
    - [Links](#links-4)
  - [VPC Service Controls](#vpc-service-controls)
    - [Links](#links-5)

---

## Best practices for operating containers

- Use the native logging mecanisms of containers
  - ![Kubernetesでの標準的なログ管理システムを示す図](https://cloud.google.com/static/architecture/images/bp-operating-containers-log-management.svg)
  - ![ログ管理用サイドカーパターン](https://cloud.google.com/static/architecture/images/bp-operating-containers-sidecar.svg)
- Ensure that your containers are stateless and imuutable
  - ![Pod内の構成ファイルとしてマウントされたConfigMapを使用してDeploymentの構成を更新する例](https://cloud.google.com/static/architecture/images/bp-operating-containers-configmap.svg)
- Avoid privileged containers
- Make your application easy to monitor
- Expose the health of your application
- Avoid running as root
- Carefully choose the image version

### Links

- [Google Cloud | Best practices for operating containers](https://cloud.google.com/architecture/best-practices-for-operating-containers)

---

## BeyondCorp Enterprise

エージェントレス・VPNレスで社内ITサービスへのアクセスを実現する、Googleのセキュリティサービス群　　

**ゼロトラストセキュリティ**：ユーザのリクエストのコンテキスト（デバイス状態、アクセス状況等、IDとパスワードだけに頼らない各種背景情報）を判断に使ってアクセス制御を行う方式

### 構成要素

- Identity-Aware Proxy (IAP)
- Identity and Access Management (IAM)
- Access Context Manager
- Endpoint Verification

### Links

- [Ggen Tech Blog | BeyondCorp Enterprise](https://blog.g-gen.co.jp/entry/beyondcorp-enterprise-explained)
- [net one | ゼロトラストセキュリティ](https://www.netone.co.jp/knowledge-center/netone-blog/20200501-1/)

---

## Cloud Armor

- WAF(Web Application Firewall)
  - SQLインジェクション、クロスサイトスクリプティングといったアプリケーションレイヤの攻撃を検知し、防御する仕組み
- **Cloud Load Balancingの背後にあるWebアプリケーションのみ**を保護

### セキュリティポリシー

防御ルールの設定  
セキュリティポリシーを作成して、外部HTTP(S)ロードバランサのバックエンドサービスにアタッチすることで、ルールが効果を発揮する  

### Links

- [Ggen Tech Blog | Cloud Armor](https://blog.g-gen.co.jp/entry/cloud-armor-explained)
- [Google Cloud | Cloud Armor](https://cloud.google.com/armor)
- [OWASP | OWASP Top 10](https://owasp.org/www-project-top-ten/)

---

## Connect to Google Cloud

- **Cloud VPN**
- **Cloud Interconnect**
  - Dedicated Interconnect
  - Partner Interconnect
- Direct Peering
- Carrier Peering

![利用目的とそれに適した接続方法のイメージ図](https://atbex.attokyo.co.jp/files/news2/Blog/20220224_Google_Cloud_Interconnect/riyoumokuteki.png)

### Links

- [ATBex | Cloud Interconnect](https://atbex.attokyo.co.jp/blog/detail/37/)
- [Google Cloud | Direct Peering](https://cloud.google.com/network-connectivity/docs/direct-peering?hl=ja)

---

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