---
title: managementAgentType 枚举类型
description: 管理代理类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401003"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理代理类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|eas|1|设备管理 Exchange server。|
|mdm|2|设备管理由 Intune mdm。|
|easMdm|3|设备所管理的 Exchange server 和 Intune mdm。|
|intuneClient|4|Intune 客户端托管。|
|easIntuneClient|5|设备是 EAS 和 Intune 客户端双托管。|
|configurationManagerClient|8|设备管理由配置管理器中。|
|configurationManagerClientMdm|10|设备所管理的配置管理器和 mdm。|
|configurationManagerClientMdmEas|11|配置管理器、 MDM 和 Eas 由管理设备。|
|unknown|16|未知的管理代理类型。|
|jamf|32|从 Jamf 获取设备属性。|
|googleCloudDevicePolicyController|64|由 Google 的 CloudDPC 管理设备。|
|microsoft365ManagedMdm|258|由 Microsoft 365 通过 Intune 管理此设备。|




