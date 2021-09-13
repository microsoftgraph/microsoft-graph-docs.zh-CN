---
title: officeClientCheckinStatus 资源类型
description: 描述租户签入统计数据的实体。
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 416b7f20477109718ab8b2efd26190050d910fda
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064425"
---
# <a name="officeclientcheckinstatus-resource-type"></a>officeClientCheckinStatus 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述租户签入统计数据的实体。
## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|userPrincipalName|String|使用设备的用户主体名称。|
|deviceName|String|尝试签入的设备名称。|
|devicePlatform|String|尝试签入的设备平台。|
|devicePlatformVersion|String|尝试签入的设备平台版本。|
|wasSuccessful|Boolean|如果最后一次签入成功。|
|userId|String|使用设备的用户标识符。|
|checkinDateTime|DateTimeOffset|上次设备签入时间（UTC）。|
|errorMessage|String|错误消息（如果有与最后一个签入相关联）。|
|appliedPolicies|String collection|作为最后一个签入传递到设备的策略列表。|

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



