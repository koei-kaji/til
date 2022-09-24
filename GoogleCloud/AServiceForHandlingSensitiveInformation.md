# A service for handling sensitive information

クレジットカードおよびデビットカードのアクセス制御されたトークン化サービスを設定する方法

トークン化：クレジットカードデータなどの機密情報を安全なプレースホルダの値（トークン）に置き換えるプロセス

- [A service for handling sensitive information](#a-service-for-handling-sensitive-information)
  - [機密情報を扱うサービス](#機密情報を扱うサービス)
  - [Links](#links)

## 機密情報を扱うサービス

トークン化サンプルアプリのアーキテクチャ

- Cloud Functions：アプリメインロジック
- Cloud KMS：暗号鍵のホスト、定期的な鍵のローテーション、保管されたアカウントデータの暗号化・復号化
- Firestore：トークン化されたデータを保存

![architecture](https://cloud.google.com/static/architecture/images/tokenizing-sensitive-cardholder-data-architecture.svg?hl=ja)

---

## Links

- [Google Cloud | A service for handling sensitive information](https://cloud.google.com/architecture/tokenizing-sensitive-cardholder-data-for-pci-dss?hl=ja#a_service_for_handling_sensitive_information)
