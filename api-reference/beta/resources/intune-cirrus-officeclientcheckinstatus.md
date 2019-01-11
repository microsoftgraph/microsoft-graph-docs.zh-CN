---
title: officeClientCheckinStatus 资源类型
description: 介绍租户中签入 stats 的实体。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ff75c5d73db35c5c2ff70ad3a3dc3e4509745188
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825231"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

介绍租户中签入 stats 的实体。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|userPrincipalName|字符串|使用设备的用户主体名称。|
|deviceName|String|要签入的设备名称。|
|devicePlatform|字符串|要签入的设备平台。|
|devicePlatformVersion|字符串|要签入的设备平台版本。|
|准备成功|布尔|如果上次签入已成功。|
|userId|String|使用设备的用户标识符。|
|checkinDateTime|DateTimeOffset|最后一个设备签入时间采用 UTC 时间。|
|errorMessage|字符串|如果有关联的最后一个签入的错误消息。|
|appliedPolicies|String 集合|策略列表送达作为最后一个签入的设备。|

## <a name="relationships"></a>Relationships
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



