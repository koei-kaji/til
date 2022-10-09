# Migrating VMs with Migrate to Virtual Machines

## Google Cloudへの移行を設計する

![workflow](https://cloud.google.com/static/architecture/images/migration-to-gcp-getting-started-migration-path.svg)

1. Assess
   1. 下記について評価する
      1. 移行元の環境
      2. Google Cloudに移行するワークロード
      3. どのVMが各ワークロードをサポートするか
2. Plan
   1. Migrate to VMsの基本インフラを作成する
      1. リソース階層のプロビジョニング、ネットワークアクセスの設定など
3. Deploy
   1. 移行元の環境のVMをCompute Engineに移行する
4. Optimize
   1. クラウドのテクノロジーと機能を最大限に活用

## 用語

- ワークロード
  - 焦点を絞ったビジネスユースエースを中心にして構成された一つ以上のVMのセット
- 移行
  - ワークロードを移行元の環境から移行先の環境に移行するプロセス
- スプリント
  - 移行作業の一区分。
  - 移行は複数のスプリントで構成される
- Wave
  - 移行するVMをバッチに整理する方法。
  - 一回でまとめて移行する場合のリスクを回避できる。スプリントは一つ以上のWaveで構成される
- RunBook
  - Waveに含めるVMを指定するファイルのこと。移行元と移行先のVMのプロパティも記述される。
  - 一つのWaveには、一つのRunBookが含まれる
- Job
  - RunBook内のVMに対して実行されるオペレーションのこと
  - 一つのWaveには一つ以上のJobを含めることができる
- 実行グループ
  - Wave内で複数のVMを移行する論理的な順序を定義したもの
- スタブVM
  - 移行中に物理サーバと通信するために、VMWare vSphereでVMに移行する管理オブジェクト

![uml](https://cloud.google.com/static/architecture/images/structure-of-migration.svg)

## Links

- [Google Cloud | Migrate for Virtual MachinesによるVMの以降：スタートガイド](https://cloud.google.com/architecture/migrating-vms-migrate-for-compute-engine-getting-started)
- [Google Cloud | Migrate for Virtual MachinesによるVMの移行：VMの移行](https://cloud.google.com/architecture/migrating-vms-migrate-for-compute-engine-migrating-vms)
