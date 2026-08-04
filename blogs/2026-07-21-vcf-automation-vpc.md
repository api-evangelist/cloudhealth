---
title: "VCF Automation 活用 – 第４部 プライベートクラウドへの「VPC」の必要性とネットワークアーキテクチャ"
url: "https://blogs.vmware.com/vmware-japan/2026/07/vcfa-4.html"
date: "2026-07-21"
author: "susumu nagatoishi"
feed_url: "https://blogs.vmware.com/feed/"
---
このブログでは、VMware Cloud Foundation® 9 （VCF 9）の新機能である VMware Cloud Foundation® Automation（VCF Automation） を複数回のテーマに分けてご紹介していきたいと思います。 第3部では、VCF 9 が「3つの管理者ロール」による職務分離（SoD）に基づき、いかに効率的かつ安全な「次世代テナント管理」を実現するかを、導入・運用フローと共に詳細に解説しました。 第4部では、そのテナント分離技術である「VPC（Virtual Private Cloud）」の概念と、それを支える VCF 9 の次世代ネットワークアーキテクチャについて、VMware NSX® のコンポーネントと関連付けながら詳細に掘り下げます。 プライベートクラウドへの「VPC」の必要性 従来のプライベートクラウドのマルチテナントは、多くの場合、vSphere の「リソースプール」や IAM（Identity and Access Management）による「論理分離」に依存していました。 ? 従来の単一テナントモデル（限界） ハードウェアと VCF 基盤を全社で共有し、プロジェクトは IAM によってアクセス制御されるだけでした。これでは、リソースの競合は防げても、ネットワークレベルの分離は担保されません。 ネットワーク分離（VLAN
