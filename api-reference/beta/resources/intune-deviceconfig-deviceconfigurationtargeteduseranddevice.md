---
title: deviceConfigurationTargetedUserAndDevice 资源类型
description: 冲突一设备配置策略的摘要。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e246d9731f5ed9d2ea888ba2b53d335fcbca19f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410740"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a>deviceConfigurationTargetedUserAndDevice 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

冲突一设备配置策略的摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceId|String|签入中的设备 id。|
|deviceName|String|签入中的设备的名称。|
|userId|String|在签入的用户 id。|
|userDisplayName|String|在签入的用户的显示名称|
|userPrincipalName|String|在签入用户的 UPN。|
|lastCheckinDateTime|DateTimeOffset|此用户/设备对上一次签入的时间。|

## <a name="relationships"></a>关系
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




