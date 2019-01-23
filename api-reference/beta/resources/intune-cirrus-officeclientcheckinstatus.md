---
title: officeClientCheckinStatus 资源类型
description: 介绍租户中签入 stats 的实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403257"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍租户中签入 stats 的实体。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|userPrincipalName|String|使用设备的用户主体名称。|
|deviceName|String|要签入的设备名称。|
|devicePlatform|String|要签入的设备平台。|
|devicePlatformVersion|String|要签入的设备平台版本。|
|准备成功|Boolean|如果上次签入已成功。|
|userId|String|使用设备的用户标识符。|
|checkinDateTime|DateTimeOffset|最后一个设备签入时间采用 UTC 时间。|
|errorMessage|String|如果有关联的最后一个签入的错误消息。|
|appliedPolicies|String 集合|策略列表送达作为最后一个签入的设备。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



