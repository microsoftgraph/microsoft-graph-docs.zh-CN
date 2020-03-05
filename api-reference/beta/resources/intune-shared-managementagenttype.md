---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5305a0a6e2749851e1669d51310db52e5a587b86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523637"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|符合|1 |设备由 Exchange server 管理。|
|mdm|2 |设备由 Intune MDM 管理。|
|easMdm|3 |设备由 Exchange server 和 Intune MDM 管理。|
|intuneClient|4 |Intune 客户端托管。|
|easIntuneClient|5 |设备为 EAS 和 Intune 客户端双重托管。|
|configurationManagerClient|8 |设备由配置管理器管理。|
|configurationManagerClientMdm|10 |设备由 Configuration Manager 和 MDM 管理。|
|configurationManagerClientMdmEas|11 |设备由 Configuration Manager、MDM 和 Eas 管理。|
|unknown|16 |未知的管理代理类型。|
|jamf|32|设备属性是从 Jamf 中提取的。|
|googleCloudDevicePolicyController|64|设备由 Google 的 CloudDPC 管理。|
|microsoft365ManagedMdm|258|此设备由 Microsoft 365 到 Intune 管理。|



