---
title: 如何通过 Microsoft Intune 保护公司的应用数据
description: Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 4a09cd527644f58f4389e47a23d96f812705b2d3
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454472"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>如何通过 Microsoft Intune 保护公司的应用数据

命名空间：microsoft.graph

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。

你可以使用 Intune 应用保护策略帮助保护公司的数据。 由于 Intune 应用保护策略可以独立于移动设备管理 (MDM) 解决方案使用，无论是否在设备管理解决方案中注册设备，你都可以保护公司的数据。 通过实现应用级策略，既可以限制对公司资源的访问，也可以将数据保留在 IT 部门的范围之内。

以下 Graph 资源可用于在 Intune 中管理应用保护策略：  

- [Android 管理的应用保护](intune-mam-androidmanagedappprotection.md)
- [Android 管理的应用注册](intune-mam-androidmanagedappregistration.md)
- [Android 移动应用标识符](intune-mam-androidmobileappidentifier.md)
- [应用程序类型](intune-wip-applicationtype.md)
- [默认托管的应用保护](intune-mam-defaultmanagedappprotection.md)
- [设备应用管理](intune-mam-deviceappmanagement.md)
- [设备管理](intune-wip-devicemanagement.md)
- [iOS 管理的应用保护](intune-mam-iosmanagedappprotection.md)
- [iOS 管理的应用注册](intune-mam-iosmanagedappregistration.md)
- [iOS 移动应用标识符](intune-mam-iosmobileappidentifier.md)
- [IP 范围](intune-mam-iprange.md)
- [IPv4 范围](intune-mam-ipv4range.md)
- [IPv6 范围](intune-mam-ipv6range.md)
- [JSON](intune-mam-json.md)
- [键/值对](intune-mam-keyvaluepair.md)
- [受管理的应用剪贴板共享级别](intune-mam-managedappclipboardsharinglevel.md)
- [托管的应用配置](intune-mam-managedappconfiguration.md)
- [受管理应用的数据加密类型](intune-mam-managedappdataencryptiontype.md)
- [受管理应用的数据存储位置](intune-mam-managedappdatastoragelocation.md)
- [受管理应用的数据传输级别](intune-mam-managedappdatatransferlevel.md)
- [托管的应用诊断状态](intune-mam-managedappdiagnosticstatus.md)
- [受管理应用的已标记原因](intune-mam-managedappflaggedreason.md)
- [托管的应用操作](intune-mam-managedappoperation.md)
- [托管的应用 PIN 字符集](intune-mam-managedapppincharacterset.md)
- [托管的应用策略](intune-mam-managedapppolicy.md)
- [托管应用策略部署摘要](intune-mam-managedapppolicydeploymentsummary.md)
- [每个应用的托管应用策略部署摘要](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [托管的应用保护](intune-mam-managedappprotection.md)
- [托管应用注册](intune-mam-managedappregistration.md)
- [托管应用状态](intune-mam-managedappstatus.md)
- [托管应用原始状态](intune-mam-managedappstatusraw.md)
- [托管浏览器类型](intune-mam-managedbrowsertype.md)
- [托管移动应用](intune-mam-managedmobileapp.md)
- [MDM Windows 信息保护策略](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [移动应用标识符](intune-mam-mobileappidentifier.md)
- [代理域](intune-mam-proxieddomain.md)
- [目标托管应用配置](intune-mam-targetedmanagedappconfiguration.md)
- [目标托管应用组类型](intune-mam-targetedmanagedappgrouptype.md)
- [目标托管应用程序策略分配](intune-mam-targetedmanagedapppolicyassignment.md)
- [目标托管应用保护](intune-mam-targetedmanagedappprotection.md)
- [用户](intune-mam-user.md)
- [Windows 信息保护](intune-mam-windowsinformationprotection.md)
- [Windows 信息保护应用](intune-mam-windowsinformationprotectionapp.md)
- [Windows 信息保护应用学习摘要](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Windows 信息保护应用锁定程序文件](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Windows 信息保护数据恢复证书](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Windows 信息保护桌面应用](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Windows 信息保护强制级别](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Windows 信息保护 IP 范围集合](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Windows 信息保护网络学习摘要](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Windows 信息保护 PIN 字符要求](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Windows 信息保护策略](intune-mam-windowsinformationprotectionpolicy.md)
- [Windows 信息保护代理域集合](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Windows 信息保护资源集合](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Windows 信息保护应用商店应用](intune-mam-windowsinformationprotectionstoreapp.md)
