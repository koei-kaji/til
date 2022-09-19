# Google Cloud

## Cloud Armor

- WAF(Web Application Firewall)
  - SQLインジェクション、クロスサイトスクリプティングといったアプリケーションレイヤの攻撃を検知し、防御する仕組み
- **Cloud Load Balancingの背後にあるWebアプリケーションのみ**を保護

### セキュリティポリシー

防御ルールの設定  
セキュリティポリシーを作成して、外部HTTP(S)ロードバランサのバックエンドサービスにアタッチすることで、ルールが効果を発揮する  

### Link

- [Google Cloud | Cloud Armor][Google_CloudArmor]
- [GgenTechBlog | Cloud Armor][GgenTechBlog_CloudArmor]
- [OWASP | OWASP Top 10][OWASP_OWASPTopTen]

[Google_CloudArmor]: https://cloud.google.com/armor
[GgenTechBlog_CloudArmor]: https://blog.g-gen.co.jp/entry/cloud-armor-explained
[OWASP_OWASPTopTen]: https://owasp.org/www-project-top-ten/
