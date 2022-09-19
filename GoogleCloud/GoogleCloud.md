# Google Cloud

## Cloud Armor

- WAF(Web Application Firewall)
  - SQLインジェクション、クロスサイトスクリプティングといったアプリケーションレイヤの攻撃を検知し、防御する仕組み
- **Cloud Load Balancingの背後にあるWebアプリケーションのみ**を保護

### セキュリティポリシー

防御ルールの設定  
セキュリティポリシーを作成して、外部HTTP(S)ロードバランサのバックエンドサービスにアタッチすることで、ルールが効果を発揮する  

### Links

- [Google Cloud | Cloud Armor](https://cloud.google.com/armor)
- [GgenTechBlog | Cloud Armor](https://blog.g-gen.co.jp/entry/cloud-armor-explained)
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

---

### Links

- [ATBex | Cloud Interconnect](https://atbex.attokyo.co.jp/blog/detail/37/)
- [Google Cloud | Direct Peering](https://cloud.google.com/network-connectivity/docs/direct-peering?hl=ja)
