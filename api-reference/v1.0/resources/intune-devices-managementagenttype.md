---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e178c22a13e089b89b709757f38d9abb3cc04df
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731930"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|大通|1|设备由 Exchange 服务器管理。|
|Mdm|2|设备由 Intune MDM 管理。|
|easMdm|3|设备由 Exchange 服务器和 Intune MDM 管理。|
|intuneClient|4|Intune 客户端托管。|
|easIntuneClient|5|设备是 EAS 和 Intune 客户端双重托管的。|
|configurationManagerClient|8 |设备由Configuration Manager管理。|
|configurationManagerClientMdm|10|设备由Configuration Manager和 MDM 管理。|
|configurationManagerClientMdmEas|11|设备由 Configuration Manager、MDM 和 Eas 管理。|
|unknown|16|未知的管理代理类型。|
|jamf|32|设备属性是从 Jamf 提取的。|
|googleCloudDevicePolicyController|64|该设备由 Google 的 CloudDPC 管理。|





