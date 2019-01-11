---
title: managementAgentType 枚举类型
description: 管理代理类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 66441a37b417cef13cbb09219a26a98250cbf610
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888485"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

管理代理类型。
## <a name="members"></a>成员
|成员|值|Description|
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



