---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0a11300891ca4b12b15de26b5be929823b4a8ddf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751354"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|eas|1|设备由Exchange管理。|
|mdm|2|设备由 Intune MDM 管理。|
|easMdm|3|设备由托管服务器Exchange Intune MDM 管理。|
|intuneClient|4 |Intune 客户端托管。|
|easIntuneClient|5 |设备是 EAS 和 Intune 客户端双托管设备。|
|configurationManagerClient|8 |设备由 Configuration Manager 管理。|
|configurationManagerClientMdm|10  |设备由 Configuration Manager 和 MDM 管理。|
|configurationManagerClientMdmEas|11|设备由 Configuration Manager、MDM 和 Eas 管理。|
|unknown|16 |未知管理代理类型。|
|jamf|32|设备属性从 Jamf 获取。|
|googleCloudDevicePolicyController|64|设备由 Google 的 CloudDPC 管理。|




