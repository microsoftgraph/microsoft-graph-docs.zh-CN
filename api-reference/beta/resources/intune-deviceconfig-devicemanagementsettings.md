---
title: deviceManagementSettings 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f676eed1acbf6711f526e612bd6c073b749607d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417663"
---
# <a name="devicemanagementsettings-resource-type"></a>deviceManagementSettings 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceComplianceCheckinThresholdDays|Int32|允许设备无需签入即可保持符合性的天数。 有效值为 0 至 120|
|isScheduledActionEnabled|Boolean|是否为规则的计划操作启用此功能。|
|secureByDefault|Boolean|它为 true 时，如果不存在目标符合性策略，则设备应为不符合。|
|enhancedJailBreak|Boolean|功能启用或非增强 jailbreak 检测。|
|deviceInactivityBeforeRetirementInDay|Int32|当设备不检查指定天数，公司数据可能会删除，设备将不会在管理下。 有效值 30 到 270|
|derivedCredentialProvider|[derivedCredentialProviderType](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|派生凭据提供程序以使用此帐户。 可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede`。|
|derivedCredentialUrl|String|派生凭据提供程序自助服务 URI。|

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




