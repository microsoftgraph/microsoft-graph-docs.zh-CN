---
title: 如何通过 Microsoft Intune 保护公司的应用数据
description: Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。
author: tfitzmac
ms.openlocfilehash: dd47d1765d53cb8beed7c3b0e87b330b306f8b12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334508"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>如何通过 Microsoft Intune 保护公司的应用数据

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

Microsoft Intune 应用保护策略可帮助保护公司数据，避免数据丢失。

你可以使用 Intune 应用保护策略帮助保护公司的数据。 因为 Intune 应用程序保护策略可用于独立于任何移动设备管理 (MDM) 解决方案，可用于保护贵公司的数据使用或不注册设备的设备管理解决方案中。 通过实现应用级策略，既可以限制对公司资源的访问，也可以将数据保留在 IT 部门的范围之内。

以下 Graph 资源可用于在 Intune 中管理应用保护策略：

- [Android 管理的应用保护](intune-mam-androidmanagedappprotection.md)
- [Android 管理的应用注册](intune-mam-androidmanagedappregistration.md)
- [Android 移动应用标识符](intune-mam-androidmobileappidentifier.md)
- [应用程序管理级别](intune-mam-appmanagementlevel.md)
- [应用程序类型](intune-wip-applicationtype.md)
- [默认托管的应用保护](intune-mam-defaultmanagedappprotection.md)
- [Intune 品牌配置文件](intune-wip-intunebrandingprofile.md)
- [iOS 管理的应用保护](intune-mam-iosmanagedappprotection.md)
- [iOS 管理的应用注册](intune-mam-iosmanagedappregistration.md)
- [iOS 移动应用标识符](intune-mam-iosmobileappidentifier.md)
- [JSON](intune-mam-json.md)
- [托管应用程序剪贴板共享级别](intune-mam-managedappclipboardsharinglevel.md)
- [托管的应用配置](intune-mam-managedappconfiguration.md)
- [托管应用程序数据的加密类型](intune-mam-managedappdataencryptiontype.md)
- [托管的应用程序数据存储位置](intune-mam-managedappdatastoragelocation.md)
- [托管的应用程序数据传输级别](intune-mam-managedappdatatransferlevel.md)
- [托管的应用诊断状态](intune-mam-managedappdiagnosticstatus.md)
- [托管的应用程序标记原因](intune-mam-managedappflaggedreason.md)
- [托管的应用操作](intune-mam-managedappoperation.md)
- [托管的应用程序 PIN 字符集。](intune-mam-managedapppincharacterset.md)
- [托管的应用策略](intune-mam-managedapppolicy.md)
- [托管应用策略部署摘要](intune-mam-managedapppolicydeploymentsummary.md)
- [每个应用的托管应用策略部署摘要](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [托管的应用保护](intune-mam-managedappprotection.md)
- [托管应用注册](intune-mam-managedappregistration.md)
- [托管的应用程序修复操作](intune-mam-managedappremediationaction.md)
- [托管应用状态](intune-mam-managedappstatus.md)
- [托管应用原始状态](intune-mam-managedappstatusraw.md)
- [托管移动应用](intune-mam-managedmobileapp.md)
- [MDM Windows 信息保护策略](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [移动应用标识符](intune-mam-mobileappidentifier.md)
- [目标托管应用配置](intune-mam-targetedmanagedappconfiguration.md)
- [目标托管应用程序策略分配](intune-mam-targetedmanagedapppolicyassignment.md)
- [目标托管应用保护](intune-mam-targetedmanagedappprotection.md)
- [Windows 信息保护](intune-mam-windowsinformationprotection.md)
- [Windows 信息保护应用](intune-mam-windowsinformationprotectionapp.md)
- [Windows 信息保护应用学习摘要](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [Windows 信息保护应用锁定程序文件](intune-mam-windowsinformationprotectionapplockerfile.md)
- [Windows 信息保护数据恢复证书](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [Windows 信息保护桌面应用](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Windows 的信息保护实施级别](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [Windows 信息保护 IP 范围集合](intune-mam-windowsinformationprotectioniprangecollection.md)
- [Windows 信息保护网络学习摘要](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Windows 信息保护 PIN 字符要求](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [Windows 信息保护策略](intune-mam-windowsinformationprotectionpolicy.md)
- [Windows 信息保护代理域集合](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [Windows 信息保护资源集合](intune-mam-windowsinformationprotectionresourcecollection.md)
- [Windows 信息保护应用商店应用](intune-mam-windowsinformationprotectionstoreapp.md)
