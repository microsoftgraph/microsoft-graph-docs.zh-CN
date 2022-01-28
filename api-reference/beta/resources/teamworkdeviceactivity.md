---
title: teamworkDeviceActivity 资源类型
description: 表示已启用Microsoft Teams的活动详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 43e9e81eb8c2f921ce3657bf42c4a94f17c7c236
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262336"
---
# <a name="teamworkdeviceactivity-resource-type"></a>teamworkDeviceActivity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示启用[Microsoft Teams的设备（](../resources/teamworkdevice.md)包括连接到该设备的活动外围设备）的活动详细信息。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 teamworkDeviceActivity](../api/teamworkdeviceactivity-get.md)|[teamworkDeviceActivity](../resources/teamworkdeviceactivity.md)|读取 [teamworkDeviceActivity](../resources/teamworkdeviceactivity.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|activePeripherals|[teamworkActivePeripherals](../resources/teamworkactiveperipherals.md)|连接到设备的活动外围设备。|
|createdBy|[identitySet](../resources/identityset.md)|创建设备活动文档的用户的标识。|
|createdDateTime|DateTimeOffset|创建设备活动文档的 UTC 日期和时间。|
|id|String|文档标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改设备活动详细信息的用户的标识。|
|lastModifiedDateTime|DateTimeOffset|上次修改设备活动详细信息的 UTC 日期和时间。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkDeviceActivity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkDeviceActivity",
  "activePeripherals": {
    "@odata.type": "microsoft.graph.teamworkActivePeripherals"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

