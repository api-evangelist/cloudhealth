---
title: "VMware Cloud Foundation における VMware vSphere Kubernetes Service (VKS) の設計およびアーキテクチャ検討について"
url: "https://blogs.vmware.com/vmware-japan/2026/06/vcf-vks-architecture-jpn.html"
date: "2026-06-30"
author: "Shinya Asako"
feed_url: "https://blogs.vmware.com/feed/"
---
最新のアプリケーションを本番環境で正常に稼働させるためには、単に仮想マシン（VM）やコンテナをデプロイするだけでなく、ロードバランサー、永続ストレージ、監視ツールなどの幅広いサービスへのアクセスが必要です。本ブログでは、VMware Cloud Foundation®（VCF）上でKubernetes環境を構築・運用するための設計指針を解説したウェビナー「Design and Architecture Considerations for VKS on VCF」から、VMware vSphere® Kubernetes Service (VKS) を導入する上で重要となる点を抜粋してご紹介します。 1. VMware vSphere® Supervisor と Namespace による統合管理 vSphere...
