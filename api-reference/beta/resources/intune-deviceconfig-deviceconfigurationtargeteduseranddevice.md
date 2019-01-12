---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 冲突一设备配置策略的摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 234cc9c909875d835ba54709f30f1ca306eb0954
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947962"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>deviceConfigurationTargetedUserAndDevice 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

冲突一设备配置策略的摘要。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceId|String|签入中的设备 id。|
|deviceName|String|签入中的设备的名称。|
|userId|String|在签入的用户 id。|
|userDisplayName|String|在签入的用户的显示名称|
|userPrincipalName|字符串|在签入用户的 UPN。|
|lastCheckinDateTime|DateTimeOffset|此用户/设备对上一次签入的时间。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





