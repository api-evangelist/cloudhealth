---
title: "VCF ネットワークと Infoblox とのシームレスな IPAM (DDI) 連携"
url: "https://blogs.vmware.com/vmware-japan/2026/07/vcf-infoblox.html"
date: "2026-07-29"
author: "susumu nagatoishi"
feed_url: "https://blogs.vmware.com/feed/"
---
このブログでは、 VMware Cloud Foundation® 9 (VCF 9) 環境において IP アドレス運用を効率化する手法についてご紹介します。本内容は、弊社本国の英字ブログ記事の内容を踏まえつつ、メリットや動作について解説を加えております。ぜひ、そちらの記事にもお立ち寄りください。 さて、エンタープライズのクラウドインフラストラクチャにおいて、仮想マシンの展開が迅速化される一方で、ネットワークの払い出しや IP アドレス・ DNS の管理といった周辺タスクがボトルネックになるケースは少なくありません。 VCF 環境において、サードパーティの IPAM （ IP アドレス管理）ソリューションである Infoblox Network Identity Operating System（NIOS） DDI と連携することは、この課題に対応する有効なアプローチの一つです。 本記事では、 VCF と Infoblox NIOS DDI の連携によって実現される主な機能とその仕組み、そしてインフラ運用にもたらすメリットについて解説します。 連携の目的と主な導入メリット VCF と Infoblox を連携させる主な目的は、 IP アドレスと DNS のライフサイクル管理の自動化です。手動での IP アドレスの払い出しや DNS レコードの登録作業を削減することで、以下のようなメ
