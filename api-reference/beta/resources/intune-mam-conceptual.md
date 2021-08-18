---
title: 使用 Microsoft Intune 管理移动应用 - Microsoft Graph API
description: 列出与租户组织的移动应用Graph MAM (MAM)  (相关的适用于 Intune) 的 Microsoft) API。
author: dougeby
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3181c9b4ed2fb287310a0286f276ff2dcac44c5d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262184"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>如何通过 Microsoft Intune 保护公司的应用数据

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。

你可以使用 Intune 应用保护策略帮助保护公司的数据。 由于 Intune 应用保护策略可以独立于任何移动设备管理 (MDM) 解决方案使用，因此，你可以使用它在设备管理解决方案中注册设备或不注册设备来保护公司数据。 通过实现应用级策略，既可以限制对公司资源的访问，也可以将数据保留在 IT 部门的范围之内。

以下 Graph 资源可用于在 Intune 中管理应用保护策略：

- [Android 管理的应用注册](intune-mam-androidmanagedappregistration.md)
- [Android 托管应用安全网络应用验证类型](intune-mam-androidmanagedappsafetynetappsverificationtype.md)
- [Android 托管应用安全网络设备证明类型](intune-mam-androidmanagedappsafetynetdeviceattestationtype.md)
- [Android 托管的应用安全网络评估类型](intune-mam-androidmanagedappsafetynetevaluationtype.md)
- [Android 移动应用标识符](intune-mam-androidmobileappidentifier.md)
- [应用管理级别](intune-mam-appmanagementlevel.md)
- [应用程序类型](intune-wip-applicationtype.md)
- [默认托管的应用保护](intune-mam-defaultmanagedappprotection.md)
- [设备平台类型](intune-wip-deviceplatformtype.md)
- [Intune 品牌打造配置文件](intune-wip-intunebrandingprofile.md)
- [Intune 品牌打造配置文件分配](intune-wip-intunebrandingprofileassignment.md)
- [iOS 管理的应用注册](intune-mam-iosmanagedappregistration.md)
- [iOS 移动应用标识符](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [键/值对](intune-mam-keyvaluepair.md)
- [Mac 应用标识符](intune-mam-macappidentifier.md)
- [受管理的应用剪贴板共享级别](intune-mam-managedappclipboardsharinglevel.md)
- [托管的应用配置](intune-mam-managedappconfiguration.md)
- [受管理应用的数据加密类型](intune-mam-managedappdataencryptiontype.md)
- [托管应用数据输入位置](intune-mam-managedappdataingestionlocation.md)
- [受管理应用的数据存储位置](intune-mam-managedappdatastoragelocation.md)
- [受管理应用的数据传输级别](intune-mam-managedappdatatransferlevel.md)
- [托管应用设备威胁级别](intune-mam-managedappdevicethreatlevel.md)
- [托管的应用诊断状态](intune-mam-managedappdiagnosticstatus.md)
- [受管理应用的已标记原因](intune-mam-managedappflaggedreason.md)
- [托管应用通知限制](intune-mam-managedappnotificationrestriction.md)
- [托管的应用操作](intune-mam-managedappoperation.md)
- [托管应用电话号码重定向级别](intune-mam-managedappphonenumberredirectlevel.md)
- [托管的应用 PIN 字符集](intune-mam-managedapppincharacterset.md)
- [托管的应用策略](intune-mam-managedapppolicy.md)
- [托管应用策略部署摘要](intune-mam-managedapppolicydeploymentsummary.md)
- [每个应用的托管应用策略部署摘要](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [托管的应用保护](intune-mam-managedappprotection.md)
- [托管应用注册](intune-mam-managedappregistration.md)
- [托管的应用修正操作](intune-mam-managedappremediationaction.md)
- [托管应用状态](intune-mam-managedappstatus.md)
- [托管应用原始状态](intune-mam-managedappstatusraw.md)
- [托管浏览器类型](intune-mam-managedbrowsertype.md)
- [托管移动应用](intune-mam-managedmobileapp.md)
- [移动应用标识符](intune-mam-mobileappidentifier.md)
- [目标托管应用组类型](intune-mam-targetedmanagedappgrouptype.md)
- [目标托管应用程序策略分配](intune-mam-targetedmanagedapppolicyassignment.md)
- [目标托管应用保护](intune-mam-targetedmanagedappprotection.md)
- [Windows应用标识符](intune-mam-windowsappidentifier.md)
- [Windows 信息保护](intune-mam-windowsinformationprotection.md)
- [Windows 信息保护应用](intune-mam-windowsinformationprotectionapp.md)
- [Windows 信息保护应用学习摘要](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Windows 信息保护应用锁定程序文件](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Windows 信息保护数据恢复证书](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Windows 信息保护桌面应用](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Windows 信息保护设备注册](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [Windows 信息保护强制级别](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Windows 信息保护 IP 范围集合](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Windows 信息保护网络学习摘要](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Windows 信息保护 PIN 字符要求](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Windows 信息保护策略](intune-mam-windowsinformationprotectionpolicy.md)
- [Windows 信息保护代理域集合](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Windows 信息保护资源集合](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Windows 信息保护应用商店应用](intune-mam-windowsinformationprotectionstoreapp.md)
- [Windows 信息保护擦除操作](intune-mam-windowsinformationprotectionwipeaction.md)