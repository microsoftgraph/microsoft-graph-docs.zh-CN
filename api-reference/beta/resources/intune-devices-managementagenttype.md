---
title: managementAgentType 枚举类型
description: 管理代理类型。
ms.openlocfilehash: 334a89c3c8a5934f491626b0956a4532cdf76de0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047774"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





