---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eba8ec934a29b78d7e6ca11f288a1bd787338d2b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790926"
---
# <a name="devicemanagementsettings-resource-type"></a>deviceManagementSettings 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|允许设备无需签入即可保持符合性的天数。 有效值为 0 至 120|
|isScheduledActionEnabled|布尔值|是否为规则的计划操作启用此功能。|
|secureByDefault|Boolean|它为 true 时，如果不存在目标符合性策略，则设备应为不符合。|
|enhancedJailBreak|布尔值|功能是否已启用或不适用于增强的 jailbreak 检测。|
|deviceInactivityBeforeRetirementInDay|Int32|如果设备在指定天数内未签入, 则可能会删除公司数据, 并且设备将不受管理。 有效值为30至270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|要用于此帐户的派生的凭据提供程序。 可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec` 或 `intercede`。|
|derivedCredentialUrl|String|派生的凭据提供程序自助服务 URI。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String"
}
```





