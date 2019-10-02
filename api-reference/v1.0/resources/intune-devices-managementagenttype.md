---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df4f3cbe6237471548dced1c13cfef601cbe7965
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356910"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|符合|1|设备由 Exchange server 管理。|
|mdm|双面|设备由 Intune MDM 管理。|
|easMdm|第三章|设备由 Exchange server 和 Intune MDM 管理。|
|intuneClient|4|Intune 客户端托管。|
|easIntuneClient|5|设备为 EAS 和 Intune 客户端双重托管。|
|configurationManagerClient|utf-8|设备由配置管理器管理。|
|configurationManagerClientMdm|10 |设备由 Configuration Manager 和 MDM 管理。|
|configurationManagerClientMdmEas|11x17|设备由 Configuration Manager、MDM 和 Eas 管理。|
|unknown|位|未知的管理代理类型。|
|jamf|32|设备属性是从 Jamf 中提取的。|
|googleCloudDevicePolicyController|64|设备由 Google 的 CloudDPC 管理。|




