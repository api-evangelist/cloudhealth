---
title: "VMware Cloud Foundation® 9.1 徹底解説！物理と仮想の境界をなくす「VLAN Extension」の全貌"
url: "https://blogs.vmware.com/vmware-japan/2026/07/vlan-extension.html"
date: "2026-07-02"
author: "VMware Community"
feed_url: "https://blogs.vmware.com/feed/"
---
1. はじめに：モダンなVPC環境と「既存の物理ネットワーク」の統合という課題 前回の記事では、VMware Cloud Foundation® 9.1 (以後VCF 9.1)で導入された「Distributed Transit Gateway (DTGW)」と「VNA」によって、エッジのボトルネックを排除した高速な分散ルーティングと、ステートフルなネットワークサービスが両立したことを解説しました。 しかし、実際のデータセンター環境は、すべてが新しく構築される「グリーンフィールド」ばかりではありません。現実には、既存の物理サーバー（ベアメタル）や、従来の物理VLANに依存して稼働しているレガシーな仮想マシン（VM）が多数残っています。 「これらの既存システムを、IPアドレスやゲートウェイ設定を変えずに、どうやって最新のVPC環境と繋ぐのか？」...
