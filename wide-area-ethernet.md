# 広域イーサネット

通信事業の提供するイーサネット閉域網を利用してVPNを実現する。

- レイヤ2サービス
  - ネットワーク層プロトコルに制限がない
- VPN通信
  - 拡張VLANタグを利用する

## 拡張VLANタグ

広域イーサネット網に入るとき、拡張VLANタグという独自のVLANタグをパケットに付与し、出るときに除去する。

広域イーサネット網内では、拡張VLANタグ内のVLAN IDが、利用者を識別する固有のVPN情報として用いられる。

この拡張VLANタグは、IEEE802.1QのVLANタグより前の位置に挿入されるため、利用者は自由にVLANを用いることができる。
