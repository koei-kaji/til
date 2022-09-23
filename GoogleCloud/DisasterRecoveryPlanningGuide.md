# Disaster recovery planning guide

- [Disaster recovery planning guide](#disaster-recovery-planning-guide)
  - [DR計画の基本](#dr計画の基本)
  - [DRのパターン](#drのパターン)
  - [Linsk](#linsk)

## DR計画の基本

- Recovery Time Objective (RTO)
  - アプリケーションがオフラインである状態が許容される最大時間
  - 通常、SLAの一部として定義される
- Recovery Point Objective (RPO)
  - 重大なインシデントが原因でアプリケーションからデータが失われている状態が許容される最大時間
  - 失われたデータの量や質ではなく時間の長さのみを表す

DR計画では、次の要件を満たす必要がある

- 容量
- セキュリティ
- ネットワークインフラストラクチャ
- サポート
- 帯域幅
- 設備

## DRのパターン

- コールド
- ウォーム
- ホット

---

## Linsk

- [Google Cloud | 障害復旧ガイド](https://cloud.google.com/architecture/dr-scenarios-planning-guide?hl=ja#implementing_control_measures)