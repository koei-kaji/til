# Best practices for operating containers

- [Best practices for operating containers](#best-practices-for-operating-containers)
  - [Use the native logging mecanisms of containers](#use-the-native-logging-mecanisms-of-containers)
  - [Ensure that your containers are stateless and immutable](#ensure-that-your-containers-are-stateless-and-immutable)
  - [Avoid privileged containers](#avoid-privileged-containers)
  - [Make your application easy to monitor](#make-your-application-easy-to-monitor)
  - [Expose the health of your application](#expose-the-health-of-your-application)
  - [Avoid running as root](#avoid-running-as-root)
  - [Carefully choose the image version](#carefully-choose-the-image-version)
  - [Links](#links)

---

## Use the native logging mecanisms of containers

![Kubernetesでの標準的なログ管理システムを示す図](https://cloud.google.com/static/architecture/images/bp-operating-containers-log-management.svg)
![ログ管理用サイドカーパターン](https://cloud.google.com/static/architecture/images/bp-operating-containers-sidecar.svg)

## Ensure that your containers are stateless and immutable

![Pod内の構成ファイルとしてマウントされたConfigMapを使用してDeploymentの構成を更新する例](https://cloud.google.com/static/architecture/images/bp-operating-containers-configmap.svg)

## Avoid privileged containers

## Make your application easy to monitor

## Expose the health of your application

## Avoid running as root

## Carefully choose the image version

---

## Links

- [Google Cloud | Best practices for operating containers](https://cloud.google.com/architecture/best-practices-for-operating-containers)
